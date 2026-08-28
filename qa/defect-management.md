# Defect Management — Week 3

## Severity classification

| Severity | Definition | Example |
|---|---|---|
| Critical | Blocks a core citizen/officer journey, causes data loss/security exposure, or could cause an incorrect payment/decision | Duplicate submission charges a citizen twice |
| High | Major function broken or significantly degraded with little/no workable alternative | Oversized document accepted without validation |
| Medium | Function works but has a meaningful usability, consistency, or minor logic issue | Status label is confusing while the correct stage remains visible |
| Low | Cosmetic or low-impact edge-case issue | Minor spacing inconsistency |

## Defect lifecycle
1. Detect during test/review.
2. Record test case, requirement/screen, steps to reproduce and evidence.
3. Classify severity and priority.
4. Assign for investigation/fix.
5. Retest the fix.
6. Reopen if the defect persists.
7. Close after verification.

## Required defect evidence
Every defect should include:
- Test-case ID
- Requirement ID where applicable
- Steps to reproduce
- Expected result
- Actual result
- Severity and priority
- Affected screen/component
- Screenshot, console output, log, or other reproducible evidence
- Environment/browser information when relevant

## Release blocking
- **Critical:** blocks release until resolved.
- **High:** blocks release unless formally accepted by the authorized risk owner.
- **Medium/Low:** may be scheduled without blocking release, unless a cluster of related defects materially affects a feature.

## Current Week 3 position
No production defect count is claimed because the repository is a static prototype and the full backend/integration test environment is not present. This document defines the process to be used as implementation proceeds.
