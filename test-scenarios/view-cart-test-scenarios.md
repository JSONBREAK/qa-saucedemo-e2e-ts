
# View Cart Test Scenarios

## User Story

**As a logged-in user**

I want to view and manage items in my cart 

So that I can review my selected products

**Acceptance Criteria**
- Cart page displays selected products
- User can remove items from cart
- Cart badge updates accordingly

---

### Acceptance Criteria → Test Scenarios

**Cart Display Scenarios**
1. Verify cart page displays all products added to cart with correct details (name, price, and quantity).
2. Verify cart badge count reflects the number of items in the cart when navigating to the cart page.

**Cart Management Scenarios**
3. Verify user can remove a product from the cart page and the cart badge count updates accordingly.
4. Verify cart page displays an empty state message when all items are removed from the cart and the cart badge is no longer displayed.

> Requirement > Cart Display Scenarios > Cart Management Scenarios

---

## 📑 Test Scenarios Table  

| Scenario ID | Scenario Description                                    |
| ----------- | ------------------------------------------------------- |
| TS-VIEWCART-001    | Verify cart page displays all products added to cart with correct details (name, price, and quantity) |
| TS-VIEWCART-002    | Verify cart badge count reflects the number of items in the cart when navigating to the cart page |
| TS-VIEWCART-003    | Verify user can remove a product from the cart page and the cart badge count updates accordingly |
| TS-VIEWCART-004    | Verify cart page displays an empty state message when all items are removed from the cart and the cart badge is no longer displayed |

---

## Test Steps Template
| Test Scenario ID | Description | Steps | Expected Result | Status |
|------------------|-------------|-------|-----------------|--------|
| TS-VIEWCART-001    | Verify cart page displays all products added to cart with correct details (name, price, and quantity) | 1. Log in with valid credentials 2. Add multiple products to cart 3. Navigate to cart page | Cart page displays all added products with correct name, price, and quantity details. | Pass/Fail |
| TS-VIEWCART-002    | Verify cart badge count reflects the number of items in the cart when navigating to the cart page | 1. Log in with valid credentials 2. Add multiple products to cart 3. Navigate to cart page | Cart badge count reflects the total number of items currently in the cart. | Pass/Fail |
| TS-VIEWCART-003    | Verify user can remove a product from the cart page and the cart badge count updates accordingly | 1. Log in with valid credentials 2. Add multiple products to cart 3. Navigate to cart page 4. Remove a product from the cart page | Product is removed from cart and cart badge count decreases by 1. | Pass/Fail |
| TS-VIEWCART-004    | Verify cart page displays an empty state message when all items are removed from the cart and the cart badge is no longer displayed | 1. Log in with valid credentials 2. Add multiple products to cart 3. Navigate to cart page 4. Remove all products from the cart page | Cart page displays an empty state message and cart badge is no longer displayed. | Pass/Fail |


