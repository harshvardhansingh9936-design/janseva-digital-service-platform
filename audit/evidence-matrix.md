# Week 4 Audit Evidence Matrix

| Audit area | Evidence source | Evidence type | Claim allowed |
|---|---|---|---|
| Prototype structure | `index.html` | Source-level | Describe implemented UI/source characteristics |
| Responsive design | `index.html` CSS/media rules | Source-level | Identify responsive implementation; runtime device performance still requires validation |
| Labels/focus | `index.html` | Source-level | Identify accessibility-oriented implementation |
| Performance | Prototype architecture | Review/benchmark | Define targets and measurement method; no invented runtime score |
| Accessibility | Source + WCAG 2.2 criteria | Review | Report evidence and gaps; no unsupported conformance claim |
| Security | Prototype boundary + OWASP guidance | Risk/design review | Identify applicable production risks and required controls |
| Week 3 QA | `qa/` package and CI workflow | Existing project evidence | Describe QA process and completed smoke checks |
| Backend/integration | No production service in repository | Boundary evidence | Mark as planned/not verified |

## Evidence rule
Every Week 4 claim should be traceable to either project evidence, an authoritative external standard, or an explicitly labelled recommendation/inference.