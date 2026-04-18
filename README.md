# Pluralsight (pluralsight)
Pluralsight provides technology skills and engineering intelligence APIs for accessing courses, learning paths, assessments, user progress, channels, teams, and engineering metrics via GraphQL and REST APIs.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Courses, Education, Engineering Metrics, Learning, Skills Assessment, Technology, Video Training

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-04-17

## APIs

30 APIs across Skills GraphQL (courses, content, learning paths, labs, channels, progress, assessments, users, teams) and Flow REST (DORA metrics, coding metrics, collaboration, commits, PRs, repos, tickets, users, teams, integrations) plus legacy REST APIs.

See [apis.yml](apis.yml) for the complete inventory.

## Features

| Name | Description |
|------|-------------|
| Course Catalog API | Access the full course catalog with titles, authors, duration, and release dates via GraphQL. |
| Skills Assessment | Measure technology skills with Skill IQ assessments and track competency levels. |
| Role IQ | Assess role readiness and track skill gaps for technology roles. |
| Learning Progress Tracking | Track course completion, content progress, and daily usage. |
| Channels | Create and manage curated content channels with sections and members. |
| User and Team Management | Manage users, invitations, teams, and permissions via GraphQL. |
| DORA Metrics | Access DevOps Research and Assessment metrics for engineering performance. |
| Coding Metrics | Track code-level productivity metrics and developer activity. |
| Collaboration Metrics | Monitor pull request and code review collaboration patterns. |
| Labs | Access hands-on lab catalog and track lab activity. |
| Practice Exams | Retrieve practice exam attempts and scores for certification prep. |
| Flow Engineering Intelligence | Access commit, PR, ticket, and repository data for analytics. |

## Use Cases

| Name | Description |
|------|-------------|
| LMS Integration | Sync course catalog and completion data with enterprise LMS. |
| Skills Gap Analysis | Assess team skill levels and identify training needs. |
| Engineering Performance | Track DORA metrics and coding activity for engineering teams. |
| Compliance Reporting | Generate training completion reports for regulatory compliance. |
| Onboarding Automation | Automate new hire provisioning and learning path enrollment. |
| Content Curation | Build custom learning channels with curated content. |
| Developer Productivity | Analyze commit and PR data to measure developer productivity. |
| Certification Tracking | Track practice exam scores for certification readiness. |

## Solutions

| Name | Description |
|------|-------------|
| Pluralsight Skills | Technology skills platform with courses, assessments, and learning paths. |
| Pluralsight Flow | Engineering intelligence platform with DORA metrics and coding analytics. |

## Artifacts

### OpenAPI

30 OpenAPI specifications in [openapi/](openapi/) covering Skills GraphQL and Flow REST APIs.

### JSON Schema

51 standalone JSON Schema files in [json-schema/](json-schema/).

### JSON Structure

51 JSON Structure files in [json-structure/](json-structure/).

### JSON-LD

- [Pluralsight Context](json-ld/pluralsight-context.jsonld) — 51 types, 8 properties

### Examples

51 example JSON files in [examples/](examples/).

## Vocabulary

- [Pluralsight Vocabulary](vocabulary/pluralsight-vocabulary.yaml) — 10 resources, 2 APIs, 4 domains, 4 personas

## Rules

- [Pluralsight Spectral Rules](rules/pluralsight-spectral-rules.yml) — 17 rules

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
