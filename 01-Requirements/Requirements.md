# Requirements Document

## 1. Document Information

| Field | Details |
|---|---|
| Project | E-Commerce Web Application |
| Document | Requirements Document |
| Version | 1.0 |
| Status | Baseline |
| Testing Type | Manual Testing |
| Prepared By | A P CHANDAN |

---

# 2. Project Overview

The E-Commerce web application allows users to create an account, log in, browse products, search and filter products, view product details, manage their shopping cart, complete checkout, place orders, and view order history.

The purpose of this document is to define the functional and non-functional requirements that will be used as the basis for manual testing.

---

# 3. User Registration Requirements

## REQ-REG-001 – User Registration

The application shall allow new users to create an account.

The registration form shall contain:

- First Name
- Last Name
- Email Address
- Password
- Confirm Password

## REQ-REG-002 – Mandatory Fields

The application shall validate all mandatory registration fields.

The user shall not be allowed to complete registration when required fields are blank.

## REQ-REG-003 – First Name Validation

The application shall validate the First Name field according to the defined input rules.

## REQ-REG-004 – Last Name Validation

The application shall validate the Last Name field according to the defined input rules.

## REQ-REG-005 – Email Validation

The application shall validate the email address format.

Invalid email formats shall not be accepted.

## REQ-REG-006 – Duplicate Email

The application shall prevent registration using an email address that is already registered.

## REQ-REG-007 – Password Validation

The application shall validate the password according to the defined password requirements.

## REQ-REG-008 – Confirm Password

The application shall verify that Password and Confirm Password contain matching values.

## REQ-REG-009 – Registration Confirmation

After successful registration, the application shall display an appropriate success confirmation.

---

# 4. User Login Requirements

## REQ-LOGIN-001 – User Login

Registered users shall be able to log in using valid credentials.

## REQ-LOGIN-002 – Invalid Credentials

The application shall reject invalid login credentials.

## REQ-LOGIN-003 – Mandatory Login Fields

The application shall validate mandatory login fields.

## REQ-LOGIN-004 – Email Format

The application shall validate the email format during login.

## REQ-LOGIN-005 – Login Error Message

The application shall display a clear and appropriate error message when authentication fails.

## REQ-LOGIN-006 – Successful Login

After successful authentication, the user shall be redirected to the appropriate authenticated page.

## REQ-LOGIN-007 – Password Masking

The password field shall hide the entered password characters.

## REQ-LOGIN-008 – Logout

Authenticated users shall be able to log out of the application.

## REQ-LOGIN-009 – Protected Pages

Users who are not authenticated shall not be able to access protected user pages.

---

# 5. Product Listing Requirements

## REQ-PROD-001 – Product Listing

The application shall display available products on the product listing page.

## REQ-PROD-002 – Product Name

Each product shall display its product name.

## REQ-PROD-003 – Product Image

Each product shall display an appropriate product image.

## REQ-PROD-004 – Product Price

Each product shall display its current price.

## REQ-PROD-005 – Product Availability

The application shall indicate whether a product is available for purchase.

## REQ-PROD-006 – Product Description

The application shall provide product description information.

## REQ-PROD-007 – Product Navigation

Users shall be able to navigate from the product listing page to the product details page.

---

# 6. Product Search Requirements

## REQ-SEARCH-001 – Product Search

Users shall be able to search for products using keywords.

## REQ-SEARCH-002 – Relevant Search Results

The application shall display products relevant to the entered search keyword.

## REQ-SEARCH-003 – Partial Keyword Search

The application shall support partial keyword searches according to the defined search behavior.

## REQ-SEARCH-004 – Invalid Search

The application shall display an appropriate message when no products match the search criteria.

## REQ-SEARCH-005 – Empty Search

The application shall handle an empty search submission according to the defined behavior.

## REQ-SEARCH-006 – Search Case Handling

Search behavior shall be consistent when users enter keywords using different letter cases.

## REQ-SEARCH-007 – Clear Search

Users shall be able to clear the search criteria and return to the appropriate product listing.

---

# 7. Product Filtering Requirements

## REQ-FILTER-001 – Product Filtering

Users shall be able to filter products using available filter options.

## REQ-FILTER-002 – Category Filter

Users shall be able to filter products by category when category filtering is available.

## REQ-FILTER-003 – Price Filter

Users shall be able to filter products based on the available price range.

## REQ-FILTER-004 – Multiple Filters

The application shall support multiple filter selections where applicable.

