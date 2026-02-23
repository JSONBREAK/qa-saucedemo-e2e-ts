
# 🚀 SauceDemo QA Testing Project

Structured Manual QA project conducted on the SauceDemo web application.

This repository demonstrates a practical application of the Software Testing Life Cycle (STLC), including requirement analysis, test scenario design, validation testing, and traceability mapping.

The goal of this project is to showcase structured thinking, functional testing skills, and traceability practices expected from a Junior QA Engineer.

---

## Project Overview

- **Application:** SauceDemo (E-commerce Demo Application)
- **Testing Type:** Manual Functional Testing
- **Target Website:** https://www.saucedemo.com/

**Scope:**
- Login
- Logout
- Add to Cart
- View Cart
- Checkout (Step One, Overview, Completion)

**Out of Scope:**
- API Testing
- Performance Testing
- Security Testing
- Database Validation

---



## Objectives

- Apply STLC concepts to a real demo web application
- Design structured test scenarios based on acceptance criteria
- Perform positive and negative testing
- Ensure full business flow validation
- Maintain requirement-to-test traceability using RTM

---


## Features Covered

**Authentication**
- Valid login
- Invalid credentials handling
- Locked user validation
- Session persistence
- Logout and session termination

**Cart Management**
- Add to cart
- Remove from cart
- Cart badge updates
- Empty cart behavior

**Checkout Process**
- Navigation to checkout
- Required field validation
- Overview page verification
- Order completion
- Post-completion redirection


---


## Repository Structure


```text
qa-saucedemo-test-design/
│   README.md
│   rtm.md
│   saucedemo-user-stories.md
│   defect-log.md
│   defect-report.md
│
└───test-scenarios
    add-to-cart-test-scenarios.md
    checkout-test-scenarios.md
    login-test-scenarios.md
    logout-test-scenarios.md
    view-cart-test-scenarios.md
```


**Key Files:**
- saucedemo-user-stories.md: Structured user stories and acceptance criteria
- test-scenarios/: Functional test scenarios organized by feature module
- rtm.md: Requirement Traceability Matrix mapping requirements to test scenarios
- defect-log.md: Ongoing log of defects found during testing
- defect-report.md: Summarized defect report for management or stakeholders

---

## Defect Tracking

Defects found during testing are tracked in two files:

- **defect-log.md:** A detailed log of all defects found, including status, severity, and feature area.
- **defect-report.md:** A summarized report of key or unresolved defects for management review.

This ensures transparency and traceability of issues throughout the QA process.

---


## Testing Approach

This project follows a structured workflow:

Requirement
→ Acceptance Criteria
→ Test Scenarios
→ Test Cases
→ Validation
→ Traceability (RTM)

Both happy path and negative scenarios are covered to ensure proper validation and navigation control.

---



## Validation Strategy

- Required field validation
- Navigation control verification
- URL verification for page transitions
- Error message verification
- Session handling validation

---



## Skills Demonstrated

- Requirement analysis
- Test scenario design
- Negative testing
- Functional flow validation
- Traceability mapping
- Clear and structured documentation


---



## Author

QA Engineer (Entry-Level) focused on structured testing practices, clear documentation, and continuous learning.

---

> **Note:** This project is created for learning and portfolio purposes. It demonstrates manual QA methodology applied to a publicly available demo web application.