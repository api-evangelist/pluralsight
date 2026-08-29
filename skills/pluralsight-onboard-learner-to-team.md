---
name: pluralsight-onboard-learner-to-team
description: Invite or create a Pluralsight learner, place them on a team, and know exactly what can and cannot be undone — there is no idempotency key on any of these mutations.
api: pluralsight:pluralsight-graphql-api
endpoint: https://paas-api.pluralsight.com/graphql
operations:
  - users
  - memberInvites
  - inviteMember
  - createUser
  - cancelInvite
  - teams
  - addTeam
  - addTeamMember
  - addTeamManager
  - moveMemberToTeam
  - removeTeamMember
  - removeUser
  - removeLicense
generated: '2026-08-29'
method: generated
source: graphql/pluralsight-graphql-operations.json, https://developer.pluralsight.com/docs/getting-started/license-management
---

# Onboard a learner onto a team

Every operation named above is a real, published Pluralsight GraphQL operation. This skill writes —
read the reversibility section before you run it.

## Steps

1. **Check for an existing user.** Query `users` filtered by email before creating anything. There
   is no idempotency key, so a duplicate `createUser` is a duplicate record, not a no-op.
2. **Check for an outstanding invite.** Query `memberInvites` — the learner may already have been
   invited and not yet redeemed.
3. **Invite or create.** Use `inviteMember` for the normal email-redemption flow, or `createUser`
   where your plan provisions directly. `inviteManager` invites a team manager.
4. **Ensure the team exists.** Query `teams`; create with `addTeam` only if it does not.
5. **Place the learner.** `addTeamMember` for a member, `addTeamManager` for a manager. Use
   `moveMemberToTeam` to relocate someone who is already on another team — capture their current
   team first, because the only way to reverse it is to move them back.
6. **Verify.** Re-query `teams` / `teamManagers` and confirm the membership landed.

## Reversibility — read this before you write

Pluralsight publishes **no reversal window** for any of these operations. What exists:

| You did | You can undo with | Window |
|---|---|---|
| `inviteMember` / `inviteManager` | `cancelInvite` | only while the invite is unredeemed; no stated expiry |
| `createUser` | `removeUser` | none stated |
| `addTeamMember` | `removeTeamMember` | none stated |
| `addTeamManager` | `removeTeamManager` | none stated |
| `moveMemberToTeam` | `moveMemberToTeam` back | you must already know the prior team |
| `addTeam` | `deleteTeam` | no documented restore of the deleted team or its membership |
| `removeLicense` | **nothing** | there is no published re-grant mutation |
| `editUser` | `editUser` with the prior values | you must have captured them first |

**`removeLicense` has no published inverse.** Treat it as irreversible and require human
confirmation before calling it.

## Rules

- **No idempotency key exists.** On a timeout, do NOT blind-retry — re-query `users` or
  `memberInvites` to find out whether the first call landed, then decide.
- **No dry-run mode exists.** There is no way to rehearse these mutations.
- Use `psUserId` (UUID). The legacy `userId` was removed 2025-11-10.
- Check `errors[]` and `extensions.warnings` on every response; HTTP 200 does not mean success.

## See also

- `conventions/pluralsight-conventions.yml` — the full reversibility block
- `lifecycle/pluralsight-lifecycle.yml` — the psUserId migration
