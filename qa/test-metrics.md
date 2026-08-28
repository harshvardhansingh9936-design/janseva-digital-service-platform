# QA Metrics & Release Criteria — Week 3

## Core QA metrics
| Metric | Definition | Use |
|---|---|---|
| Test-case completion | Executed applicable tests / planned executable tests × 100 | Measures execution progress |
| Pass rate | Passed executed tests / executed tests × 100 | Indicates current quality status |
| Defect density | Valid defects / agreed scope size | Tracks defect concentration when implementation size is measurable |
| Critical/High open defects | Count of unresolved Critical and High defects | Release risk indicator |
| Defect leakage | Post-release defects / total defects | Measures escaped defects in later phases |
| Regression pass rate | Passed regression tests / executed regression tests × 100 | Protects previously working functionality |
| Accessibility defect count | Open accessibility findings by severity | Accessibility release readiness |
| Performance p95 | 95th-percentile response time for defined workloads | Performance readiness |

## Release gate
A release candidate should not be approved until:
- No Critical defects remain open.
- High defects are fixed or formally risk-accepted by the authorized owner.
- All in-scope executable requirements have passing evidence.
- Core citizen screens meet the agreed accessibility gate.
- Staging performance thresholds are met.
- Required security scans and penetration testing have no open Critical/High findings.
- Regression coverage is executed for affected areas.

## Week 3 interpretation
The current repository is a static prototype, so production defect counts, performance measurements, security-scan results and uptime are **not claimed** here. The metrics and gates define how release readiness will be measured once the interactive implementation and staging environment exist.
