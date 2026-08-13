# Test Scenarios

## 1. Document Information

| Field | Details |
|---|---|
| Project | E-Commerce Web Application |
| Document | Test Scenarios |
| Version | 1.0 |
| Status | Baseline |
| Testing Type | Manual Testing |
| Prepared By | A P CHANDAN |
| Purpose | Define high-level test scenarios for validating the E-Commerce Web Application |

---

## 2. Scenario Identification

Test scenarios are high-level conditions or functionalities that need to be validated during testing.

The scenarios in this document are derived from the functional scope defined in the Test Plan and cover the major business workflows of the E-Commerce Web Application.

Each scenario will be converted into detailed test cases during test case preparation.

---

## 3. User Registration Scenarios

| ID | Test Scenario |
|---|---|
| TS-REG-001 | Verify that the user can access the registration page |
| TS-REG-002 | Verify registration with valid user details |
| TS-REG-003 | Verify registration with all mandatory fields blank |
| TS-REG-004 | Verify registration with First Name blank |
| TS-REG-005 | Verify registration with Last Name blank |
| TS-REG-006 | Verify registration with Email blank |
| TS-REG-007 | Verify registration with Password blank |
| TS-REG-008 | Verify registration with Confirm Password blank |
| TS-REG-009 | Verify registration with invalid email format |
| TS-REG-010 | Verify registration with invalid password |
| TS-REG-011 | Verify registration with mismatched passwords |
| TS-REG-012 | Verify registration using an already registered email |
| TS-REG-013 | Verify minimum password length validation |
| TS-REG-014 | Verify maximum password length validation |
| TS-REG-015 | Verify special characters in registration fields |
| TS-REG-016 | Verify spaces in registration fields |
| TS-REG-017 | Verify successful registration message |
| TS-REG-018 | Verify navigation after successful registration |

---

## 4. Login Scenarios

| ID | Test Scenario |
|---|---|
| TS-LOGIN-001 | Verify that the user can access the login page |
| TS-LOGIN-002 | Verify login with valid credentials |
| TS-LOGIN-003 | Verify login with invalid email |
| TS-LOGIN-004 | Verify login with incorrect password |
| TS-LOGIN-005 | Verify login with both email and password blank |
| TS-LOGIN-006 | Verify login with email blank |
| TS-LOGIN-007 | Verify login with password blank |
| TS-LOGIN-008 | Verify invalid email format validation |
| TS-LOGIN-009 | Verify password masking |
| TS-LOGIN-010 | Verify login error message |
| TS-LOGIN-011 | Verify successful login navigation |
| TS-LOGIN-012 | Verify login using registered user credentials |
| TS-LOGIN-013 | Verify login using unregistered user credentials |
| TS-LOGIN-014 | Verify login behavior after multiple invalid attempts |
| TS-LOGIN-015 | Verify Remember Me functionality where applicable |

---

## 5. Logout Scenarios

| ID | Test Scenario |
|---|---|
| TS-LOGOUT-001 | Verify logout option is available to authenticated users |
| TS-LOGOUT-002 | Verify successful logout |
| TS-LOGOUT-003 | Verify user is redirected to the appropriate page after logout |
| TS-LOGOUT-004 | Verify session is terminated after logout |
| TS-LOGOUT-005 | Verify protected page cannot be accessed after logout |
| TS-LOGOUT-006 | Verify browser back navigation after logout |
| TS-LOGOUT-007 | Verify refresh after logout |

---

## 6. Product Listing Scenarios

| ID | Test Scenario |
|---|---|
| TS-PROD-001 | Verify product listing page loads successfully |
| TS-PROD-002 | Verify products are displayed |
| TS-PROD-003 | Verify product names are displayed correctly |
| TS-PROD-004 | Verify product images are displayed correctly |
| TS-PROD-005 | Verify product prices are displayed correctly |
| TS-PROD-006 | Verify product descriptions are displayed correctly |
| TS-PROD-007 | Verify product availability information |
| TS-PROD-008 | Verify product count |
| TS-PROD-009 | Verify navigation from product listing to product details |
| TS-PROD-010 | Verify unavailable products are handled correctly |
| TS-PROD-011 | Verify product listing after login |
| TS-PROD-012 | Verify product listing consistency after page refresh |

---

## 7. Product Search Scenarios