## REQ-FILTER-005 – Filter Results

The displayed products shall match the selected filter criteria.

## REQ-FILTER-006 – Clear Filters

Users shall be able to remove applied filters and return to the default product listing.

---

# 8. Product Sorting Requirements

## REQ-SORT-001 – Product Sorting

Users shall be able to sort products using the available sorting options.

## REQ-SORT-002 – Price Low to High

The application shall support sorting products from lowest price to highest price when the option is available.

## REQ-SORT-003 – Price High to Low

The application shall support sorting products from highest price to lowest price when the option is available.

## REQ-SORT-004 – Name Sorting

The application shall support alphabetical product sorting when the option is available.

## REQ-SORT-005 – Sorting Accuracy

Products shall be displayed according to the selected sorting option.

---

# 9. Product Details Requirements

## REQ-DETAIL-001 – Product Details

Users shall be able to view detailed information for a selected product.

## REQ-DETAIL-002 – Product Information

The product details page shall display:

- Product Name
- Product Image
- Product Price
- Product Description
- Product Availability

## REQ-DETAIL-003 – Product Quantity

Users shall be able to select the quantity of the product before adding it to the cart.

## REQ-DETAIL-004 – Add to Cart

Users shall be able to add an available product to the shopping cart.

## REQ-DETAIL-005 – Unavailable Product

Unavailable products shall not be purchasable.

---

# 10. Shopping Cart Requirements

## REQ-CART-001 – Add Product

Users shall be able to add products to the shopping cart.

## REQ-CART-002 – View Cart

Users shall be able to view products currently added to the shopping cart.

## REQ-CART-003 – Multiple Products

Users shall be able to add multiple different products to the cart.

## REQ-CART-004 – Increase Quantity

Users shall be able to increase the quantity of a product in the cart.

## REQ-CART-005 – Decrease Quantity

Users shall be able to decrease the quantity of a product in the cart.

## REQ-CART-006 – Remove Product

Users shall be able to remove products from the cart.

## REQ-CART-007 – Subtotal Calculation

The application shall calculate the product subtotal correctly based on product price and quantity.

## REQ-CART-008 – Tax Calculation

The application shall calculate applicable taxes correctly.

## REQ-CART-009 – Final Total

The application shall display the correct final cart total.

## REQ-CART-010 – Empty Cart

The application shall display an appropriate message when the cart contains no products.

## REQ-CART-011 – Invalid Quantity

The application shall prevent invalid product quantities such as negative values or other unsupported values.

## REQ-CART-012 – Cart Persistence

The cart shall behave according to the defined session and user-account persistence requirements.

---

# 11. Checkout Requirements

## REQ-CHECKOUT-001 – Checkout Access

Users shall be able to proceed from the shopping cart to checkout when the cart contains valid products.

## REQ-CHECKOUT-002 – Customer Information

The checkout process shall allow users to provide required customer information.

## REQ-CHECKOUT-003 – Delivery Address

Users shall be able to enter a delivery address.

The address may include:

- Full Name
- Address
- City
- State
- PIN/ZIP Code
- Phone Number

## REQ-CHECKOUT-004 – Mandatory Address Fields

The application shall validate mandatory delivery address fields.

## REQ-CHECKOUT-005 – PIN/ZIP Validation

The application shall validate the PIN/ZIP code according to the defined format.

## REQ-CHECKOUT-006 – Payment Method

Users shall be able to select an available payment method.

## REQ-CHECKOUT-007 – Payment Validation

The application shall validate required payment information.

## REQ-CHECKOUT-008 – Order Summary

The checkout page shall display a summary of the products being ordered.

## REQ-CHECKOUT-009 – Checkout Total

The checkout total shall match the applicable cart total.

## REQ-CHECKOUT-010 – Address Modification

Users shall be able to modify delivery information before placing the order.

## REQ-CHECKOUT-011 – Empty Cart Checkout

Users shall not be able to complete checkout when the cart is empty.

## REQ-CHECKOUT-012 – Order Review

Users shall be able to review order details before final submission.

## REQ-CHECKOUT-013 – Duplicate Submission

The application shall prevent accidental duplicate order submission.

## REQ-CHECKOUT-014 – Successful Checkout

The application shall allow users to successfully complete checkout when all required information is valid.

---

# 12. Order Placement Requirements

## REQ-ORDER-001 – Place Order

Users shall be able to place an order after successfully completing checkout.

## REQ-ORDER-002 – Order Confirmation

