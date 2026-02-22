# Login Test Scenarios



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
| TS-LOGIN-06 | Verify system requires username and password when both fields are empty |
| TS-LOGIN-07 | Verify system requires username when password field is empty |
| TS-LOGIN-08 | Verify system requires password when username field is empty |
| TS-LOGIN-09 | Verify login is case-sensitive                          |
| TS-LOGIN-10 | Verify system behavior when username contains leading or trailing spaces |
| TS-LOGIN-11 | Verify user remains logged in after page refresh         |

---

## Test Steps Template

| Test Scenario ID | Description | Steps | Expected Result | Status |
|------------------|-------------|-------|-----------------|--------|
| TS-LOGIN-01 | Verify successful login with valid credentials and redirection to inventory page | 1. Navigate to login page 2. Enter valid username and password 3. Click login button | User is redirected to the inventory page and product listings are displayed. | Pass/Fail |
| TS-LOGIN-02 | Verify system displays error message when password is incorrect | 1. Navigate to login page 2. Enter valid username and invalid password 3. Click login button | An error message is displayed indicating invalid credentials. | Pass/Fail |
| TS-LOGIN-03 | Verify system displays error message when username is incorrect | 1. Navigate to login page 2. Enter invalid username and valid password 3. Click login button | An error message is displayed indicating invalid credentials. | Pass/Fail |
| TS-LOGIN-04 | Verify system displays error message when both username and password are incorrect | 1. Navigate to login page 2. Enter invalid username and invalid password 3. Click login button | An error message is displayed indicating invalid credentials. | Pass/Fail |
| TS-LOGIN-05 | Verify system prevents login for locked user | 1. Navigate to login page 2. Enter locked user's username and password 3. Click login button | An error message is displayed indicating that the user account is locked and cannot log in. | Pass/Fail |
| TS-LOGIN-06 | Verify system requires username and password when both fields are empty | 1. Navigate to login page 2. Leave both username and password fields empty 3. Click login button | A validation message is displayed indicating that both fields are required. | Pass/Fail |
| TS-LOGIN-07 | Verify system requires username when password field is empty | 1. Navigate to login page 2. Leave username field empty and enter valid password 3. Click login button | A validation message is displayed indicating that the username field is required. | Pass/Fail |
| TS-LOGIN-08 | Verify system requires password when username field is empty | 1. Navigate to login page 2. Enter valid username and leave password field empty 3. Click login button | A validation message is displayed indicating that the password field is required. | Pass/Fail |
| TS-LOGIN-09 | Verify login is case-sensitive | 1. Navigate to login page 2. Enter valid username with different case and valid password 3. Click login button | An error message is displayed indicating invalid credentials. | Pass/Fail |
| TS-LOGIN-10 | Verify system behavior when username contains leading or trailing spaces | 1. Navigate to login page 2. Enter valid username with leading/trailing spaces and valid password 3. Click login button | An error message is displayed indicating invalid credentials. | Pass/Fail |
| TS-LOGIN-11 | Verify user remains logged in after page refresh | 1. Log in with valid credentials 2. Refresh the page | User remains logged in and is still on the inventory page after refreshing. | Pass/Fail |