| ID | Test Scenario |
|---|---|
| TS-SEARCH-001 | Verify search field is available |
| TS-SEARCH-002 | Search using a valid product name |
| TS-SEARCH-003 | Search using a partial product name |
| TS-SEARCH-004 | Search using uppercase characters |
| TS-SEARCH-005 | Search using lowercase characters |
| TS-SEARCH-006 | Search using mixed-case characters |
| TS-SEARCH-007 | Search using an invalid product name |
| TS-SEARCH-008 | Search with no matching products |
| TS-SEARCH-009 | Search with blank input |
| TS-SEARCH-010 | Search using special characters |
| TS-SEARCH-011 | Search using numeric values |
| TS-SEARCH-012 | Verify search result accuracy |
| TS-SEARCH-013 | Verify clearing search criteria |
| TS-SEARCH-014 | Verify search results after applying filters |
| TS-SEARCH-015 | Verify sorting of search results |

---

## 8. Product Filtering Scenarios

| ID | Test Scenario |
|---|---|
| TS-FILTER-001 | Verify category filter |
| TS-FILTER-002 | Verify price filter |
| TS-FILTER-003 | Verify minimum price boundary |
| TS-FILTER-004 | Verify maximum price boundary |
| TS-FILTER-005 | Verify multiple filters |
| TS-FILTER-006 | Verify filter result accuracy |
| TS-FILTER-007 | Verify applying a filter |
| TS-FILTER-008 | Verify removing a selected filter |
| TS-FILTER-009 | Verify Clear Filters functionality |
| TS-FILTER-010 | Verify filtering after product search |
| TS-FILTER-011 | Verify sorting after applying filters |
| TS-FILTER-012 | Verify filter behavior after page refresh |

---

## 9. Product Sorting Scenarios

| ID | Test Scenario |
|---|---|
| TS-SORT-001 | Verify sorting option is available |
| TS-SORT-002 | Sort products by price low to high |
| TS-SORT-003 | Sort products by price high to low |
| TS-SORT-004 | Sort products alphabetically A to Z |
| TS-SORT-005 | Sort products alphabetically Z to A |
| TS-SORT-006 | Verify sorting accuracy |
| TS-SORT-007 | Verify sorting after search |
| TS-SORT-008 | Verify sorting after filtering |
| TS-SORT-009 | Verify sorting after page refresh |
| TS-SORT-010 | Verify default sorting behavior |

---

## 10. Product Details Scenarios

| ID | Test Scenario |
|---|---|
| TS-DETAIL-001 | Verify product details page opens |
| TS-DETAIL-002 | Verify product name |
| TS-DETAIL-003 | Verify product image |
| TS-DETAIL-004 | Verify product price |
| TS-DETAIL-005 | Verify product description |
| TS-DETAIL-006 | Verify product availability |
| TS-DETAIL-007 | Verify product quantity selection |
| TS-DETAIL-008 | Verify Add to Cart button |
| TS-DETAIL-009 | Verify unavailable product behavior |
| TS-DETAIL-010 | Verify navigation back to product listing |
| TS-DETAIL-011 | Verify product information consistency with listing page |

---

## 11. Shopping Cart Scenarios

| ID | Test Scenario |
|---|---|
| TS-CART-001 | Verify shopping cart is accessible |
| TS-CART-002 | Add one product to cart |
| TS-CART-003 | Add multiple products to cart |
| TS-CART-004 | Add the same product multiple times |
| TS-CART-005 | Verify product name in cart |
| TS-CART-006 | Verify product price in cart |
| TS-CART-007 | Verify selected quantity |
| TS-CART-008 | Increase product quantity |
| TS-CART-009 | Decrease product quantity |
| TS-CART-010 | Remove a product from cart |
| TS-CART-011 | Remove all products from cart |
| TS-CART-012 | Verify empty cart behavior |
| TS-CART-013 | Verify subtotal calculation |
| TS-CART-014 | Verify tax calculation where applicable |
| TS-CART-015 | Verify final cart total |
| TS-CART-016 | Verify invalid quantity |
| TS-CART-017 | Verify zero quantity |
| TS-CART-018 | Verify negative quantity |
| TS-CART-019 | Verify maximum allowed quantity |
| TS-CART-020 | Verify cart after page refresh |
| TS-CART-021 | Verify cart persistence according to requirements |
| TS-CART-022 | Verify navigation from cart to product details |
| TS-CART-023 | Verify navigation from cart to checkout |

