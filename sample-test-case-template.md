# Test Case Template — Sample

> Fictional example demonstrating test case documentation structure.

**Feature:** User Login
**Module:** Authentication
**Test Environment:** Web (Chrome, Firefox, Safari), Mobile (iOS, Android)

---

| Field | Details |
|---|---|
| **Test Case ID** | TC-LOGIN-001 |
| **Title** | Verify successful login with valid credentials |
| **Preconditions** | User has an existing verified account |
| **Priority** | High |
| **Type** | Functional |

### Test Steps
1. Navigate to login page
2. Enter valid email address
3. Enter correct password
4. Click "Log In"

### Expected Result
User is redirected to the dashboard/home screen. Session is created. Welcome/greeting element displays the correct username.

### Actual Result
*(filled in during execution)*

### Status
*(Pass / Fail / Blocked)*

---

## Additional Sample Cases (same feature)

| Test Case ID | Title | Priority | Type |
|---|---|---|---|
| TC-LOGIN-002 | Verify error message on incorrect password | High | Negative |
| TC-LOGIN-003 | Verify "Forgot Password" link navigates correctly | Medium | Functional |
| TC-LOGIN-004 | Verify field validation on empty email/password | Medium | Negative |
| TC-LOGIN-005 | Verify login persists after app restart (Remember Me checked) | Low | Functional |
| TC-LOGIN-006 | Verify account lockout after 5 failed attempts | High | Security |

---

*Structure: each case includes ID, title, preconditions, priority, type, numbered steps, and expected result — kept consistent across a full test suite so cases can be batch-executed and tracked easily in tools like TestRail or Jira.*
