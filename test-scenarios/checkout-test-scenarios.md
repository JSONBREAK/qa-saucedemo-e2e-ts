# Checkout Test Scenarios

**As a customer**

I want to complete checkout

So that I can place an order

**Acceptance Criteria**
- User can proceed to checkout from cart page
- User must fill required information (First Name, Last Name, Postal Code)
- System validates required fields
- User can continue to order overview page
- User can finish checkout
- Order confirmation page displays success message and order details

---

### Acceptance Criteria → Test Scenarios

**Checkout Navigation Scenarios**
1. Verify user can navigate to checkout page from cart page.
2. Verify user can navigate to order overview page after filling required information on checkout page.


**Checkout Validation Scenarios**
3. Verify system displays validation message when required fields are empty on checkout page.
4. Verify user cannot proceed to order overview page if required fields are not filled on checkout page.

**Checkout Overview Scenarios**
5. Verify order overview page displays correct order details (items, quantity, price, and total amount).
6. Verify user can finish checkout from order overview page.
7. Verify order confirmation page displays success message and correct order details after finishing checkout.


**Checkout Completion Scenarios**
8. Verify user is redirected to inventory page after completing checkout and clicking "Back Home" button on order confirmation page.

    > Requirement > Checkout Navigation Scenarios > Checkout Validation Scenarios > Checkout Overview Scenarios > Checkout Completion Scenarios

---

## 📑 Test Scenarios Table

| Scenario ID | Scenario Description                                    |
| ----------- | ------------------------------------------------------- |
| TS-CHECKOUT-001    | Verify user can navigate to checkout page from cart page |
| TS-CHECKOUT-002    | Verify user can navigate to order overview page after filling required information on checkout page |
| TS-CHECKOUT-003    | Verify system displays validation message when all required fields are empty on checkout page |
| TS-CHECKOUT-004    | Verify system displays validation message when First Name is missing on checkout page |
| TS-CHECKOUT-005    | Verify system displays validation message when Last Name is missing on checkout page |
| TS-CHECKOUT-006    | Verify system displays validation message when Postal Code is missing on checkout page |
| TS-CHECKOUT-007    | Verify user cannot proceed to order overview page if required fields are not filled on checkout page |
| TS-CHECKOUT-008    | Verify order overview page displays correct order details (items, quantity, price, and total amount) |
| TS-CHECKOUT-009    | Verify user can finish checkout from order overview page |
| TS-CHECKOUT-010    | Verify order confirmation page displays success message and correct order details after finishing checkout |
| TS-CHECKOUT-011    | Verify user is redirected to inventory page after completing checkout and clicking "Back Home" button on order confirmation page |

---

## Test Steps Template

| Test Scenario ID | Description | Steps | Expected Result | Status |
|------------------|-------------|-------|-----------------|--------|
| TS-CHECKOUT-001    | Verify user can navigate to checkout page from cart page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button | User is navigated to Checkout Information page and URL contains /checkout-step-one. | Pass/Fail |
| TS-CHECKOUT-002    | Verify user can navigate to order overview page after filling required information on checkout page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Fill in required fields (First Name, Last Name, Postal Code) 6. Click "Continue" button | User is navigated to Order Overview page and URL contains /checkout-step-two. | Pass/Fail |
| TS-CHECKOUT-003    | Verify system displays validation message when all required fields are empty on checkout page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Leave all required fields empty 6. Click "Continue" button | A validation message is displayed indicating that all required fields must be filled. | Pass/Fail |
| TS-CHECKOUT-004    | Verify system displays validation message when First Name is missing on checkout page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Leave First Name empty, fill other fields 6. Click "Continue" button | A validation message is displayed indicating that First Name is required. | Pass/Fail |
| TS-CHECKOUT-005    | Verify system displays validation message when Last Name is missing on checkout page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Leave Last Name empty, fill other fields 6. Click "Continue" button | A validation message is displayed indicating that Last Name is required. | Pass/Fail |
| TS-CHECKOUT-006    | Verify system displays validation message when Postal Code is missing on checkout page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Leave Postal Code empty, fill other fields 6. Click "Continue" button | A validation message is displayed indicating that Postal Code is required. | Pass/Fail |
| TS-CHECKOUT-007    | Verify user cannot proceed to order overview page if required fields are not filled on checkout page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Leave any required field empty 6. Click "Continue" button | User remains on Checkout Information page and cannot proceed to Order Overview page. | Pass/Fail |
| TS-CHECKOUT-008    | Verify order overview page displays correct order details (items, quantity, price, and total amount) | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Fill in required fields (First Name, Last Name, Postal Code) 6. Click "Continue" button | Order Overview page displays correct order details including items, quantity, price, and total amount. | Pass/Fail |
| TS-CHECKOUT-009    | Verify user can finish checkout from order overview page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Fill in required fields (First Name, Last Name, Postal Code) 6. Click "Continue" button 7. Click "Finish" button | User is able to finish checkout and is navigated to Order Confirmation page and URL contains /checkout-complete. | Pass/Fail |
| TS-CHECKOUT-010    | Verify order confirmation page displays success message and correct order details after finishing checkout | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Fill in required fields (First Name, Last Name, Postal Code) 6. Click "Continue" button 7. Click "Finish" button | Order Confirmation page displays a success message and correct order details including items, quantity, price, and total amount. | Pass/Fail |
| TS-CHECKOUT-011    | Verify user is redirected to inventory page after completing checkout and clicking "Back Home" button on order confirmation page | 1. Log in with valid credentials 2. Add product to cart 3. Navigate to cart page 4. Click "Checkout" button 5. Fill in required fields (First Name, Last Name, Postal Code) 6. Click "Continue" button 7. Click "Finish" button 8. Click "Back Home" button on order confirmation page | User is redirected to Inventory page and URL contains /inventory after clicking "Back Home" button on Order Confirmation page. | Pass/Fail |

