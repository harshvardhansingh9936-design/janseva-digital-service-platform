# Security Test Plan — Week 3

## Objective
Define security verification activities for the JanSeva platform without claiming production security testing that cannot be performed against the current static prototype.

## Security areas
| Area | Test focus | Current status |
|---|---|---|
| Authentication | Credential handling, session lifecycle, lockout/recovery expectations | Planned for real IdP |
| Authorization / RBAC | Citizen/officer/admin boundary enforcement | Planned for backend |
| Input validation | Injection-style inputs, malformed values, boundary values | Planned/partial UI review |
| File handling | Type, size, filename/content validation and safe storage | Planned for backend |
| Session security | Expiry, logout, fixation/hijacking protections | Planned for backend |
| Data protection | Encryption in transit/at rest and minimisation | Planned for deployed system |
| Dependencies | Vulnerability/dependency scanning | Planned when dependencies are introduced |
| SAST | Static security analysis | Planned for implementation pipeline |
| Audit integrity | Sensitive-event logging and tamper resistance | Planned with backend |
| Penetration testing | Approved black/grey-box testing of deployed target | Planned |

## Test principles
- Never use real citizen PII in test environments.
- Do not test third-party production systems without explicit authorization.
- Record reproducible evidence for every finding.
- Critical/High security findings require remediation or formal risk acceptance before release.

## Recommended tooling
CI-integrated SAST and dependency scanning, plus approved DAST/penetration-testing tooling when the deployed test environment exists.

## Current prototype boundary
The current repository is static HTML/CSS/JavaScript. Its source can be reviewed for security-conscious structure, but source review does not prove authentication, authorization, cryptographic, database or gateway security. Those checks remain planned.
