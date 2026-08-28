# Week 3 QA Documentation — JanSeva Digital Service Platform

This directory contains the Quality Assurance and Testing Strategy artifacts for Week 3 of the Junior Web Developer – E-Governance & Digital Services internship task.

## QA objective
Establish a practical, traceable and repeatable approach for checking the JanSeva citizen-service journey before release, with the Income Certificate journey used as the representative service.

## What is covered
- Functional test planning
- Unit, integration, system and UAT/E2E test levels
- Ten detailed test scenarios (TC-01–TC-10)
- Requirement-to-test traceability for FR-01–FR-14
- Manual versus automated execution strategy
- Responsive and accessibility review
- Performance, stress, soak and spike test planning
- Security and role/permission test planning
- Synthetic QA test-data policy
- QA risk register
- Defect lifecycle and release-blocking rules
- Test metrics and exit criteria
- Repository-integrity CI smoke checks

## Artifact index
| Artifact | Purpose |
|---|---|
| [`test-plan.md`](test-plan.md) | Overall QA strategy, scope, environments, data, entry/exit criteria and automation approach |
| [`test-cases.md`](test-cases.md) | Ten detailed scenarios with preconditions, steps, expected outcomes, priority and execution status |
| [`requirement-traceability.md`](requirement-traceability.md) | Maps Week 1 requirements to Week 3 coverage and identifies Week 4 carry-forward items |
| [`test-execution-summary.md`](test-execution-summary.md) | Conservative record of prototype-review observations versus infrastructure-dependent planned tests |
| [`performance-plan.md`](performance-plan.md) | Proposed baseline, peak, stress, soak and spike scenarios with measurable thresholds |
| [`security-plan.md`](security-plan.md) | Authentication, authorization, input, file, dependency, SAST and penetration-testing strategy |
| [`accessibility-checklist.md`](accessibility-checklist.md) | Source/UI checklist and planned keyboard, screen-reader and automated accessibility checks |
| [`test-data.md`](test-data.md) | Synthetic test-data categories and privacy controls |
| [`risk-register.md`](risk-register.md) | QA risks, likelihood, impact and mitigation controls |
| [`defect-management.md`](defect-management.md) | Severity definitions, evidence requirements, lifecycle and release rules |
| [`test-metrics.md`](test-metrics.md) | QA metrics, release gates and interpretation for the current prototype stage |
| [`.github/workflows/qa.yml`](../.github/workflows/qa.yml) | Lightweight CI smoke checks for project integrity, HTML sanity, accessibility-oriented source markers and QA documentation links |

## Current implementation boundary
The repository is a self-contained HTML5/CSS3/JavaScript prototype. It does not provide a production backend, database, real identity provider, payment gateway, notification service, workflow engine or staging environment.

Consequently, this repository does **not** claim completed backend, payment, penetration, load, screen-reader or full automated regression results. Where execution depends on missing infrastructure, the artifact is explicitly marked **Planned**.

## Prototype-review evidence policy
A prototype review can establish that a UI characteristic is represented in the source, but it cannot prove production behaviour such as persistent storage, authorization enforcement, payment settlement, notification delivery or uptime. Those checks are carried forward to the implementation stage where they can be executed properly.

## Week 4 carry-forward
- FR-11 Reporting
- FR-12 Integration
- FR-14 Assisted Service
- Backend/database integration
- Live identity and payment integrations
- Full E2E/regression execution
- Staging load/stress/soak/spike testing
- Security scanning and penetration testing in an approved test environment
- Interactive keyboard and screen-reader validation
