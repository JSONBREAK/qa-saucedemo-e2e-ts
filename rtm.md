# Requirement Traceability Matrix (RTM)

| Requirement ID | Requirement Description | Test Scenario ID(s) | Test Scenario Description | Coverage Notes |
| -------------- | ---------------------- | ------------------- | ------------------------ | ------------- |
| REQ-LOGIN-01   | Valid credentials redirect to inventory page | TS-LOGIN-01 | Verify successful login with valid credentials and redirection to inventory page | Direct coverage |
| REQ-LOGIN-02   | Invalid credentials show error message | TS-LOGIN-02, TS-LOGIN-03, TS-LOGIN-04, TS-LOGIN-09, TS-LOGIN-10 | Error message for invalid credentials, case sensitivity, leading/trailing spaces | Covers all invalid input cases |
| REQ-LOGIN-03   | Empty fields show validation message | TS-LOGIN-06, TS-LOGIN-07, TS-LOGIN-08 | Validation for empty username/password/both | All empty field cases |
| REQ-LOGIN-04   | Locked user cannot log in | TS-LOGIN-05 | Locked user error message | Direct coverage |
| REQ-LOGIN-05   | User remains logged in until logout | TS-LOGIN-11 | Session persists after refresh | Direct coverage |
| REQ-LOGOUT-01  | Clicking logout redirects to login page | TS-LOGOUT-001 | Logout redirects to login page | Direct coverage |
| REQ-LOGOUT-02  | User cannot access inventory page after logout | TS-LOGOUT-002, TS-LOGOUT-003, TS-LOGOUT-004, TS-LOGOUT-005 | Session termination, back button, direct URL, refresh | Covers all access attempts post-logout |
| REQ-CHECKOUT-01| User can proceed to checkout from cart page | TS-CHECKOUT-001 | Navigate to checkout page | Direct coverage, URL check |
| REQ-CHECKOUT-02| User must fill required information | TS-CHECKOUT-003, TS-CHECKOUT-004, TS-CHECKOUT-005, TS-CHECKOUT-006, TS-CHECKOUT-007 | Validation for missing fields | Covers all missing field cases |
| REQ-CHECKOUT-03| System validates required fields | TS-CHECKOUT-003–TS-CHECKOUT-007 | Validation messages and prevention of navigation | Complete coverage |
| REQ-CHECKOUT-04| User can continue to order overview page | TS-CHECKOUT-002 | Navigation after valid input | URL check |
| REQ-CHECKOUT-05| User can finish checkout | TS-CHECKOUT-009 | Finish checkout, navigate to confirmation | URL check |
| REQ-CHECKOUT-06| Order confirmation page displays success message and order details | TS-CHECKOUT-010 | Confirmation page, success message, order details | Direct coverage |
| REQ-CHECKOUT-07| User is redirected to inventory page after completing checkout | TS-CHECKOUT-011 | Back Home button redirects to inventory | URL check |
