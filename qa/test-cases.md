# Week 3 Test Cases

> Status values are intentionally conservative: prototype-review checks are not presented as backend execution results.

## TC-01 — Sign-in journey
**Priority:** High  
**Type:** Manual / future automated E2E  
**Current status:** Partial — UI journey review only

**Precondition:** Prototype is open.

**Steps:**
1. Open Sign in.
2. Review the identity fields and labels.
3. Submit empty or incomplete input where the prototype permits interaction.
4. Observe feedback and navigation.

**Expected:** Clear labels and feedback are provided; authentication is not represented as a real identity-provider transaction in the current prototype.

## TC-02 — Service discovery and eligibility
**Priority:** High  
**Type:** Manual / future E2E  
**Current status:** Reviewable in prototype

**Steps:** Search/browse Services → open Income Certificate → review service description, eligibility and guidance → continue to application.

**Expected:** Relevant service information is presented clearly and the user can proceed through the intended journey.

## TC-03 — Application form validation and save/resume
**Priority:** High  
**Type:** Manual now / unit + E2E later  
**Current status:** Partial — interface and validation expectations reviewed

**Steps:** Open application → inspect required fields → submit incomplete data → correct invalid data → review the form flow.

**Expected:** Required/invalid fields receive clear feedback; valid information can proceed to review. Persistent save/resume requires a backend and is planned.

## TC-04 — Document upload validation
**Priority:** High  
**Type:** Manual now / integration later  
**Current status:** Partial — upload UI reviewed

**Steps:** Open upload stage → attempt supported and unsupported file scenarios in an interactive build → test size boundary → continue.

**Expected:** File type/size rules are enforced and useful error messages are shown. Real storage/upload execution requires backend infrastructure and is planned.

## TC-05 — Submission and reference number
**Priority:** Critical  
**Type:** E2E  
**Current status:** Planned for live workflow

**Steps:** Complete valid application → review → submit → verify confirmation and unique reference number → reopen status journey.

**Expected:** A successful submission produces one traceable reference number and the application becomes trackable. Duplicate/failed submission behaviour must not create unintended duplicate records or charges.

## TC-06 — Officer case-processing workflow
**Priority:** High  
**Type:** System/E2E  
**Current status:** Planned

**Steps:** Sign in as authorized officer → locate case → review submitted data/documents → update case stage → verify audit trail and citizen-visible status.

**Expected:** Authorized officers can process assigned cases; unauthorized roles cannot access officer functions; status and audit events remain consistent.

## TC-07 — Status timeline and notification delivery
**Priority:** High  
**Type:** System/E2E  
**Current status:** Reviewable as prototype UI; delivery planned

**Steps:** Open application status → inspect timeline → trigger a status change in an interactive environment → verify notification record/delivery log.

**Expected:** Current stage is understandable and notification delivery is traceable. Real notification dispatch requires service integration.

## TC-08 — Payment and reconciliation
**Priority:** Critical  
**Type:** Integration/E2E  
**Current status:** Planned

**Steps:** Initiate payment → complete success path → verify single transaction/reference → simulate timeout/failure → retry safely → reconcile application/payment records.

**Expected:** No duplicate charge or duplicate application is created; failures are recoverable and reconciliation is auditable.

## TC-09 — Role-based access control and security
**Priority:** Critical  
**Type:** Security/system  
**Current status:** Planned for deployed backend

**Steps:** Attempt citizen access to officer routes; attempt unauthorized record access; test session expiry; test malformed/injection-style inputs and upload boundaries in the secured application.

**Expected:** Unauthorized actions are denied, sessions are handled securely, inputs are validated, and security-relevant events are auditable.

## TC-10 — Accessibility and responsive behaviour
**Priority:** High  
**Type:** Manual + automated accessibility  
**Current status:** Partial — visual/responsive review; interactive accessibility execution planned

**Steps:** Review desktop/tablet/mobile layouts → inspect labels, focus styling and readable hierarchy → execute keyboard-only navigation on interactive build → run axe-core/WAVE → conduct NVDA/VoiceOver walkthrough.

**Expected:** Layout remains usable at target breakpoints; interactive controls are keyboard accessible; no critical accessibility violations occur on core journey screens.