---

## 12. Checkout Scenarios

| ID | Test Scenario |
|---|---|
| TS-CHECKOUT-001 | Verify checkout page is accessible |
| TS-CHECKOUT-002 | Proceed to checkout with valid cart |
| TS-CHECKOUT-003 | Attempt checkout with empty cart |
| TS-CHECKOUT-004 | Verify customer information |
| TS-CHECKOUT-005 | Verify mandatory checkout fields |
| TS-CHECKOUT-006 | Verify invalid customer information |
| TS-CHECKOUT-007 | Verify delivery address fields |
| TS-CHECKOUT-008 | Verify incomplete delivery address |
| TS-CHECKOUT-009 | Verify invalid PIN/ZIP code |
| TS-CHECKOUT-010 | Verify payment method selection |
| TS-CHECKOUT-011 | Verify payment information validation |
| TS-CHECKOUT-012 | Verify order summary |
| TS-CHECKOUT-013 | Verify product quantity in order summary |
| TS-CHECKOUT-014 | Verify product price in order summary |
| TS-CHECKOUT-015 | Verify subtotal in order summary |
| TS-CHECKOUT-016 | Verify tax in order summary where applicable |
| TS-CHECKOUT-017 | Verify final order total |
| TS-CHECKOUT-018 | Verify modification of delivery address |
| TS-CHECKOUT-019 | Verify navigation between checkout steps |
| TS-CHECKOUT-020 | Verify duplicate order submission prevention |
| TS-CHECKOUT-021 | Verify successful checkout |

---

## 13. Delivery Address Scenarios

| ID | Test Scenario |
|---|---|
| TS-ADDRESS-001 | Verify delivery address section |
| TS-ADDRESS-002 | Enter valid delivery address |
| TS-ADDRESS-003 | Leave mandatory address fields blank |
| TS-ADDRESS-004 | Enter invalid PIN/ZIP code |
| TS-ADDRESS-005 | Enter invalid characters |
| TS-ADDRESS-006 | Enter minimum allowed address length |
| TS-ADDRESS-007 | Enter maximum allowed address length |
| TS-ADDRESS-008 | Verify address validation messages |
| TS-ADDRESS-009 | Modify delivery address |
| TS-ADDRESS-010 | Verify selected address in order summary |

---

## 14. Payment Scenarios

| ID | Test Scenario |
|---|---|
| TS-PAY-001 | Verify payment section is available |
| TS-PAY-002 | Verify available payment methods |
| TS-PAY-003 | Select a valid payment method |
| TS-PAY-004 | Verify mandatory payment fields |
| TS-PAY-005 | Enter invalid payment information |
| TS-PAY-006 | Submit payment with incomplete information |
| TS-PAY-007 | Verify payment validation messages |
| TS-PAY-008 | Verify payment amount matches order total |
| TS-PAY-009 | Verify payment failure handling where applicable |
| TS-PAY-010 | Verify successful payment flow using approved test data |

Note: Actual payment gateway certification and real financial transactions are outside the scope of this manual testing project.

---

## 15. Order Placement Scenarios

| ID | Test Scenario |
|---|---|
| TS-ORDER-001 | Place an order with valid information |
| TS-ORDER-002 | Verify order creation |
| TS-ORDER-003 | Verify order reference number |
| TS-ORDER-004 | Verify order date |
| TS-ORDER-005 | Verify order amount |
| TS-ORDER-006 | Verify ordered products |
| TS-ORDER-007 | Verify ordered quantities |
| TS-ORDER-008 | Verify delivery information |
| TS-ORDER-009 | Verify order status |
| TS-ORDER-010 | Verify successful order confirmation |
| TS-ORDER-011 | Verify duplicate order prevention |
| TS-ORDER-012 | Verify order creation after page refresh according to requirements |

---

## 16. Order Confirmation Scenarios

| ID | Test Scenario |
|---|---|
| TS-CONFIRM-001 | Verify order confirmation page |
| TS-CONFIRM-002 | Verify confirmation message |
| TS-CONFIRM-003 | Verify order reference |
| TS-CONFIRM-004 | Verify order amount |
| TS-CONFIRM-005 | Verify ordered products |
| TS-CONFIRM-006 | Verify ordered quantities |
| TS-CONFIRM-007 | Verify order date |
| TS-CONFIRM-008 | Verify navigation to order history |
| TS-CONFIRM-009 | Verify navigation after order completion |

