# Requirement-to-Test Traceability — Week 3

This matrix uses the Week 1 requirement IDs exactly as defined in the project plan. Week 3 documents or assesses the requirements appropriate to the current static prototype stage; FR-11, FR-12 and FR-14 are explicitly deferred to Week 4.

| Requirement | Week 1 meaning | Week 3 primary coverage | Status |
|---|---|---|---|
| FR-01 | Service discovery: search, categories, filters, plain-language guidance | TC-02 | Reviewable in prototype |
| FR-02 | Account & identity: sign-in, identity provider integration, recovery | TC-01 | UI review; live IdP planned |
| FR-03 | Application: save/resume, validation, consent, receipt, reference number | TC-03, TC-05 | UI review; persistent submission planned |
| FR-04 | Documents: upload, metadata, size/type validation, secure storage | TC-04 | UI/rules review; secure storage planned |
| FR-05 | Workflow: queues, assignment, verification, decisions, escalation, SLA | TC-06 | Workflow UI review; live engine planned |
| FR-06 | Status: citizen timeline, current stage, required action, next event | TC-05, TC-07 | UI review; live state planned |
| FR-07 | Payments: approved gateway, receipt, reconciliation | TC-08 | Planned |
| FR-08 | Notifications: event-based delivery, preferences, delivery logs | TC-07 | UI review; integration planned |
| FR-09 | Grievance: capture, routing, acknowledgement, status, closure feedback | TC-07 (extension) | UI review; backend workflow planned |
| FR-10 | Admin: service configuration, workflows, content, roles and permissions | TC-09 | Planned for authenticated build |
| FR-11 | Reporting: volume, completion/drop-off, SLA, satisfaction metrics | — | Deferred to Week 4 |
| FR-12 | Integration: versioned APIs, events/webhooks, legacy adapters | — | Deferred to Week 4 |
| FR-13 | Audit: immutable/tamper-evident logs for sensitive actions | TC-06, TC-09 | Planned with backend |
| FR-14 | Assisted service: staff-assisted mode and accessible alternatives | — | Deferred to Week 4 |

## Non-functional coverage

| Quality attribute | Week 3 primary focus | Status |
|---|---|---|
| Performance | Normal-load response target; load/stress/soak/spike scenarios | Planned for staging |
| Availability | Monitoring and operational readiness; 99.9% target | Planned for deployed environment |
| Security | Authentication, authorization, input/file handling, dependency scanning, penetration strategy | Mostly planned; UI/data handling review only where possible |
| Privacy | Synthetic test data and data-minimisation expectations | Defined now; implementation controls planned |
| Accessibility | Labels, heading structure, focus styling, responsive behaviour, keyboard/screen reader/automated scan strategy | Partial review; interactive checks planned |
| Usability | Plain language, task flow, responsive interaction | Reviewable in prototype |
| Scalability | Load model and stress scenarios | Planned for deployed environment |
| Interoperability | API/event/adapter strategy | Deferred with FR-12 |
| Observability | Logging, metrics, traces and alerts strategy | Planned with backend |
| Maintainability | CI automation and structured QA artefacts | CI smoke check added; full test suite planned |
| Resilience | Failure handling, retry/idempotency and recovery strategy | Planned with backend |

## Coverage rule
A requirement is not marked **Pass** merely because a screen exists. Prototype-reviewable items are labelled as reviewable; backend, integration, infrastructure, or assistive-technology-dependent checks are labelled **Planned** until executed in an appropriate environment.
