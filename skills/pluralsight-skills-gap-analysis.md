---
name: pluralsight-skills-gap-analysis
description: Read Skill IQ and Role IQ results out of Pluralsight to find where a team's skills sit against a role, using only published query and mutation names.
api: pluralsight:pluralsight-graphql-api
endpoint: https://paas-api.pluralsight.com/graphql
operations:
  - skillAssessmentCatalog
  - skillAssessmentResults
  - skillIqsSummary
  - roleIqCatalog
  - roleIqSkills
  - roleIqAssignments
  - roleIqLearnerLevels
  - roleIqsSummary
  - addRole
  - editRole
  - assignUsersToRole
  - assignTeamsToRole
  - deleteRole
  - teams
  - users
generated: '2026-08-29'
method: generated
source: graphql/pluralsight-graphql-operations.json, https://developer.pluralsight.com/docs/getting-started/change-log
---

# Skills gap analysis

## Steps

1. **List the roles.** `roleIqCatalog` returns Pluralsight-curated and custom Role IQs.
   `roleIqSkills` returns the skills that make up a given role.
2. **Read assignments and levels.** `roleIqAssignments` says who is assigned to which role;
   `roleIqLearnerLevels` returns each learner's proficiency level. Both key on `psUserId` and both
   page with `first` / `after`.
3. **Read Skill IQ.** `skillAssessmentCatalog` lists the available assessments;
   `skillAssessmentResults` returns per-learner scores, filtered by `psUserIds`.
4. **Roll up.** `skillIqsSummary` and `roleIqsSummary` give the aggregate views without a
   client-side rollup.
5. **Close the gap (write).** `addRole` creates a custom role, `editRole` changes it,
   `assignUsersToRole` / `assignTeamsToRole` assign it.

## Two things that will surprise you

- **`skillAssessmentCatalog` changed behaviour on 2026-04-29.** It now returns only assessments
  assigned to the plan by default. If you are comparing against a pre-2026 extract, the counts will
  differ for that reason and not because your plan changed. Use the `showOffPlanContent` /
  `isOnPlan` handling if you need the wider set.
- **`stackOverflowTags` no longer exists** on `skillAssessmentCatalog` — removed 2025-11-10. Any
  query or filter still referencing it will fail.

## Reversibility

`assignUsersToRole` and `assignTeamsToRole` have **no published unassign mutation** in Pluralsight's
71-operation index. If you assign a role to the wrong people there is no documented API path to undo
it. Confirm the target set with a human before assigning, and never assign in a loop over an
unverified list.

`addRole` → `deleteRole` exists, with no stated window and no documented restore.

## Rules

- `psUserId` UUIDs everywhere; the legacy `userId` was removed 2025-11-10.
- Read `extensions.warnings` and `errors[]` on every response.
- Page at 1000 records; anything larger is silently truncated and reported only in
  `extensions.warnings`.

## See also

- `changelog/pluralsight-changelog.yml`
- `conventions/pluralsight-conventions.yml`
