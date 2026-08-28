# Accessibility QA Checklist — Week 3

## Purpose
Provide a repeatable checklist for the core citizen journey and distinguish source-level review from interactive assistive-technology execution.

## Source and UI review
- [x] Document declares `lang="en"`.
- [x] Responsive viewport metadata is present.
- [x] Form controls use labels in the current prototype where applicable.
- [x] Search controls have accessible labels.
- [x] Navigation has an accessible navigation label.
- [x] Focus styling is defined for form controls.
- [x] Responsive breakpoints are defined for tablet/mobile layouts.
- [ ] Full keyboard-only journey execution — planned on interactive build.
- [ ] Screen-reader walkthrough with NVDA/VoiceOver — planned.
- [ ] Automated axe-core/WAVE scan — planned.

## Manual test journey
1. Start at Home.
2. Navigate to Services.
3. Open Income Certificate.
4. Move through application/review/status screens.
5. Check heading order, visible focus, labels, instructions and error feedback.
6. Repeat at desktop, tablet and mobile widths.

## Acceptance guidance
Core citizen screens should have no critical accessibility violations before release. Keyboard and screen-reader checks must be completed on the interactive build; their absence from the current prototype stage is not treated as a pass.

## Evidence
Record browser, viewport, assistive technology/version where applicable, test date, result, defect ID and screenshot or scan output.
