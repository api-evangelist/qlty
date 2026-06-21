# Qlty (qlty)

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
