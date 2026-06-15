# Pluralsight (pluralsight)

APIs for the Pluralsight technology skills and engineering intelligence platform, providing access to courses, learning paths, assessments, user progress, channels, teams, and engineering metrics via GraphQL and REST APIs.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training

## Timestamps

- **Created:** 2024
- **Modified:** 2026-04-17

## APIs

### Pluralsight Course Catalog API

GraphQL query for accessing course catalog information including titles, descriptions, authors, duration, release dates, and retirement status. Updated daily.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Catalog
- Content
- Courses
- Graphql

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/course-catalog.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/course-catalog.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/course-catalog.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Content Catalog API

GraphQL query for accessing the general content catalog including videos, guides, interactive courses, and other content types beyond traditional courses.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Catalog
- Content
- Graphql

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/content-catalog.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/content-catalog.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/content-catalog.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Learning Paths API

GraphQL query for accessing learning path catalog data including structured sequences of courses and content organized around specific skills and roles.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Catalog
- Content
- Graphql
- Learning Paths

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/learning-paths.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/learning-paths.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/learning-paths.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Labs API

GraphQL queries for accessing lab catalog and lab activity data for hands-on learning experiences and practical exercises.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Catalog
- Graphql
- Hands-On
- Labs

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/labs.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Programs API

GraphQL query for accessing the program catalog including structured learning programs and curriculum offerings.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Catalog
- Curriculum
- Graphql
- Programs

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/programs.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/programs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/programs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Tags API

GraphQL query for accessing content tags and taxonomy data used to categorize and organize learning content.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Content
- Graphql
- Taxonomy

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/tags.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tags.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tags.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Content Slug API

GraphQL query for resolving content slugs to internal identifiers, enabling lookup of content by human-readable URL slugs.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Content
- Graphql
- Identifiers
- Slugs

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/content-slug.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/content-slug.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/content-slug.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Channels API

GraphQL queries and mutations for managing content channels including creating channels, managing members and groups, organizing content sections, and tracking channel progress.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Channels
- Content Curation
- Graphql
- Members

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/channels.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/channels.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/channels.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Course Progress API

GraphQL query for tracking user course progress including completion status and viewing history for video courses. Updated daily.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Completion
- Courses
- Graphql
- Progress

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/course-progress.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/course-progress.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/course-progress.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Content Progress API

GraphQL query for tracking user progress across all content types including videos, guides, paths, interactive courses, and projects. Currently in beta.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Analytics
- Beta
- Content
- Graphql
- Progress

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/content-progress.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/content-progress.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/content-progress.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Course Daily Usage API

GraphQL query for retrieving daily course engagement metrics and usage statistics.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Analytics
- Daily Metrics
- Graphql
- Usage

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/course-daily-usage.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/course-daily-usage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/course-daily-usage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Practice Exams API

GraphQL query for retrieving practice exam attempt data including scores and results.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Assessments
- Certification Prep
- Graphql
- Practice Exams

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/practice-exams.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/practice-exams.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/practice-exams.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Skills Assessment API

GraphQL queries for accessing skill assessments, Skill IQ scores, assessment catalogs, and competency measurements.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Assessments
- Graphql
- Skill Iq
- Skills

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/skills-assessment.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/skills-assessment.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/skills-assessment.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Role IQ API

GraphQL queries and mutations for Role IQ assessments, role catalogs, skill assignments, and user/team role associations.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Assessments
- Graphql
- Role Iq
- Roles
- Skills

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/role-iq.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/role-iq.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/role-iq.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight User Management API

GraphQL queries and mutations for managing users including listing users, inviting members, editing user details, removing users, and canceling invitations.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Graphql
- Invitations
- Licensing
- Users

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/user-management.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/user-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/user-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Teams API

GraphQL queries and mutations for managing teams including creating teams, managing membership, assigning managers, and configuring team permissions.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Graphql
- Management
- Permissions
- Teams

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/teams.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/teams.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/teams.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Plan Info API

GraphQL query for retrieving account and plan details including subscription tier and configuration.