---

## 17. Order History Scenarios

| ID | Test Scenario |
|---|---|
| TS-HISTORY-001 | Verify order history page is accessible |
| TS-HISTORY-002 | Verify previous orders are displayed |
| TS-HISTORY-003 | Verify order reference |
| TS-HISTORY-004 | Verify order date |
| TS-HISTORY-005 | Verify order amount |
| TS-HISTORY-006 | Verify order status |
| TS-HISTORY-007 | Verify order details |
| TS-HISTORY-008 | Verify multiple orders |
| TS-HISTORY-009 | Verify empty order history |
| TS-HISTORY-010 | Verify unauthorized access to order history |
| TS-HISTORY-011 | Verify order history after placing a new order |

---

## 18. Navigation Scenarios

| ID | Test Scenario |
|---|---|
| TS-NAV-001 | Verify header navigation |
| TS-NAV-002 | Verify navigation to product listing |
| TS-NAV-003 | Verify navigation to product details |
| TS-NAV-004 | Verify navigation to shopping cart |
| TS-NAV-005 | Verify navigation to checkout |
| TS-NAV-006 | Verify navigation to order history |
| TS-NAV-007 | Verify navigation to account section |
| TS-NAV-008 | Verify browser back navigation |
| TS-NAV-009 | Verify browser forward navigation |
| TS-NAV-010 | Verify navigation after logout |
| TS-NAV-011 | Verify broken or invalid navigation links |
| TS-NAV-012 | Verify navigation consistency across pages |

---

## 19. Session Management Scenarios

| ID | Test Scenario |
|---|---|
| TS-SESSION-001 | Verify session is created after successful login |
| TS-SESSION-002 | Verify authenticated user can access protected pages |
| TS-SESSION-003 | Verify unauthenticated user cannot access protected pages |
| TS-SESSION-004 | Verify session after page refresh |
| TS-SESSION-005 | Verify session after browser back navigation |
| TS-SESSION-006 | Verify logout terminates session |
| TS-SESSION-007 | Verify protected page access after logout |
| TS-SESSION-008 | Verify session timeout where applicable |
| TS-SESSION-009 | Verify application behavior after session expiration |
| TS-SESSION-010 | Verify user-specific data is not exposed to another user |

---

## 20. Error Handling Scenarios

| ID | Test Scenario |
|---|---|
| TS-ERROR-001 | Verify validation for blank mandatory fields |
| TS-ERROR-002 | Verify invalid email error |
| TS-ERROR-003 | Verify invalid password error |
| TS-ERROR-004 | Verify password mismatch error |
| TS-ERROR-005 | Verify invalid quantity error |
| TS-ERROR-006 | Verify empty cart checkout error |
| TS-ERROR-007 | Verify invalid address error |
| TS-ERROR-008 | Verify invalid PIN/ZIP error |
| TS-ERROR-009 | Verify invalid payment information error |
| TS-ERROR-010 | Verify appropriate error message for failed operations |
| TS-ERROR-011 | Verify application does not crash for invalid input |
| TS-ERROR-012 | Verify technical error details are not unnecessarily exposed |

---

## 21. UI and Usability Scenarios

| ID | Test Scenario |
|---|---|
| TS-UI-001 | Verify consistent page layout |
| TS-UI-002 | Verify field labels |
| TS-UI-003 | Verify button labels |
| TS-UI-004 | Verify button alignment and visibility |
| TS-UI-005 | Verify input field alignment |
| TS-UI-006 | Verify product image display |
| TS-UI-007 | Verify text readability |
| TS-UI-008 | Verify validation message visibility |
| TS-UI-009 | Verify error message clarity |
| TS-UI-010 | Verify consistent navigation |
| TS-UI-011 | Verify cart information visibility |
| TS-UI-012 | Verify checkout information clarity |
| TS-UI-013 | Verify order confirmation information |
| TS-UI-014 | Verify no overlapping UI elements |
| TS-UI-015 | Verify page content is displayed correctly after browser resize |

---

## 22. Cross-Browser Compatibility Scenarios

