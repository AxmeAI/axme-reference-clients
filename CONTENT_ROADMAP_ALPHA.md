# axme-reference-clients Content Roadmap (Alpha)

This roadmap defines implementation requirements for turning this repository from skeleton to runnable reference clients.

## Current State

- Contract-first skeleton exists (`enterprise-portal/README.md`).
- No full client application implementation yet.

## Alpha Objectives

- Provide runnable reference clients for enterprise and personal cabinet use-cases.
- Demonstrate access governance, quota/usage visibility, and service-account lifecycle flows.
- Keep integration behavior aligned with canonical public API schemas.

## Required Deliverables

### 1) Enterprise Portal runnable baseline

- Frontend application scaffold with route-level pages:
  - organization/workspace admin
  - access requests queue + review actions
  - quota/usage overview
  - service-account key lifecycle
- API client package with typed request wrappers.
- Local development setup and environment configuration.

### 2) Test and validation baseline

- Smoke tests for critical routes.
- Contract-alignment checks against `axme-spec` schema families.
- CI workflow that runs build + tests.

### 3) Documentation baseline

- Architecture doc (`docs/client-architecture.md`).
- API mapping table (`docs/api-contract-mapping.md`).
- Troubleshooting section for auth/session and scope failures.

## Definition of Ready for Full README

Full product-style README is unlocked when:

1. At least one runnable portal client is merged.
2. Build and smoke tests pass in CI.
3. API mapping and setup docs are published.
4. Alpha disclaimers are present in root and subproject READMEs.
