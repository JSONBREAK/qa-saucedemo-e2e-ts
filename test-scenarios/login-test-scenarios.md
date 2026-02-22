# Login Test Scenarios

### Login

**As a registered user**
I want to log in
So that I can access the product inventory

**Acceptance Criteria**
- Valid credentials redirect to inventory page 
- Invalid credentials show error message 
- Empty fields show validation message
- Locked user cannot log in
- User remains logged in until logout

---

### Acceptance Criteria → Test Scenarios 

From Acceptance Criteria:
- Successful Login → Navigate to inventory page
- Invalid credential handling → Error message display
- Field validation → Validation message display for empty fields
- Locked user handling → Cannot log in
- User session handling → Remains logged in until logout



## Login - Test Scenarios

**Positive Scenarios**
1. Verify successful login with valid credentials and redirection to inventory page.


**Negative Scenarios**

2. Verify login with invalid username 
3. Verify login with invalid password
4. Verify login with both username and password invalid
5. Verify login with locked user


## Validation Scenarios
6. Verify login with empty username and password fields
7. Verify login with empty username field
8. Verify login with empty password field
9. Verify login with case-sensitive username
10. Verify login with leading/trailing spaces in username

## Session Scenarios
11. Verify user remains logged in after page refresh
12. Verify user is redirected to login page after logout
13. Verify user cannot access inventory page after logout using browser back button

 > Requirement > Positive/Negative Scenarios > Validation Scenarios > Session Scenarios

---

## 📑 Test Scenarios Table

| Scenario ID | Scenario Description                                    |
| ----------- | ------------------------------------------------------- |
| TS-LOGIN-01 | Verify successful login with valid credentials and redirection to inventory page            |
| TS-LOGIN-02 | Verify system displays error message when password is incorrect |
| TS-LOGIN-03 | Verify system displays error message when username is incorrect |
| TS-LOGIN-04 | Verify system displays error message when both username and password are incorrect |
| TS-LOGIN-05 | Verify system prevents login for locked user            |
| TS-LOGIN-06 | Verify system requires username when password field is empty |
| TS-LOGIN-07 | Verify system requires password when username field is empty |
| TS-LOGIN-08 | Verify login is case-sensitive                          |
| TS-LOGIN-09 | Verify system behavior when username contains leading or trailing spaces |
| TS-LOGIN-10 | Verify system behavior when entering excessively long input in username field |
| TS-LOGIN-11 | Verify user remains logged in after page refresh         |
| TS-LOGIN-12 | Verify user is redirected to login page after logout     |
| TS-LOGIN-13 | Verify user cannot access inventory page after logout using browser back button |

---





