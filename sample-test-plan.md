# Test Plan — Sample

> Fictional example demonstrating test planning structure at a project/feature level.

**Project:** Mobile Banking App - Fund Transfer Feature
**Version:** v2.4.0
**Prepared By:** Sample QA Tester
**Date:** Sample Date

---

## 1. Objective
Verify that the Fund Transfer feature works correctly, securely, and consistently across supported platforms before the v2.4.0 release, covering functional accuracy, error handling, and edge cases.

## 2. Scope

**In Scope:**
- Internal transfers (between user's own accounts)
- External transfers (to other bank accounts)
- Transfer confirmation & receipt generation
- Input validation (amount limits, insufficient funds, invalid recipient)

**Out of Scope:**
- Third-party payment gateway internals (covered by vendor's own QA)
- Push notification delivery timing (tracked separately under Notifications test plan)

## 3. Test Environment
- **Platforms:** iOS 17+, Android 13+, Web (Chrome, Safari)
- **Test Accounts:** 3 sandbox accounts with varying balance tiers
- **Tools:** TestRail (case management), Jira (bug tracking), Postman (API-level checks), BrowserStack (device coverage)

## 4. Test Approach
- **Functional testing** - core transfer flows, confirmation screens, receipts
- **Negative testing** - invalid amounts, insufficient balance, expired session mid-transfer
- **Boundary testing** - minimum/maximum transfer limits
- **Cross-platform testing** - consistency of flow and copy across iOS/Android/Web
- **Regression testing** - ensure existing account/balance features remain unaffected

## 5. Entry Criteria
- Feature build deployed to QA environment
- Test cases written and reviewed
- Sandbox test accounts provisioned with required balance states

## 6. Exit Criteria
- 100% of high-priority test cases executed
- No open Critical or High severity bugs
- Medium/Low severity bugs logged and triaged with dev team sign-off

## 7. Risks & Assumptions
- **Risk:** Sandbox environment may not fully replicate production bank integration behavior — flagged for smoke retest post-deployment.
- **Assumption:** Payment gateway sandbox is stable and available throughout the test cycle.

## 8. Deliverables
- Executed test case results (TestRail)
- Bug reports for identified issues (Jira)
- End-of-cycle summary report (pass rate, blockers, recommendations)

---

*This plan defines scope, approach, environment, and exit criteria before test execution begins — keeping the testing effort aligned with release goals and making handoff between QA and dev teams straightforward.*
