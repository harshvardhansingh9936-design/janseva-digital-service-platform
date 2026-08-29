# Week 4 Audit Execution Schedule

This schedule documents the five-stage audit process used for the final Week 4 assessment. It separates completed source-level review from validation that requires infrastructure not present in the static prototype.

| Stage / Day | Activity | Evidence / Output | Status |
|---|---|---|---|
| Day 1 — Scope & evidence | Confirm Week 1–3 continuity, inspect the GitHub main branch, and define evidence boundaries plus severity/priority criteria. | Scope, evidence sources, limitations and assessment method. | Completed |
| Day 2 — Performance | Inspect HTML/CSS/JavaScript architecture, dependencies and responsive breakpoints; define KPI targets and measurement methods. | Performance benchmark framework and source-level findings. | Completed |
| Day 3 — Accessibility | Review semantic structure, labels, ARIA, focus, responsive source characteristics and colour contrast against WCAG 2.2. | WCAG-oriented findings and computed contrast evidence; interactive checks identified as planned. | Completed |
| Day 4 — Security | Review authentication, access control, input handling, uploads, headers, dependencies and logging against OWASP Top 10:2025. | SF-01–SF-12 findings with severity, evidence, validation and remediation. | Completed |
| Day 5 — Synthesis & remediation | Cross-reference findings, prioritize P0–P3 actions, prepare scorecard, evidence matrix and production-readiness checklist. | Final audit conclusions and prioritized improvement plan. | Completed |

## Evidence rule
The schedule does not imply that infrastructure-dependent tests were executed. Live performance measurement, DAST/penetration testing, server-side injection testing, interactive keyboard/screen-reader sessions, load/stress testing, and real authentication/payment testing remain planned until an appropriate staging environment exists.
