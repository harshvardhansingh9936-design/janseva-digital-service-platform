# JanSeva Digital Service Platform (JSDSP)

## Project
Responsive citizen-facing prototype developed for the internship task **Junior Web Developer – E-Governance & Digital Services**.

## Week 2 prototype
The prototype translates the Week 1 project plan into a concrete responsive citizen service journey:

Home → Services → Service Details → Sign In → Application → Review → Submission → Status → Help/Grievance

## Features demonstrated
- Service catalogue and search
- Service details and eligibility guidance
- Sign-in / identity UI (simulated)
- Guided application form
- Document upload UI (prototype only)
- Review and submission flow
- Reference number confirmation
- Application status timeline
- Notifications and grievance/help UI
- Officer dashboard demonstration
- Responsive desktop/tablet/mobile layout
- Accessibility-oriented labels, focus states and clear feedback

## Technology
The Week 1 roadmap recommended React + TypeScript for the frontend. Because this submission is a self-contained prototype package, the included runnable reference implementation is delivered as HTML5/CSS3/JavaScript so it can be opened immediately without a build step. The production implementation can be moved to React + TypeScript using the same component and screen structure.

## Representative service
Income Certificate is used only as a **demonstration service** for the prototype. Eligibility, fees and processing details shown in the interface are illustrative and must be replaced by authoritative departmental content in a production system.

## Week 3 — Quality Assurance & Testing
Week 3 defines and documents a comprehensive QA strategy for the JanSeva platform. The work covers functional test planning, test-case design, requirement-to-test traceability, manual versus automated testing, performance and security planning, accessibility, QA risks, defect management, metrics and release exit criteria.

The `qa/` directory contains the Week 3 artifacts:

- [`qa/test-plan.md`](qa/test-plan.md) — overall testing strategy and environments
- [`qa/test-cases.md`](qa/test-cases.md) — ten detailed test scenarios (TC-01–TC-10)
- [`qa/requirement-traceability.md`](qa/requirement-traceability.md) — requirement coverage and Week 4 carry-forward items
- [`qa/test-execution-summary.md`](qa/test-execution-summary.md) — current prototype-review evidence and planned tests
- [`qa/risk-register.md`](qa/risk-register.md) — QA risks and mitigations
- [`qa/defect-management.md`](qa/defect-management.md) — severity, lifecycle and release rules

### Testing status and limitations
The current repository is a self-contained static HTML5/CSS3/JavaScript prototype. It does not contain a production backend, real government identity provider, payment gateway, database, workflow engine, or staging environment.

Accordingly, Week 3 documentation clearly distinguishes **prototype/UI reviewable checks** from **planned infrastructure-dependent tests**. Load testing, penetration testing, real authentication/payment/integration testing, full automated regression execution, and interactive screen-reader/keyboard execution are not represented as completed where the required environment is unavailable.

FR-11 (Reporting), FR-12 (Integration), FR-14 (Assisted Service), and the remaining implementation-dependent regression work are carried forward to Week 4.

## Important
This is an internship prototype and is not an official government service.
