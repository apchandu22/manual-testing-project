# Test Plan

## 1. Document Information

| Field | Details |
|---|---|
| Project | E-Commerce Web Application |
| Document | Test Plan |
| Version | 1.0 |
| Status | Baseline |
| Testing Type | Manual Testing |
| Prepared By | A P CHANDAN |
| Document Purpose | Define the overall testing strategy and approach for the E-Commerce Web Application |

---

# 2. Project Overview

The E-Commerce Web Application allows users to register, log in, browse products, search for products, filter and sort products, view product details, manage shopping cart items, complete checkout, place orders, and view order history.

This Test Plan defines the approach that will be followed to validate the application's functional behavior, usability, compatibility, data accuracy, and major business workflows through manual testing.

The testing process will focus on identifying functional defects, validating business requirements, verifying negative scenarios, and ensuring that changes do not adversely affect existing functionality.

---

# 3. Test Objectives

The main objectives of testing are:

1. Verify that the application meets the documented requirements.
2. Verify that users can register successfully.
3. Verify that registered users can log in and log out.
4. Verify authentication and protected-page behavior.
5. Verify product listing functionality.
6. Verify product search functionality.
7. Verify product filtering functionality.
8. Verify product sorting functionality.
9. Verify product details functionality.
10. Verify product availability behavior.
11. Verify add-to-cart functionality.
12. Verify cart quantity management.
13. Verify cart removal functionality.
14. Verify cart price calculations.
15. Verify checkout functionality.
16. Verify delivery address validation.
17. Verify payment method selection.
18. Verify order review functionality.
19. Verify order placement.
20. Verify order confirmation.
21. Verify order history.
22. Verify order status information.
23. Verify navigation between application modules.
24. Verify validation and error messages.
25. Verify basic UI and usability behavior.
26. Verify supported browser compatibility.
27. Identify and document defects.
28. Retest defects after fixes.
29. Perform regression testing after application changes.
30. Maintain traceability between requirements and test cases.

---

# 4. Test Scope

## 4.1 In Scope

The following application areas are included in the testing scope.

### 4.1.1 User Registration

Testing will cover:

- Registration page access
- First Name validation
- Last Name validation
- Email validation
- Password validation
- Confirm Password validation
- Mandatory field validation
- Invalid input handling
- Duplicate email handling
- Successful registration
- Registration confirmation

---

### 4.1.2 User Login

Testing will cover:

- Login page access
- Valid credentials
- Invalid credentials
- Blank email
- Blank password
- Invalid email format
- Password masking
- Login error messages
- Successful login
- Logout
- Protected-page access
- Session behavior

---

### 4.1.3 Product Listing

Testing will cover:

- Product listing page
- Product names
- Product images
- Product prices
- Product descriptions
- Product availability
- Product navigation
- Product count
- Product display consistency

---

### 4.1.4 Product Search

Testing will cover:

- Search using valid keywords
- Search using partial keywords
- Search using invalid keywords
- Search with no matching products
- Empty search
- Search case handling
- Search result accuracy
- Clearing search criteria

---

### 4.1.5 Product Filtering

Testing will cover:

- Category filtering
- Price filtering
- Multiple filters
- Filter result accuracy
- Applying filters
- Removing filters
- Clear filters
- Filter persistence where applicable

---

### 4.1.6 Product Sorting

Testing will cover:

- Price low to high
- Price high to low
- Alphabetical sorting
- Sorting accuracy
- Sorting after search
- Sorting after filtering
- Resetting sorting where applicable

---

### 4.1.7 Product Details

Testing will cover:

- Product details page
- Product name
- Product image
- Product price
- Product description
- Product availability
- Product quantity
- Add to Cart
- Unavailable product behavior

---

### 4.1.8 Shopping Cart

Testing will cover:

- Add product
- Add multiple products
- View cart
- Increase quantity
- Decrease quantity
- Remove product
- Empty cart
- Product subtotal
- Tax calculation
- Final total
- Invalid quantity
- Cart persistence according to application behavior

---

### 4.1.9 Checkout

Testing will cover:

- Checkout navigation
- Customer information
- Delivery address
- Mandatory address fields
- PIN/ZIP validation
- Payment method
- Payment information validation
- Order summary
- Order total
- Address modification
- Order review
- Empty cart checkout
- Duplicate order submission
- Successful checkout

---

### 4.1.10 Order Placement

Testing will cover:

