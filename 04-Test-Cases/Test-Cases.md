# 🧪 Test Cases

## 1. Purpose

Detailed manual test cases for the e-commerce application covering critical business workflows.

## 2. Test Case Format

| Field | Description |
|---|---|
| Test Case ID | Unique identifier |
| Requirement ID | Related requirement |
| Module | Application area |
| Scenario | What is being validated |
| Preconditions | Required setup |
| Test Data | Input data |
| Steps | Execution steps |
| Expected Result | Expected behavior |
| Priority | Business priority |
| Type | Functional/Negative/Boundary |

## 3. Sample Test Cases

| ID | Requirement | Module | Scenario | Expected Result | Priority | Type |
|---|---|---|---|---|---|---|
| TC-LOGIN-001 | REQ-LOGIN-001 | Login | Login with valid credentials | User is authenticated and redirected to the home page | High | Functional |
| TC-LOGIN-002 | REQ-LOGIN-001 | Login | Login with invalid password | Appropriate validation message is displayed | High | Negative |
| TC-LOGIN-003 | REQ-LOGIN-001 | Login | Submit empty credentials | Mandatory field validation is displayed | High | Negative |
| TC-SEARCH-001 | REQ-SEARCH-001 | Search | Search using valid product name | Relevant products are displayed | High | Functional |
| TC-SEARCH-002 | REQ-SEARCH-001 | Search | Search using unavailable product | No-result message is displayed | Medium | Negative |
| TC-CART-001 | REQ-CART-001 | Cart | Add product to cart | Product and correct quantity are added | High | Functional |
| TC-CART-002 | REQ-CART-001 | Cart | Update product quantity | Cart total is recalculated correctly | High | Functional |
| TC-CART-003 | REQ-CART-001 | Cart | Remove product | Product is removed and totals are updated | High | Functional |
| TC-CHECKOUT-001 | REQ-CHECKOUT-001 | Checkout | Complete checkout with valid address | User can proceed to payment | Critical | E2E |
| TC-PAY-001 | REQ-PAY-001 | Payment | Successful payment | Order is created and confirmation is displayed | Critical | Integration |
| TC-PAY-002 | REQ-PAY-001 | Payment | Failed payment | Payment failure is shown and order is not duplicated | Critical | Negative |
| TC-ORDER-001 | REQ-ORDER-001 | Orders | Verify order history after successful order | Latest order is displayed with correct details | High | Functional |
| TC-LOGOUT-001 | REQ-LOGIN-001 | Logout | Logout from authenticated session | Session is terminated and user returns to login | High | Security/Functional |

## 4. Detailed Example – Checkout

### TC-CHECKOUT-001 – Successful Checkout

**Precondition:** Registered user is logged in and has an item in the cart.

**Steps:**
1. Open Cart.
2. Verify product, quantity and price.
3. Select or add a valid delivery address.
4. Continue to checkout.
5. Verify order summary.
6. Select a supported payment method.
7. Complete payment.

**Expected Result:**
- Order is successfully created.
- Order ID is generated.
- Confirmation is displayed.
- Cart is cleared or updated according to business rules.
- Order appears in Order History.

## 5. Defect Evidence

For failed cases, attach screenshots, request/response evidence for API-related failures, relevant application logs, timestamps and other reproducible evidence to the defect record.

> All examples in this repository are synthetic and contain no production or customer data.