| ID | Test Scenario |
|---|---|
| TS-COMP-001 | Verify application launch in Google Chrome |
| TS-COMP-002 | Verify application launch in Microsoft Edge |
| TS-COMP-003 | Verify registration in Google Chrome |
| TS-COMP-004 | Verify registration in Microsoft Edge |
| TS-COMP-005 | Verify login in Google Chrome |
| TS-COMP-006 | Verify login in Microsoft Edge |
| TS-COMP-007 | Verify product browsing in Google Chrome |
| TS-COMP-008 | Verify product browsing in Microsoft Edge |
| TS-COMP-009 | Verify cart functionality in Google Chrome |
| TS-COMP-010 | Verify cart functionality in Microsoft Edge |
| TS-COMP-011 | Verify checkout in Google Chrome |
| TS-COMP-012 | Verify checkout in Microsoft Edge |
| TS-COMP-013 | Verify order placement in Google Chrome |
| TS-COMP-014 | Verify order placement in Microsoft Edge |
| TS-COMP-015 | Verify UI consistency across supported browsers |

---

## 23. Negative Testing Scenarios

| ID | Test Scenario |
|---|---|
| TS-NEG-001 | Submit registration with invalid data |
| TS-NEG-002 | Login with invalid credentials |
| TS-NEG-003 | Submit forms with blank mandatory fields |
| TS-NEG-004 | Enter invalid email format |
| TS-NEG-005 | Enter invalid password |
| TS-NEG-006 | Enter mismatched passwords |
| TS-NEG-007 | Search using invalid characters |
| TS-NEG-008 | Search for a non-existing product |
| TS-NEG-009 | Enter invalid product quantity |
| TS-NEG-010 | Enter zero product quantity |
| TS-NEG-011 | Enter negative product quantity |
| TS-NEG-012 | Checkout with an empty cart |
| TS-NEG-013 | Submit incomplete delivery information |
| TS-NEG-014 | Enter invalid PIN/ZIP code |
| TS-NEG-015 | Enter invalid payment information |
| TS-NEG-016 | Access protected pages without authentication |
| TS-NEG-017 | Access protected pages after logout |

---

## 24. Boundary Value Scenarios

| ID | Test Scenario |
|---|---|
| TS-BVA-001 | Verify password minimum boundary |
| TS-BVA-002 | Verify password maximum boundary |
| TS-BVA-003 | Verify password below minimum |
| TS-BVA-004 | Verify password above maximum |
| TS-BVA-005 | Verify product quantity minimum boundary |
| TS-BVA-006 | Verify product quantity maximum boundary |
| TS-BVA-007 | Verify quantity below minimum |
| TS-BVA-008 | Verify quantity above maximum |
| TS-BVA-009 | Verify name minimum length |
| TS-BVA-010 | Verify name maximum length |
| TS-BVA-011 | Verify search input boundary |
| TS-BVA-012 | Verify PIN/ZIP code length boundary |
| TS-BVA-013 | Verify address minimum length |
| TS-BVA-014 | Verify address maximum length |

The exact boundary values will be determined from the application's documented requirements.

---

## 25. Equivalence Partitioning Scenarios

| ID | Test Scenario |
|---|---|
| TS-EQP-001 | Verify valid email partition |
| TS-EQP-002 | Verify invalid email partition |
| TS-EQP-003 | Verify valid password partition |
| TS-EQP-004 | Verify invalid password partition |
| TS-EQP-005 | Verify valid quantity partition |
| TS-EQP-006 | Verify invalid quantity partition |
| TS-EQP-007 | Verify valid PIN/ZIP partition |
| TS-EQP-008 | Verify invalid PIN/ZIP partition |
| TS-EQP-009 | Verify valid search input partition |
| TS-EQP-010 | Verify invalid search input partition |

---

## 26. Exploratory Testing Scenarios

| ID | Test Scenario |
|---|---|
| TS-EXP-001 | Navigate through the application using unexpected paths |
| TS-EXP-002 | Refresh pages during critical workflows |
| TS-EXP-003 | Use browser back and forward buttons during checkout |
| TS-EXP-004 | Open multiple product pages in separate tabs |
| TS-EXP-005 | Add and remove products repeatedly |
| TS-EXP-006 | Rapidly change cart quantity |
| TS-EXP-007 | Attempt checkout after removing all cart items |
| TS-EXP-008 | Refresh the order confirmation page |
| TS-EXP-009 | Logout and attempt to continue using protected functionality |
| TS-EXP-010 | Enter unexpected characters in input fields |

