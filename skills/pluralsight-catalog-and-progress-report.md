---
name: pluralsight-catalog-and-progress-report
description: Pull the Pluralsight course/content catalog and per-learner progress out of the Skills GraphQL API into a report, paging safely and without silently truncating the result set.
api: pluralsight:pluralsight-graphql-api
endpoint: https://paas-api.pluralsight.com/graphql
operations:
  - courseCatalog
  - contentCatalog
  - pathCatalog
  - labCatalog
  - courseProgress
  - contentProgress
  - courseDailyUsage
  - labProgress
generated: '2026-08-29'
method: generated
source: https://developer.pluralsight.com/docs/getting-started/pagination, graphql/pluralsight-graphql-operations.json
---

# Report on catalog and learner progress

All eight operations below are real, published Pluralsight GraphQL operations (see
`graphql/pluralsight-graphql-operations.json`). They are queries — this skill never writes.

## Before you start

- You need a plan-admin API key from https://developer.pluralsight.com/manage-keys.
- Confirm the plan actually carries the API entitlement at
  https://developer.pluralsight.com/plan-permissions. Without it every call returns
  `401 {"error":"AuthenticationError: Invalid API Key"}`.
- If any field you intend to select is tagged Beta, the key must have Beta access or the **entire**
  call fails — not just that field.

## Steps

1. **Read the catalog.** Call `courseCatalog` for video courses, or `contentCatalog` for the
   superset (courses, interactive courses, code labs, guides). Use `pathCatalog` and `labCatalog`
   for learning paths and labs.
2. **Page with cursors, not offsets.** Pass `first: 1000` and, on every subsequent call,
   `after: <the previous response's pageInfo.endCursor>`. Stop when `pageInfo.hasNextPage` is false.
   Do not ask for more than 1000 — see the truncation rule below.
3. **Read progress.** Call `courseProgress` / `contentProgress` / `labProgress` filtered to the
   learners and window you need. Use `courseDailyUsage` for day-level usage.
4. **Filter aggressively.** Pluralsight's own guidance is one query per API with tight filters — a
   30- or 90-day window on `courseProgress` rather than an unbounded pull. This is a documented
   performance requirement, not a preference.
5. **Join on `psUserId`.** Progress records key on `psUserId` (a UUID). The old integer `userId` was
   removed on 2025-11-10 and a user's `psUserId` is a different value from their old `userId` — do
   not attempt to map between them.

## Rules you must not skip

- **Check `extensions.warnings` on every response.** It carries both deprecation notices and the
  page-size truncation notice. If you request more than the batch limit the API does **not** error —
  it quietly returns fewer records and tells you only in this field. A report built without reading
  it can be silently incomplete.
- **Check `errors[]` on every response.** GraphQL returns HTTP 200 on field-level failures.
- **On 429, back off exponentially with jitter.** Pluralsight publishes no numeric limit, no window
  and no `RateLimit-*` or `Retry-After` header contract. Reducing page size is the only lever you
  have.
- Do not assume totals: `totalCount` is available on connections, but reconcile it against the
  number of nodes you actually collected.

## See also

- `conventions/pluralsight-conventions.yml` — pagination, error envelope, rate-limit signal
- `errors/pluralsight-problem-types.yml`
- `data-model/pluralsight-data-model.yml`
