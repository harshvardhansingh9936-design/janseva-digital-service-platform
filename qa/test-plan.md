# Week 3 Test Plan

## 1. Purpose
This test plan defines the QA approach for the JanSeva Digital Service Platform (JSDSP), with the Income Certificate journey used as the representative service.

## 2. Scope
### In scope for this QA cycle
- Citizen service discovery and eligibility information
- Sign-in UI and authentication journey design
- Application form validation and review flow
- Document-upload interface and validation rules
- Submission and reference-number journey
- Application-status timeline
- Officer case-processing workflow
- Notification behaviour
- Role-based access-control expectations
- Accessibility and responsive UI review

### Deferred to Week 4 / later implementation
- FR-11 Reporting
- FR-12 Integration
- FR-14 Assisted Service
- Live identity-provider integration
- Live payment gateway integration
- Backend/database integration
- Full automated regression execution
- Load/stress execution against a staging backend
- Penetration testing against a deployed environment

## 3. Test Levels
1. **Unit:** validation rules, eligibility logic, date/file-size checks, and reusable UI components once component tests are available.
2. **Integration:** API/workflow, storage, notification, identity, and payment adapters when backend services exist.
3. **System:** complete platform behaviour against in-scope requirements, including permissions and audit logging.
4. **UAT/E2E:** complete citizen and officer journeys.
5. **Manual & accessibility:** exploratory review, keyboard navigation, screen-reader review, and automated accessibility scanning.

## 4. Test Environment
Current: browser-based static prototype using HTML5, CSS3 and JavaScript.

Future execution environment: deployed application + test backend + staging database + synthetic data + test identity/payment integrations.

## 5. Test Data
Use synthetic citizen identities, synthetic documents, boundary-value inputs, invalid file types/sizes, duplicate-submission scenarios, and representative officer accounts. Real citizen PII must not be used in test data.

## 6. Entry Criteria
- Relevant build is available.
- Requirements/test scope is approved.
- Test data is available.
- Required test environment and integrations are accessible for the applicable test level.

## 7. Exit Criteria
- Zero open Critical defects.
- High defects fixed or formally accepted by the authorized risk owner.
- All in-scope traceability rows have an appropriate passing test before release.
- No critical accessibility violations on core citizen screens.
- Performance thresholds are met in the staging load test.
- Security scans and required penetration testing have no open Critical/High findings.

## 8. Automation Strategy
Recommended tools: Jest + React Testing Library for unit/component tests; Supertest/Postman/Newman for API/integration tests; Playwright or Cypress for E2E; k6 or JMeter for performance; CI-integrated SAST/dependency scanning; axe-core/WAVE plus NVDA/VoiceOver for accessibility.

The current static prototype is not represented as having executed these future automation suites.