- **Human URL:** [https://developer.pluralsight.com](https://developer.pluralsight.com)
- **Base URL:** `https://paas-api.pluralsight.com/graphql`

#### Tags

- Account
- Graphql
- Plan
- Subscription

#### Properties

- [Documentation](https://developer.pluralsight.com)
- [Graph Q L](https://paas-api.pluralsight.com/graphql)
- [OpenAPI](openapi/plan-info.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/plan-info.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/plan-info.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow DORA Metrics API

REST API for accessing DORA engineering metrics including deployment frequency, lead time for changes, change failure rate, and time to restore service.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/articles/27573677812884-DORA-metrics-API](https://help.pluralsight.com/hc/en-us/articles/27573677812884-DORA-metrics-API)
- **Base URL:** `https://flow-api.pluralsight.com/dora/build-release`

#### Tags

- Change Failure Rate
- Deployment Frequency
- Dora
- Engineering Metrics
- Lead Time

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/articles/27573677812884-DORA-metrics-API)
- [OpenAPI](openapi/flow-dora-metrics.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-dora-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-dora-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Coding Metrics API

REST API for accessing code-level engineering metrics and developer productivity data with date range filtering.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/articles/31476876875028-Updated-Coding-metrics-API](https://help.pluralsight.com/hc/en-us/articles/31476876875028-Updated-Coding-metrics-API)
- **Base URL:** `https://flow-api.pluralsight.com/collaboration/code/metrics`

#### Tags

- Coding Metrics
- Engineering Metrics
- Productivity

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/articles/31476876875028-Updated-Coding-metrics-API)
- [OpenAPI](openapi/flow-coding-metrics.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-coding-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-coding-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Collaboration Metrics API

REST API for accessing pull request and collaboration metrics for engineering teams with date range filtering.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/articles/24286030333332-Collaboration-metrics-API](https://help.pluralsight.com/hc/en-us/articles/24286030333332-Collaboration-metrics-API)
- **Base URL:** `https://api.appfireflow.com/collaboration/pullrequest/metrics`

#### Tags

- Collaboration
- Engineering Metrics
- Pull Requests

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/articles/24286030333332-Collaboration-metrics-API)
- [OpenAPI](openapi/flow-collaboration-metrics.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-collaboration-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-collaboration-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Commits API

REST API for accessing commit data and aggregated commit metrics across repositories.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- **Base URL:** `https://<workspace>.appfireflow.com/v3/customer/core`

#### Tags

- Commits
- Engineering Data
- Source Control

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- [OpenAPI](openapi/flow-commits.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-commits.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-commits.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Pull Requests API

REST API for accessing pull request data, comments, and events across repositories.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- **Base URL:** `https://<workspace>.appfireflow.com/v3/customer/core`

#### Tags

- Code Review
- Engineering Data
- Pull Requests

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- [OpenAPI](openapi/flow-pull-requests.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-pull-requests.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-pull-requests.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Repos API

REST API for accessing repository data and metadata across connected source control systems.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- **Base URL:** `https://<workspace>.appfireflow.com/v3/customer/core`

#### Tags

- Engineering Data
- Repositories
- Source Control

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- [OpenAPI](openapi/flow-repos.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-repos.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-repos.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Users API

REST API for managing Flow users including listing, updating, merging, hiding, and bulk operations on user accounts.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- **Base URL:** `https://<workspace>.appfireflow.com/v3/customer/core`

#### Tags

- Engineering Data
- Management
- Users

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- [OpenAPI](openapi/flow-users.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-users.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-users.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Teams API

REST API for managing Flow engineering teams and team membership data.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- **Base URL:** `https://<workspace>.appfireflow.com/v3/customer/core`

#### Tags

- Engineering Data
- Management
- Teams

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- [OpenAPI](openapi/flow-teams.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-teams.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-teams.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Integrations API

REST API for managing Flow integrations and checking connection status with external tools and services.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/articles/24285986280212-Integrations-API](https://help.pluralsight.com/hc/en-us/articles/24285986280212-Integrations-API)
- **Base URL:** `https://<workspace>.appfireflow.com/v3/customer/core`

#### Tags

- Connections
- Engineering Data
- Integrations

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/articles/24285986280212-Integrations-API)
- [OpenAPI](openapi/flow-integrations.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-integrations.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-integrations.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Flow Tickets API

REST API for accessing ticket data including comments, events, and project associations from connected project management tools.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- **Base URL:** `https://<workspace>.appfireflow.com/v3/customer/core`

#### Tags

- Engineering Data
- Project Management
- Tickets

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/sections/24176771997588-Customer-API-references)
- [OpenAPI](openapi/flow-tickets.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/flow-tickets.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/flow-tickets.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Reports REST API

Legacy REST API for downloading user, course completion, and course usage reports as CSV files. Deprecated as of February 2025, removal scheduled for November 2025.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/articles/24420566008084-Migrating-from-REST-to-GraphQL-APIs](https://help.pluralsight.com/hc/en-us/articles/24420566008084-Migrating-from-REST-to-GraphQL-APIs)
- **Base URL:** `https://app.pluralsight.com/plans/api/reports/v1`

#### Tags

- Csv
- Deprecated
- Legacy
- Reports

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/articles/24420566008084-Migrating-from-REST-to-GraphQL-APIs)
- [OpenAPI](openapi/reports-rest.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/reports-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/reports-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Licensing REST API

Legacy REST API for managing user invitations, users, and teams within a plan. Deprecated as of February 2025, removal scheduled for November 2025.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/articles/24420566008084-Migrating-from-REST-to-GraphQL-APIs](https://help.pluralsight.com/hc/en-us/articles/24420566008084-Migrating-from-REST-to-GraphQL-APIs)
- **Base URL:** `https://app.pluralsight.com/plans/api/license/v1`

#### Tags

- Deprecated
- Invitations
- Legacy
- Licensing
- Users

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/articles/24420566008084-Migrating-from-REST-to-GraphQL-APIs)
- [OpenAPI](openapi/licensing-rest.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/licensing-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/licensing-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pluralsight Public Course Catalog REST API

Legacy public REST API for accessing the full course catalog without authentication. Returns course IDs, titles, durations, release dates, and retirement status.

- **Human URL:** [https://help.pluralsight.com/hc/en-us/articles/24420554286868-Skills-APIs-and-integrations](https://help.pluralsight.com/hc/en-us/articles/24420554286868-Skills-APIs-and-integrations)
- **Base URL:** `https://paas-rest-api.pluralsight.com`

#### Tags

- Catalog
- Courses
- Legacy
- Public

#### Properties

- [Documentation](https://help.pluralsight.com/hc/en-us/articles/24420554286868-Skills-APIs-and-integrations)
- [OpenAPI](openapi/public-course-catalog-rest.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/public-course-catalog-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/public-course-catalog-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/pluralsight)
- [LinkedIn](https://www.linkedin.com/company/pluralsight)
- [Portal](https://developer.pluralsight.com)
- [Getting Started](https://developer.pluralsight.com/docs/getting-started)
- [Authentication](https://developer.pluralsight.com/docs/getting-started)
- [F A Q](https://developer.pluralsight.com/docs/getting-started/faqs)
- [Code Examples](https://developer.pluralsight.com/docs/getting-started/examples)
- [Graph Q L](https://developer.pluralsight.com/docs/getting-started/using-graphql)
- [Documentation](https://developer.pluralsight.com/docs/deprecations/2025-deprecation-guide)
- [Documentation](https://help.pluralsight.com/hc/en-us/articles/24420566008084-Migrating-from-REST-to-GraphQL-APIs)
- [Rate Limits](https://developer.pluralsight.com/docs/rate-limits)
- [Terms of Service](https://www.pluralsight.com/terms)
- [Privacy Policy](https://www.pluralsight.com/privacy)
- [Support](https://help.pluralsight.com)
- [Status Page](https://status.pluralsight.com)
- [Blog](https://www.pluralsight.com/blog)
- [Features](undefined)
- [Use Cases](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
