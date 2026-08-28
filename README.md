# JanSeva Digital Service Platform (JSDSP)

## Project
Responsive citizen-facing prototype developed for the internship task **Junior Web Developer – E-Governance & Digital Services**.

## Prototype journey
Home → Services → Service Details → Sign In → Application → Review → Submission → Status → Help/Grievance

## Features demonstrated
- Service catalogue and search
- Service details and eligibility guidance
- Simulated sign-in / identity UI
- Guided application form
- Document-upload UI (prototype only)
- Review and submission flow
- Reference-number confirmation
- Application-status timeline
- Notification and grievance/help UI
- Officer dashboard demonstration
- Responsive desktop/tablet/mobile layout
- Accessibility-oriented labels, focus states and clear feedback

## Technology
The Week 1 roadmap recommended React + TypeScript for the production frontend. For this self-contained internship prototype, the runnable reference implementation uses HTML5, CSS3 and JavaScript so it can be opened without a build step. The screen and component structure can be migrated to a production framework later.

## Representative service
Income Certificate is used as a **demonstration service**. Eligibility, fees and processing details shown in the prototype are illustrative and must be replaced with authoritative departmental content before any production use.

## Week 3 — Quality Assurance & Testing
Week 3 adds a structured QA package covering test planning, ten test cases, requirement traceability, prototype-review evidence, manual versus automated testing, performance/security/accessibility strategy, risk management and defect management.

See [`qa/README.md`](qa/README.md) for the QA artifact index.

### Current testing boundary
The repository is a static prototype. It does not contain a production backend, database, real identity provider, payment gateway, notification service, workflow engine or staging environment. Therefore, infrastructure-dependent checks are documented as **Planned** rather than claimed as completed.

A lightweight GitHub Actions workflow (`.github/workflows/qa.yml`) performs repository-integrity, HTML-sanity and QA-artifact smoke checks on pushes and pull requests.

### Week 4 carry-forward
FR-11 Reporting, FR-12 Integration and FR-14 Assisted Service are intentionally deferred to Week 4, together with backend-dependent integration, full E2E/regression execution, staging performance testing and deployed-environment security testing.

## Important
This is an internship prototype and is not an official government service.
