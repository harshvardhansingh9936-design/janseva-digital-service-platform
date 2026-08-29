# Production Readiness Checklist

Use this checklist after the prototype stage and before public or pilot deployment.

## Performance
- [ ] Staging environment established
- [ ] Core Web Vitals measured at p75
- [ ] Performance budgets defined and enforced
- [ ] Representative mobile and constrained-network testing completed
- [ ] Production assets compressed/cached/optimized

## Accessibility
- [ ] Keyboard-only end-to-end journey completed
- [ ] Contrast validated for normal and interactive states
- [ ] Screen-reader testing completed
- [ ] Zoom/reflow tested
- [ ] Form errors and dynamic status updates announced appropriately
- [ ] WCAG 2.2 findings remediated or formally accepted

## Security
- [ ] Server-side authentication implemented
- [ ] Server-side authorization/RBAC and IDOR protections tested
- [ ] Server-side input validation and output encoding implemented
- [ ] Parameterized database access used
- [ ] Secure file-upload controls implemented
- [ ] HTTPS, security headers and secure cookies configured
- [ ] Rate limiting and abuse protection implemented
- [ ] Security logging and monitoring implemented
- [ ] Dependency/security scanning enabled
- [ ] Staging security testing completed

## Quality and operations
- [ ] Full integration/E2E/regression suite executed
- [ ] Release evidence stored
- [ ] Defects triaged and P0/P1 issues closed or formally accepted
- [ ] Rollback and incident-response procedures tested
- [ ] Production monitoring and alerting configured

## Release decision
The prototype should not be treated as production-ready until the applicable checks above have evidence from a representative staging/deployment environment.