# Add to Cart Test Scenarios

**As a logged-in user**
I want to manage products in my cart
So that I can review items before checkout

**Acceptance Criteria**

- Clicking “Add to Cart” adds item to cart
- Cart badge count increases
- Button changes to “Remove”

---

### Acceptance Criteria → AC Analysis 

```
- User can add product to cart → Clicking “Add to Cart” from `/inventory` page adds item to cart and updates badge count
- Cart badge count updates → Cart badge count increases by 1 for each item added to cart
- “Add to Cart” button changes to “Remove” → After adding item to cart, button text changes to “Remove”
- User can remove product from cart → Clicking “Remove” from `/inventory` page removes item from cart and updates badge count
- Cart badge count updates on removal → Cart badge count decreases by 1 for each item removed from cart
- “Remove” button changes back to “Add to Cart” → After removing item from cart, button text changes back to “Add to Cart”
- Cart updates accordingly on inventory page → Cart badge count and button states reflect current cart contents when navigating back to inventory page
- Cart page displays added items → Items added to cart appear in the cart page with correct details
```

---

### Acceptance Criteria → Test Scenarios

**Add to Cart Functionality** 

1. Verify user can add a single product to cart and cart badge count updates accordingly.
2. Verify "Add to Cart" button changes to "Remove" after adding a product to cart.

**Remove from Cart Functionality**

3. Verify user can remove a single product from cart and cart badge count updates accordingly.
4. Verify "Remove" button changes back to "Add to Cart" after removing a product from cart.

**Cart Page Scenarios**

5. Verify added product appears in the cart page with correct details (name, price, and quantity).
6. Verify user can remove product from cart page and cart badge count updates accordingly.
7. Verify cart is empty after removing all products and cart badge is no longer displayed.

 > Requirement > Add to Cart Functionality > Remove from Cart Functionality > Cart Page Scenarios


### 📑 Test Scenarios Table

| Scenario ID | Scenario Description                                    |
| ----------- | ------------------------------------------------------- |
| TS-CART-001    | Verify user can add a single product to cart and cart badge count updates accordingly |
| TS-CART-002    | Verify "Add to Cart" button changes to "Remove" after adding a product to cart |
| TS-CART-003    | Verify user can remove a single product from cart and cart badge count updates accordingly |
| TS-CART-004    | Verify "Remove" button changes back to "Add to Cart" after removing a product from cart |
| TS-CART-005    | Verify added product appears in the cart page with correct details (name, price, and quantity) |
| TS-CART-006    | Verify user can remove product from cart page and cart badge count updates accordingly |
| TS-CART-007    | Verify cart is empty after removing all products and cart badge is no longer displayed |

---

## Test Steps Template

| Test Scenario ID | Description | Steps | Expected Result | Status |
|------------------|-------------|-------|-----------------|--------|
| TS-CART-001    | Verify user can add a single product to cart and cart badge count updates accordingly | 1. Log in with valid credentials 2. Navigate to inventory page 3. Click "Add to Cart" button for a product | Product is added to cart and cart badge count increases by 1. | Pass/Fail |
| TS-CART-002    | Verify "Add to Cart" button changes to "Remove" after adding a product to cart | 1. Log in with valid credentials 2. Navigate to inventory page 3. Click "Add to Cart" button for a product | Button text changes from "Add to Cart" to "Remove". | Pass/Fail |
| TS-CART-003    | Verify user can remove a single product from cart and cart badge count updates accordingly | 1. Log in with valid credentials 2. Navigate to inventory page 3. Click "Add to Cart" button for a product 4. Click "Remove" button for the same product | Product is removed from cart and cart badge count decreases by 1. | Pass/Fail |
| TS-CART-004    | Verify "Remove" button changes back to "Add to Cart" after removing a product from cart | 1. Log in with valid credentials 2. Navigate to inventory page 3. Click "Add to Cart" button for a product 4. Click "Remove" button for the same product | Button text changes from "Remove" back to "Add to Cart". | Pass/Fail |
| TS-CART-005    | Verify added product appears in the cart page with correct details (name, price, and quantity) | 1. Log in with valid credentials 2. Navigate to inventory page 3. Click "Add to Cart" button for a product 4. Click on cart icon to navigate to cart page | Added product appears in cart page with correct name, price, and quantity. | Pass/Fail |
| TS-CART-006    | Verify user can remove product from cart page and cart badge count updates accordingly | 1. Log in with valid credentials 2. Navigate to inventory page 3. Click "Add to Cart" button for a product 4. Click on cart icon to navigate to cart page 5. Click "Remove" button for the product in cart page | Product is removed from cart and cart badge count decreases by 1. | Pass/Fail |
| TS-CART-007    | Verify cart is empty after removing all products and cart badge is no longer displayed | 1. Log in with valid credentials 2. Navigate to inventory page 3. Click "Add to Cart" button for multiple products 4. Click on cart icon to navigate to cart page 5. Click "Remove" button for all products in cart page | Cart is empty and cart badge is no longer displayed. | Pass/Fail |