# Requirement-to-Test Traceability — Week 3

| Requirement | Week 3 coverage | Primary test(s) | Status |
|---|---|---|---|
| FR-01 Service discovery | Citizen can find services | TC-02 | In scope |
| FR-02 Service information | Eligibility/guidance is understandable | TC-02 | In scope |
| FR-03 Authentication | Sign-in journey and identity expectations | TC-01 | In scope; real IdP planned |
| FR-04 Application form | Required/invalid inputs handled | TC-03 | In scope |
| FR-05 Document upload | Type/size validation expectations | TC-04 | In scope; real storage planned |
| FR-06 Submission | Valid application creates traceable submission | TC-05 | Planned live execution |
| FR-07 Status tracking | Timeline and stage visibility | TC-07 | In scope as UI; live state planned |
| FR-08 Notifications | Notification behaviour and delivery traceability | TC-07 | Integration planned |
| FR-09 Payment | Safe payment/reconciliation behaviour | TC-08 | Planned |
| FR-10 Role-based permissions | Citizen/officer authorization boundaries | TC-06, TC-09 | Planned |
| FR-11 Reporting | Reporting capability | — | Deferred to Week 4 |
| FR-12 Integration | External/service integration | — | Deferred to Week 4 |
| FR-13 Audit logging | Audit events for sensitive actions | TC-06, TC-09 | Planned with backend |
| FR-14 Assisted Service | Assisted-service pathway | — | Deferred to Week 4 |

## Non-functional coverage

| Area | Primary test(s) | Week 3 treatment |
|---|---|---|
| Performance / response time | TC-05, performance plan | Planned for staging |
| Availability | Monitoring / operational checks | Planned for deployed environment |
| Security | TC-08, TC-09, security plan | Planned where backend is required |
| Accessibility | TC-10 | Partial visual review; interactive execution planned |
| Responsive usability | TC-10 | Reviewable in current prototype |
| Data privacy | Test-data policy / TC-09 | Synthetic data only; implementation controls planned |

**Traceability note:** Week 3 covers the requirements that can be meaningfully assessed or planned at the current prototype stage. FR-11, FR-12 and FR-14 are intentionally carried forward to Week 4 rather than being represented as tested in Week 3.