The application shall display an order confirmation after successful order placement.

## REQ-ORDER-003 – Order Reference

The application shall generate a unique order reference for each successfully placed order.

## REQ-ORDER-004 – Order Details

The order shall contain relevant information including:

- Order Reference
- Product
- Quantity
- Price
- Total Amount
- Order Date
- Order Status

## REQ-ORDER-005 – Order Total

The order total shall match the amount confirmed during checkout.

---

# 13. Order History Requirements

## REQ-HISTORY-001 – Order History

Authenticated users shall be able to view their previous orders.

## REQ-HISTORY-002 – Order Information

Order history shall display relevant order information.

## REQ-HISTORY-003 – Order Details

Users shall be able to open an individual order and view its details.

## REQ-HISTORY-004 – Multiple Orders

The application shall display multiple orders when multiple orders exist.

## REQ-HISTORY-005 – Empty Order History

New users with no previous orders shall see an appropriate empty-state message.

## REQ-HISTORY-006 – Order Status

The application shall display the current order status where applicable.

## REQ-HISTORY-007 – Order Persistence

Successfully placed orders shall remain available according to the application's order-history requirements.

## REQ-HISTORY-008 – Unauthorized Access

Unauthenticated users shall not be able to access another user's order history.

## REQ-HISTORY-009 – Order Sorting

Order history shall be displayed according to the defined sorting behavior.

---

# 14. Navigation Requirements

## REQ-NAV-001 – Application Navigation

Users shall be able to navigate between major application sections.

## REQ-NAV-002 – Header Navigation

The application header shall provide access to relevant navigation options.

## REQ-NAV-003 – Cart Navigation

Users shall be able to navigate to the shopping cart.

## REQ-NAV-004 – Account Navigation

Authenticated users shall be able to access their account-related functionality.

## REQ-NAV-005 – Back Navigation

Browser and application navigation should behave consistently without causing unintended data loss.

---

# 15. UI and Usability Requirements

## REQ-UI-001 – Consistent UI

The application interface should maintain consistent layouts and controls across pages.

## REQ-UI-002 – Validation Messages

Validation messages should be clear and understandable.

## REQ-UI-003 – Button Behavior

Buttons should have clear labels and perform their intended actions.

## REQ-UI-004 – Field Labels

Input fields should have appropriate labels or instructions.

## REQ-UI-005 – Error Visibility

Important validation and error messages should be visible to users.

## REQ-UI-006 – Product Images

Product images should load correctly and be displayed without unintended distortion.

---

# 16. Compatibility Requirements

## REQ-COMP-001 – Browser Compatibility

The application should function correctly on supported browsers.

The initial test scope includes:

- Google Chrome
- Microsoft Edge

## REQ-COMP-002 – Responsive Behavior

The application should maintain usable layouts across supported screen sizes where responsive behavior is part of the application scope.

---

# 17. Security-Related Functional Requirements

> Security requirements listed here are limited to basic functional validation. Dedicated security/VAPT testing is outside the scope of this manual-testing project.

## REQ-SEC-001 – Password Protection

Passwords shall not be displayed in plain text while being entered.

## REQ-SEC-002 – Authentication

Protected functionality shall require valid authentication.

## REQ-SEC-003 – Session Protection

After logout, authenticated functionality should not remain accessible through normal navigation.

## REQ-SEC-004 – User Data Isolation

A user should only be able to access their own account and order information.

---

# 18. Non-Functional Requirements

## REQ-NFR-001 – Usability

The application should provide an intuitive and easy-to-understand user experience.

## REQ-NFR-002 – Compatibility

The application should work consistently across supported browsers.

## REQ-NFR-003 – Reliability

The application should consistently perform core business operations without unexpected failures.

## REQ-NFR-004 – Data Accuracy

Product, cart, checkout, and order information should remain accurate throughout the user journey.

## REQ-NFR-005 – Maintainability

Application behavior and validation messages should be consistent and understandable for future maintenance.

---

# 19. End-to-End Business Flow

The primary E-Commerce business flow is:

```text
User Registration
       ↓
User Login
       ↓
Browse Products
       ↓
Search Product
       ↓
Filter / Sort Products
       ↓
View Product Details
       ↓
Add Product to Cart
       ↓
Update Cart
       ↓
Proceed to Checkout
       ↓
Enter Delivery Information
       ↓
Select Payment Method
       ↓
Review Order
       ↓
Place Order
       ↓
Order Confirmation
       ↓
View Order History