---

## 27. End-to-End Scenarios

### 27.1 New User Purchase Flow

| ID | Test Scenario |
|---|---|
| TS-E2E-001 | Register a new user, login, browse products, add a product to cart, checkout, place an order, verify confirmation, verify order history, and logout |

### 27.2 Existing User Purchase Flow

| ID | Test Scenario |
|---|---|
| TS-E2E-002 | Login with an existing user, search for a product, apply filter/sort, add product to cart, update quantity, checkout, place order, and verify order history |

### 27.3 Multi-Product Purchase Flow

| ID | Test Scenario |
|---|---|
| TS-E2E-003 | Login, add multiple products to cart, update quantities, verify totals, complete checkout, place order, and verify order details |

### 27.4 Negative Checkout Flow

| ID | Test Scenario |
|---|---|
| TS-E2E-004 | Login, add product to cart, proceed to checkout, submit invalid or incomplete information, verify validation, correct the information, and complete the order |

---

## 28. Integration Scenarios

| ID | Test Scenario |
|---|---|
| TS-INT-001 | Verify Login to Product Listing integration |
| TS-INT-002 | Verify Product Listing to Product Details integration |
| TS-INT-003 | Verify Product Details to Cart integration |
| TS-INT-004 | Verify Cart to Checkout integration |
| TS-INT-005 | Verify Checkout to Order Placement integration |
| TS-INT-006 | Verify Order Placement to Order Confirmation integration |
| TS-INT-007 | Verify Order Placement to Order History integration |
| TS-INT-008 | Verify Logout and Protected Page integration |
| TS-INT-009 | Verify product price consistency between listing, details, cart, and checkout |
| TS-INT-010 | Verify product quantity consistency between product, cart, and order |
| TS-INT-011 | Verify order total consistency between cart, checkout, confirmation, and history |

---

## 29. Test Scenario Execution Status

Test scenario execution will be tracked using the following statuses:

| Status | Meaning |
|---|---|
| Not Executed | Scenario has not yet been executed |
| Pass | Scenario completed successfully |
| Fail | Scenario did not meet the expected behavior |
| Blocked | Scenario cannot be executed because of a dependency or blocker |
| Not Applicable | Scenario is not applicable to the current build or requirement |

---

## 30. Test Scenario Priority

Scenarios will be prioritized based on business impact.

| Priority | Description |
|---|---|
| P1 - High | Critical business functionality such as login, cart, checkout, and order placement |
| P2 - Medium | Important functionality such as search, filtering, sorting, and order history |
| P3 - Low | Minor UI, usability, or less critical functionality |

---

## 31. Scenario Coverage

The scenarios in this document provide coverage for the major functional areas of the E-Commerce Web Application.

Coverage includes:

- User registration
- Authentication
- Logout
- Product listing
- Product search
- Product filtering
- Product sorting
- Product details
- Shopping cart
- Checkout
- Delivery address
- Payment
- Order placement
- Order confirmation
- Order history
- Navigation
- Session management
- Error handling
- UI and usability
- Browser compatibility
- Negative testing
- Boundary testing
- Equivalence partitioning
- Exploratory testing
- Integration testing
- End-to-end testing

---

## 32. Traceability

Each test scenario should be mapped to the applicable requirement and subsequently to one or more detailed test cases.

The expected traceability flow is:

```text
Requirement
     |
     v
Test Scenario
     |
     v
Test Case
     |
     v
Test Execution
     |
     v
Defect
```

This traceability helps ensure that requirements are covered and that identified defects can be linked back to the affected functionality.

---

## 33. Review and Maintenance

Test scenarios should be reviewed whenever:

- New functionality is introduced.
- Existing functionality is modified.
- Requirements change.
- Defects reveal missing coverage.
- Business rules change.
- New browsers are supported.
- Existing workflows are changed.

Any updated scenario should retain a unique and traceable identifier.

---

## 34. Document Revision History

| Version | Date | Author | Description |
|---|---|---|---|
| 1.0 | TBD | A P CHANDAN | Initial Test Scenarios document |
| 1.1 | TBD | A P CHANDAN | Updated scenarios and coverage |
