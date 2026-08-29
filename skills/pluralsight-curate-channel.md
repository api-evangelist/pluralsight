---
name: pluralsight-curate-channel
description: Build and populate a Pluralsight channel — create it, add content and members, assign teams, and archive it — using only published mutations.
api: pluralsight:pluralsight-graphql-api
endpoint: https://paas-api.pluralsight.com/graphql
operations:
  - channels
  - addChannel
  - editChannel
  - channelContent
  - addChannelContent
  - removeChannelContent
  - channelMembers
  - addChannelMembers
  - removeChannelMember
  - addTeamsToChannels
  - channelProgress
  - archiveChannel
  - channelGroup
  - addChannelGroups
  - addChannelsToChannelGroups
  - updateChannelGroups
  - deleteChannelGroup
  - deleteChannelGroupChannels
  - contentSlugToId
  - contentCatalog
generated: '2026-08-29'
method: generated
source: graphql/pluralsight-graphql-operations.json
---

# Curate a Pluralsight channel

Channels are the largest write surface in the Skills GraphQL API — 13 of the 24 published mutations
are channel mutations. All operation names below come from Pluralsight's published operation index.

## Steps

1. **Check whether it already exists.** Query `channels` before creating. There is no idempotency
   key; a repeated `addChannel` creates a second channel.
2. **Create.** `addChannel`, supplying `createdByPsUserId` (UUID — the legacy `createdByUserId` was
   removed 2025-11-10). Use `editChannel` to change name or description later.
3. **Resolve the content you want.** Query `contentCatalog` for candidates, or `contentSlugToId`
   when you have a slug from a Pluralsight URL and need its id. Content types seen in the changelog
   include `COURSE`, `LAB` and `ILX_EXPERIENCE`.
4. **Add content.** `addChannelContent`, passing `actorPsUserId`. Verify with `channelContent`.
5. **Add people.** `addChannelMembers` takes `ownerPsUserId`, `contributorPsUserIds` and
   `memberPsUserIds` as distinct roles — they are not interchangeable. Use `addTeamsToChannels` to
   attach whole teams rather than enumerating members.
6. **Group it (optional).** `addChannelGroups` creates a group; `addChannelsToChannelGroups` puts
   channels in it; `updateChannelGroups` edits it.
7. **Measure.** `channelProgress` returns per-learner progress through the channel, keyed on
   `psUserId`. Page it with `first` / `after`.

## Reversibility

- `addChannel` → `archiveChannel`. This **archives**; Pluralsight does not document whether or for
  how long an archived channel can be restored. Do not tell a user it is undoable.
- `addChannelContent` → `removeChannelContent`; `addChannelMembers` → `removeChannelMember`;
  `addChannelsToChannelGroups` → `deleteChannelGroupChannels`. No windows are stated for any of
  them.
- `addChannelGroups` → `deleteChannelGroup` is a **delete**, not an archive. There is no documented
  restore path. Require human confirmation.

## Rules

- Every actor field is now a UUID `psUserId` / `actorPsUserId` / `ownerPsUserId`.
- Read `extensions.warnings` and `errors[]` on every response.
- No idempotency key, no dry-run. On a timeout, re-query `channels` or `channelContent` to find out
  what landed before retrying.

## See also

- `data-model/pluralsight-data-model.yml` — the Channel / ChannelGroup relationships
- `conventions/pluralsight-conventions.yml`
