# Defect Report




This document contains detailed reports of defects found during testing of the SauceDemo application. Each defect is described with its summary, related test case, environment details, steps to reproduce, expected and actual results, severity, priority, and current status.

---


## 🐞 Defect: DEF-001 — Login

```
Summary: Error message is not displayed when user enters incorrect password.
Defect Type: Functional

Related Test Case: TC-LOGIN-002

Environment:
- Application: SauceDemo
- Browser: Chrome 120+
- OS: Windows 11
- Date Found: 2026-02-23

Preconditions:
User is on the login page.

Steps to Reproduce:
1. Enter valid username.
2. Enter incorrect password.
3. Click the "Login" button.

Expected Result:
System should display an error message indicating invalid credentials.

Actual Result:
User remains on login page without any error message displayed.

Severity: High

Priority: High

Status: Open

**Notes:**
This defect is created for demonstration purposes in QA portfolio.
```

---


## 🐞 Defect: DEF-002 — Add to Cart

```
Summary: Cart badge does not update after removing product from cart page.
Defect Type: UI / Functional

Related Test Case: TC-CART-006

Environment:
- Application: SauceDemo
- Browser: Chrome 120+
- OS: Windows 11
- Date Found: 2026-02-23

Preconditions:
User is logged in and has at least one product in the cart.

Steps to Reproduce:
1. Go to cart page.
2. Remove a product from the cart.

Expected Result:
Cart badge should decrease by 1 or disappear if no items remain.

Actual Result:
Cart badge count does not update after removing product.

Severity: Medium

Priority: Medium

Status: Open

**Notes:**
Observed only on Chrome. On Firefox, badge updates correctly.
```

---


## 🐞 Defect: DEF-003 — Checkout

```
Summary: System allows checkout with empty Postal Code field.
Defect Type: Validation

Related Test Case: TC-CHECKOUT-006

Environment:
- Application: SauceDemo
- Browser: Chrome 120+
- OS: Windows 11
- Date Found: 2026-02-23

Preconditions:
User is logged in and has at least one product in the cart.

Steps to Reproduce:
1. Go to cart page and click Checkout.
2. Leave Postal Code field empty, fill other required fields.
3. Click Continue.

Expected Result:
System should display a validation message for missing Postal Code and not allow to proceed.

Actual Result:
User can proceed to order overview page without entering Postal Code.

Severity: High

Priority: High

Status: Open

**Notes:**
Occurs on both Chrome and Firefox.
```
```

---


## 🐞 Defect: DEF-004 — Logout

```
Summary: User can access inventory page after logout by using browser back button.
Defect Type: Security

Related Test Case: TC-LOGOUT-003

Environment:
- Application: SauceDemo
- Browser: Chrome 120+
- OS: Windows 11
- Date Found: 2026-02-23

Preconditions:
User is logged in and on the inventory page.

Steps to Reproduce:
1. Click logout button.
2. Click browser back button.

Expected Result:
User should be redirected to login page and not able to access inventory page.

Actual Result:
User is able to view inventory page after logout by using browser back button.

Severity: Critical

Priority: High

Status: Open

**Notes:**
Security issue. User session not properly terminated.
```

---
