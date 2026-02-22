# Logout Test Scenarios

**As a logged-in user**
I want to log out
So that my session is securely terminated

**Acceptance Criteria**
- Clicking logout redirects to login page
- User cannot access inventory page after logout

---

### Acceptance Criteria → Test Scenarios 

**Positive Scenarios**
1. Verify user can successfully log out and is redirected to login page.


**Negative Scenarios(Session Termination Scenarios)**

2. Verify user session is terminated after logout.
3. Verify user cannot access inventory page after logout using browser back button.
4. Verify user cannot access inventory page after logout by directly entering URL.
5. Verify user cannot access inventory page after logout by refreshing the page.

 > Requirement > Positive Scenarios > Negative Scenarios

 ---

## 📑 Test Scenarios Table

| Scenario ID | Scenario Description                                    |
| ----------- | ------------------------------------------------------- |
| TS-LOGOUT-001    | Verify successful logout and redirection to login page |
| TS-LOGOUT-002    | Verify user session is terminated after logout |
| TS-LOGOUT-003    | Verify user cannot access inventory page after logout using browser back button |
| TS-LOGOUT-004    | Verify user cannot access inventory page after logout by directly entering URL |
| TS-LOGOUT-005    | Verify user cannot access inventory page after logout by refreshing the page |

---

## Test Steps Template

| Test Scenario ID | Description | Steps | Expected Result | Status |
|------------------|-------------|-------|-----------------|--------|
| TS-LOGOUT-001    | Verify successful logout and redirection to login page | 1. Log in with valid credentials 2. Click logout button | User is redirected to the login page and login form is displayed. | Pass/Fail |
| TS-LOGOUT-002    | Verify user session is terminated after logout | 1. Log in with valid credentials 2. Click logout button 3. Attempt to access inventory page | Login page is displayed and user session is not restored. | Pass/Fail |
| TS-LOGOUT-003    | Verify user cannot access inventory page after logout using browser back button | 1. Log in with valid credentials 2. Click logout button 3. Click browser back button | User is redirected to the login page when the browser back button is clicked after logout. | Pass/Fail |
| TS-LOGOUT-004    | Verify user cannot access inventory page after logout by directly entering URL | 1. Log in with valid credentials 2. Click logout button 3. Enter inventory page URL directly | User is redirected to the login page when inventory URL is entered directly after logout. | Pass/Fail |
| TS-LOGOUT-005    | Verify user cannot access inventory page after logout by refreshing the page | 1. Log in with valid credentials 2. Click logout button 3. Refresh the page | Login page remains displayed and user session is not restored after page refresh. | Pass/Fail |
