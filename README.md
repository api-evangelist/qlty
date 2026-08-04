# Qlty (qlty)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Qlty is a code quality and coverage platform from the team behind Code Climate. It pairs the free Qlty CLI - a polyglot Rust tool for universal linting, auto-formatting, security scanning, and maintainability analysis - with Qlty Cloud, a hosted service for automated pull request review, code coverage upload, quality gates, and dashboards.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/apis.yml)

## Tags

- Code Quality
- Code Coverage
- Static Analysis
- Linting
- Developer Tools

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Qlty CLI

The free Qlty CLI is a polyglot, Rust-based command-line tool for universal linting, auto-formatting, security scanning, code smells, duplication, and maintainability metrics. It runs 70+ static analysis tools across 40+ languages natively (no Docker), is configured via a .qlty/qlty.toml file, and is free for all use including commercial projects. The CLI is a local developer tool, not an HTTP API; key commands include qlty init, qlty check, qlty fmt, qlty smells, qlty metrics, and qlty coverage publish.

- **Human URL:** [https://docs.qlty.sh/cli/quickstart](https://docs.qlty.sh/cli/quickstart)
- **Base URL:** `https://qlty.sh`

#### Tags

- CLI
- Linting
- Formatting
- Static Analysis
- Maintainability

#### Properties

- [Documentation](https://docs.qlty.sh/cli/quickstart)
- [Source Code](https://github.com/qltysh/qlty)
- [OpenAPI](openapi/qlty-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/qlty.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/qlty.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Qlty Coverage Upload

Coverage publishing is performed by the Qlty CLI command qlty coverage publish, which uploads test coverage reports to Qlty Cloud from a CI pipeline. It authenticates with a per-project QLTY_COVERAGE_TOKEN environment variable and accepts standard report formats including lcov, Cobertura, Clover, JaCoCo, SimpleCov, dotCover, and xccov-json. Qlty does not publish a documented public REST endpoint for coverage upload; ingestion is handled through the CLI / GitHub Action.

- **Human URL:** [https://docs.qlty.sh/coverage/quickstart](https://docs.qlty.sh/coverage/quickstart)
- **Base URL:** `https://qlty.sh`

#### Tags

- Code Coverage
- Upload
- CI/CD

#### Properties

- [Documentation](https://docs.qlty.sh/coverage/quickstart)
- [Documentation](https://docs.qlty.sh/coverage/generating-data)
- [OpenAPI](openapi/qlty-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/qlty.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/qlty.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Qlty Cloud API

Qlty Cloud is the hosted platform that analyzes pull requests, posts automated code review comments on newly introduced issues, enforces quality gates, aggregates coverage, and renders trends and dashboards. It is consumed primarily through Git provider integrations (GitHub App / Action) and the web app rather than a documented public REST API; no public HTTP API surface is published as of this catalog entry.

- **Human URL:** [https://docs.qlty.sh/what-is-qlty](https://docs.qlty.sh/what-is-qlty)
- **Base URL:** `https://qlty.sh`

#### Tags

- Cloud
- Pull Request Review
- Quality Gates
- Dashboards

#### Properties

- [Documentation](https://docs.qlty.sh/what-is-qlty)
- [Website](https://qlty.sh/)
- [OpenAPI](openapi/qlty-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/qlty.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/qlty.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/qltysh)
- [LinkedIn](https://www.linkedin.com/company/qltysh)
- [Website](https://qlty.sh/)
- [Documentation](https://docs.qlty.sh)
- [Plans](plans/qlty-plans-pricing.yml)
- [Rate Limits](rate-limits/qlty-rate-limits.yml)
- [Fin Ops](finops/qlty-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
