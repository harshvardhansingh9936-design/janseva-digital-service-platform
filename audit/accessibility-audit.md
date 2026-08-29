# Accessibility Audit

## Framework
WCAG 2.2 is used as the principal reference framework. This is an evidence-oriented prototype review, not a declaration of conformance.

## Findings
| Area | Current evidence | Status | Priority | Validation |
|---|---|---|---|---|
| Language | `lang="en"` is present | Evidence present | P2 | Confirm with accessibility tooling |
| Form labels | Label-oriented controls are present | Evidence present | P1 | Keyboard + screen reader |
| Focus visibility | Focus styling is present | Evidence present | P1 | Keyboard-only test |
| Responsive reflow | Responsive layout/breakpoints are present | Evidence present | P1 | 320px/reflow/zoom testing |
| Colour contrast | Contrast review identifies pairs for validation | Partially verified | P1 | Automated + manual contrast checks |
| Keyboard navigation | Source supports focus-oriented interaction | Not fully verified | P1 | Complete keyboard journey |
| Screen reader | No completed assistive-technology session is claimed | Not verified | P1 | NVDA/VoiceOver/TalkBack testing |
| Error/status announcements | Needs runtime assistive-technology validation | Not verified | P1 | Live-region/status testing |
| Accessible authentication | Production authentication is not implemented | Planned | P1 | Validate final authentication flow |

## Important boundary
Presence of labels, focus styles or responsive CSS is evidence of accessibility-oriented implementation, not proof of WCAG 2.2 AA conformance. Full conformance requires testing the implemented experience, including keyboard operation, zoom/reflow, contrast, error handling and assistive technology.

## Recommendations
- Complete a keyboard-only test of every citizen journey.
- Validate focus order and visible focus at every interactive step.
- Run automated contrast checks and manually verify meaningful states.
- Test with at least one desktop screen reader and one mobile assistive technology in staging.
- Ensure validation errors and dynamic status changes have accessible names and appropriate announcements.
- Apply WCAG 2.2 criteria to the final production authentication and document-upload flows.

## Release condition
Do not claim formal WCAG conformance until representative manual and assistive-technology testing has been completed and documented.