- Place Order
- Successful order placement
- Order confirmation
- Order reference
- Order details
- Order amount
- Order date
- Order status

---

### 4.1.11 Order History

Testing will cover:

- Order history access
- Previous orders
- Multiple orders
- Order details
- Order status
- Empty order history
- Order sorting where applicable
- Unauthorized access

---

### 4.1.12 Navigation

Testing will cover:

- Header navigation
- Product navigation
- Cart navigation
- Account navigation
- Checkout navigation
- Browser back navigation
- Application navigation
- Logout navigation

---

### 4.1.13 UI and Usability

Testing will cover:

- Consistent layout
- Correct field labels
- Correct button labels
- Button behavior
- Error message visibility
- Validation message clarity
- Image display
- Page alignment
- Basic usability
- Navigation consistency

---

### 4.1.14 Compatibility

Testing will cover supported desktop browsers.

Initial browser coverage:

- Google Chrome
- Microsoft Edge

---

### 4.2 Out of Scope

The following activities are outside the scope of this project:

- Performance testing
- Load testing
- Stress testing
- Volume testing
- Security penetration testing
- VAPT
- API automation
- Mobile application testing
- Database performance testing
- Infrastructure testing
- Production monitoring
- Payment gateway certification
- Third-party service certification
- Accessibility certification
- Infrastructure security testing

Basic security-related functional checks are included, such as:

- Login authentication
- Logout behavior
- Protected page access
- Basic user data isolation

---

# 5. Testing Strategy

The testing strategy will follow a structured manual testing approach.

The overall process will be:

```text
Requirement Analysis
        ↓
Test Planning
        ↓
Test Scenario Identification
        ↓
Test Case Design
        ↓
Test Data Preparation
        ↓
Test Case Review
        ↓
Smoke Testing
        ↓
Functional Testing
        ↓
Integration Testing
        ↓
Negative Testing
        ↓
Defect Reporting
        ↓
Defect Retesting
        ↓
Regression Testing
        ↓
Test Closure

---
## 6. Test Environment

### 6.1 Hardware Environment

| Component | Details |
|---|---|
| Device | Desktop / Laptop |
| Operating System | Windows |
| Network | Stable Internet Connection |
| Screen | Standard Desktop/Laptop Resolution |

### 6.2 Software Environment

| Component | Details |
|---|---|
| Browser 1 | Google Chrome |
| Browser 2 | Microsoft Edge |
| Testing Type | Manual Testing |
| Defect Tracking | JIRA / GitHub Issues |
| Documentation | Markdown |
| Version Control | GitHub |

### 6.3 Environment Requirements

The test environment should:

- Provide access to the application under test.
- Support required test accounts.
- Provide required test data.
- Support supported browsers.
- Allow defect reproduction.
- Provide a stable network connection.
- Allow application data to be reset where required.

---
# 7. Testing Types

## 7.1 Functional Testing

Functional testing will verify that the application functionality works according to the documented requirements.

Functional testing will cover:

- User Registration
- User Login
- Product Listing
- Product Search
- Product Filtering
- Product Sorting
- Product Details
- Shopping Cart
- Checkout
- Order Placement
- Order History
- Logout

The objective is to verify that each feature produces the expected result for valid and invalid inputs.

---

## 7.2 Smoke Testing

Smoke testing will be performed on every new application build to verify that the build is stable enough for detailed testing.

Critical smoke scenarios include:

1. Launch the application.
2. Verify the application loads successfully.
3. Log in with valid credentials.
4. Verify the home/product page.
5. Browse products.
6. Open a product.
7. Add the product to the cart.
8. Open the shopping cart.
9. Verify cart details.
10. Proceed to checkout.
11. Verify the checkout page.
12. Place an order where test payment functionality is available.
13. Verify order confirmation.

### Critical Smoke Flow

```text
Launch Application
        |
        v
Login
        |
        v
Browse Products
        |
        v
View Product
        |
        v
Add Product to Cart
        |
        v
Open Cart
        |
        v
Proceed to Checkout
        |
        v
Place Order
        |
        v
