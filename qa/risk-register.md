# QA Risk Register — Week 3

| ID | Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|---|
| RT-01 | Regression in payment reconciliation after a code change | Medium | High | Automated integration coverage on every merge once payment integration exists; explicit TC-08 reconciliation scenario. |
| RT-02 | Accessibility defects reach production because manual checks are skipped | Medium | High | Automated accessibility gate plus scheduled manual keyboard/screen-reader review. |
| RT-03 | Load/stress testing is postponed until after an incident | Medium | High | Include performance testing in the release plan and exit criteria. |
| RT-04 | Test data contains real citizen PII | Low | High | Synthetic-data-only policy and controlled test-environment access. |
| RT-05 | Automated suite creates false confidence by covering only happy paths | Medium | Medium | Require edge cases and failure paths in test cases. |
| RT-06 | Two officers act on the same case concurrently | Low | Medium | Add concurrency testing to TC-06 when workflow backend exists. |
| RT-07 | Notification delivery silently fails | Medium | Medium | Delivery logs, reconciliation and alerting when notification integration exists. |
| RT-08 | Security testing is treated as a one-time pre-launch activity | Medium | High | CI SAST/dependency scanning plus periodic security review and penetration testing. |

## Risk treatment principle
The current prototype stage is intentionally not presented as having resolved infrastructure-dependent risks. The mitigations above define controls and tests for the implementation stages where those risks become executable.
