# QA Test Data Plan — Week 3

## Data policy
All QA data must be synthetic. Do not use real citizen names, identity numbers, addresses, documents, phone numbers, email addresses or payment credentials.

## Dataset categories
| Dataset | Examples | Purpose |
|---|---|---|
| Valid citizen profile | Synthetic name/contact/address | Happy-path application |
| Boundary profile | Minimum/maximum allowed values | Validation testing |
| Invalid profile | Missing/malformed fields | Negative testing |
| Documents | Synthetic PDF/JPG/PNG, invalid type, oversized file | Upload validation |
| Applications | Draft, submitted, under review, approved, rejected | Status/workflow testing |
| Roles | Synthetic citizen/officer/admin accounts | Authorization testing |
| Payment | Synthetic success/failure/timeout references | Reconciliation scenarios |

## Privacy controls
- Store test data only in approved test environments.
- Keep secrets and credentials out of source control.
- Use masked or generated values in logs.
- Delete temporary test files according to the test-environment retention policy.

## Current prototype
The static prototype does not require a real backend dataset. The dataset definitions above become executable when the interactive application and test services are available.