Verify Order Confirmation
```
### 7.3. Regression Testing

Regression testing will be performed after application changes, enhancements, or defect fixes.

The objective is to verify that existing functionality has not been negatively impacted by recent changes.

Regression testing will cover both the changed functionality and related business-critical areas.

## 7.4. Sanity Testing

Sanity testing will be performed after minor changes, enhancements, or defect fixes to verify that the specific functionality is working as expected.

The purpose of sanity testing is to determine whether the application is stable enough for detailed regression testing.

Sanity testing will focus on the changed functionality and its closely related areas.

Examples:

Verify a fixed login issue.
Verify a modified search functionality.
Verify a cart quantity fix.
Verify a checkout validation fix.
Verify an order placement defect fix.
Sanity Testing Flow
Change / Defect Fix
        |
        v
Build Deployed
        |
        v
Test Changed Functionality
        |
        v
Test Related Functionality
        |
        v
Pass / Fail
        |
        +---- Pass ----> Continue Regression Testing
        |
        +---- Fail ----> Report / Reopen Defect

Sanity testing is narrower than regression testing and focuses primarily on the impacted functionality.

## 7.5 Integration Testing

Integration testing will verify that different modules of the E-Commerce Web Application work correctly when integrated with each other.

The objective of integration testing is to validate:

- Data flow between modules
- Communication between application components
- Navigation between related pages
- Data consistency across modules
- Error handling during module interaction
- Complete business workflows

The following integrations will be validated.

### Login to Product Listing

```text
Login
   |
   v
Authentication
   |
   v
Product Listing

Verification:

User authentication is successful.
Authorized users are redirected to the correct page.
Session is created successfully.
User-specific data is loaded correctly.

## 7.5 Integration Testing

Integration testing will verify that different modules of the E-Commerce Web Application work correctly when integrated with each other.

The objective of integration testing is to validate:

- Data flow between modules
- Communication between application components
- Navigation between related pages
- Data consistency across modules
- Error handling during module interaction
- Complete business workflows

The following integrations will be validated.

### Login to Product Listing

```text
Login
   |
   v
Authentication
   |
   v
Product Listing
```

Verification:

- User authentication is successful.
- Authorized users are redirected to the correct page.
- User session is created successfully.
- User-specific data is loaded correctly.

---

### Product Listing to Product Details

```text
Product Listing
       |
       v
Select Product
       |
       v
Product Details
```

Verification:

- Selected product opens successfully.
- Product name is correct.
- Product image is correct.
- Product price is correct.
- Product description is correct.
- Product availability is displayed correctly.

---

### Product Details to Shopping Cart

```text
Product Details
       |
       v
Add to Cart
       |
       v
Shopping Cart
```

Verification:

- Selected product is added successfully.
- Product name is displayed correctly.
- Product price is transferred correctly.
- Selected quantity is maintained.
- Product subtotal is calculated correctly.

---

### Shopping Cart to Checkout

```text
Shopping Cart
       |
       v
Proceed to Checkout
       |
       v
Checkout
```

Verification:

- Cart items are displayed correctly.
- Product quantities are maintained.
- Product prices are accurate.
- Subtotal is calculated correctly.
- Applicable tax is calculated correctly.
- Final total is calculated correctly.
- Cart information is correctly transferred to checkout.

---

### Checkout to Order Placement

```text
Checkout
    |
    v
Customer Information
    |
    v
Delivery Address
    |
    v
Payment Method
    |
    v
Order Review
    |
    v
Place Order
```

Verification:

- Customer information is accepted correctly.
- Delivery address is validated correctly.
- Selected payment method is retained.
- Order summary displays correct information.
- Product quantities are correct.
- Product prices are correct.
- Final order amount is correct.
- Order can be placed successfully when all required information is valid.

---

### Order Placement to Order Confirmation

```text
Place Order
     |
     v
Order Processing
     |
     v
Order Confirmation
```

Verification:

- Order is created successfully.
- Order confirmation is displayed.
- Order reference/order ID is generated where applicable.
- Order amount is displayed correctly.
- Order details are accurate.

---

### Order Placement to Order History

```text
Place Order
     |
     v
Order Confirmation
     |
     v
Order History
     |
     v
Order Details
```

Verification:

- Newly placed order appears in order history.
- Order information is accurate.
- Order amount matches the placed order.
- Order status is displayed correctly.
- Order details can be opened successfully.

---

### Integration Testing Focus Areas

Integration testing will focus on:

- Module-to-module interaction
- Data transfer accuracy
- Data consistency
- Navigation flow
- Session management
- Business workflow continuity
- Error handling
- Validation across integrated modules
- Correct calculation and transfer of order information

The objective is to ensure that individual modules work together correctly as part of the complete application workflow.

---

## 7.6 System Testing
