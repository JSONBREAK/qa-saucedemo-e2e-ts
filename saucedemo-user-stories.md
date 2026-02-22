# SauceDemo QA – User Stories & Requirements

---

## User Stories

---

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

### Logout

**As a logged-in user**
I want to log out
So that my session is securely terminated

**Acceptance Criteria**
- Clicking logout redirects to login page
- User cannot access inventory page after logout

---

### Add to Cart

**As a logged-in user**
I want to add products to my cart
So that I can purchase them later

**Acceptance Criteria**
- Clicking "Add to Cart" increases cart badge count
- Item appears in cart page

---

### View Cart

**As a logged-in user**
I want to view and manage items in my cart
So that I can review my selected products

**Acceptance Criteria**
- Cart page displays selected products
- User can remove items from cart
- Cart badge updates accordingly

---

### Checkout

**As a customer**
I want to complete checkout
So that I can place an order

**Acceptance Criteria**
- Required fields must be filled
- Missing fields show validation message
- Order summary displays selected items and total amount
- Order confirmation page appears after successful checkout
- User can cancel checkout and return to product page
