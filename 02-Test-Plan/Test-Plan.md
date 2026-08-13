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

## 2. Project Overview

The E-Commerce Web Application allows users to register, log in, browse products, search for products, filter and sort products, view product details, manage shopping cart items, complete checkout, place orders, and view order history.

This Test Plan defines the approach that will be followed to validate the application's functional behavior, usability, compatibility, data accuracy, and major business workflows through manual testing.

The testing process will focus on identifying functional defects, validating business requirements, verifying negative scenarios, and ensuring that changes do not adversely affect existing functionality.

---

## 3. Test Objectives

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

## 4. Test Scope

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

## 4.2 Out of Scope

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

## 5. Testing Strategy

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
```

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
## 7. Testing Types

### 7.1 Functional Testing

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

### 7.2 Smoke Testing

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
### 7.3 Regression Testing

Regression testing will be performed after application changes, enhancements, or defect fixes.

The objective is to verify that existing functionality has not been negatively impacted by recent changes.

Regression testing will cover both the changed functionality and related business-critical areas.

### 7.4 Sanity Testing

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

### 7.5 Integration Testing

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
### 7.6 System Testing

System testing will verify the complete E-Commerce Web Application as an integrated system against the specified functional and business requirements.

The objective is to validate the application's end-to-end behavior from the user's perspective and ensure that all major modules work correctly together in the complete application environment.

System testing will cover:

- Application launch and accessibility
- User registration
- User login and logout
- Product browsing
- Product search
- Product filtering
- Product sorting
- Product details
- Shopping cart management
- Checkout
- Address validation
- Payment method selection
- Order placement
- Order confirmation
- Order history
- Navigation
- Validation messages
- Error handling
- Session behavior
- Supported browser compatibility

#### System Testing Scenarios

| ID | Scenario | Expected Result |
|---|---|---|
| ST-001 | Launch the application | Application loads successfully without critical errors |
| ST-002 | Register a new user | User account is created successfully |
| ST-003 | Login with valid credentials | User is authenticated and redirected to the appropriate page |
| ST-004 | Login with invalid credentials | Appropriate error message is displayed |
| ST-005 | Browse products | Available products are displayed correctly |
| ST-006 | Search for a product | Relevant search results are displayed |
| ST-007 | Apply product filters | Products matching the selected filters are displayed |
| ST-008 | Sort products | Products are displayed in the selected order |
| ST-009 | Open product details | Correct product information is displayed |
| ST-010 | Add product to cart | Product is added to the shopping cart |
| ST-011 | Update cart quantity | Cart quantity and total amount are updated correctly |
| ST-012 | Remove product from cart | Selected product is removed from the cart |
| ST-013 | Proceed to checkout | User is navigated to the checkout page |
| ST-014 | Enter valid delivery information | Delivery information is accepted |
| ST-015 | Enter invalid delivery information | Appropriate validation message is displayed |
| ST-016 | Review order summary | Product, quantity, price, tax, and total are displayed correctly |
| ST-017 | Place an order | Order is created successfully |
| ST-018 | Verify order confirmation | Confirmation message and order reference are displayed |
| ST-019 | Open order history | User's previous orders are displayed |
| ST-020 | Logout | User session is terminated successfully |

#### Critical System Flow

```text
User Registration / Login
          |
          v
Product Listing
          |
          v
Search / Filter / Sort
          |
          v
Product Details
          |
          v
Add to Cart
          |
          v
Shopping Cart
          |
          v
Checkout
          |
          v
Delivery Information
          |
          v
Payment Method
          |
          v
Order Review
          |
          v
Place Order
          |
          v
Order Confirmation
          |
          v
Order History
          |
          v
Logout
```

#### System Testing Focus Areas

System testing will primarily focus on:

1. Complete business workflows.
2. Correct interaction between application modules.
3. Data consistency across different pages.
4. Correct calculation of cart and order totals.
5. Validation of mandatory fields.
6. Correct error and validation messages.
7. Authentication and session behavior.
8. Correct order creation and order history.
9. Navigation between application modules.
10. Consistent behavior across supported browsers.

#### System Testing Expected Result

The application should perform the complete user workflow successfully without critical or high-severity functional defects that prevent the core business process from being completed.

---

### 7.7 End-to-End Testing

End-to-End testing will verify complete business workflows from the initial user action through the final expected outcome.

The objective is to ensure that the entire application workflow functions correctly across all relevant modules.

#### End-to-End Scenario 1 — New User Purchase

```text
Open Application
      |
      v
Register New User
      |
      v
Login
      |
      v
Browse Products
      |
      v
Search Product
      |
      v
Open Product Details
      |
      v
Add Product to Cart
      |
      v
Open Cart
      |
      v
Verify Product and Price
      |
      v
Proceed to Checkout
      |
      v
Enter Delivery Address
      |
      v
Select Payment Method
      |
      v
Review Order
      |
      v
Place Order
      |
      v
Verify Order Confirmation
      |
      v
Open Order History
      |
      v
Verify Order Details
      |
      v
Logout
```

#### End-to-End Scenario 2 — Existing User Purchase

```text
Open Application
      |
      v
Login with Existing User
      |
      v
Browse Products
      |
      v
Apply Filter / Sort
      |
      v
Select Product
      |
      v
Add Product to Cart
      |
      v
Update Quantity
      |
      v
Proceed to Checkout
      |
      v
Verify Order Summary
      |
      v
Place Order
      |
      v
Verify Confirmation
      |
      v
Verify Order History
```

#### End-to-End Validation Points

The following should be verified during the complete workflow:

- User authentication
- Product availability
- Product information
- Product price
- Cart quantity
- Cart subtotal
- Applicable tax
- Final order total
- Delivery information
- Payment method
- Order details
- Order reference
- Order status
- Order history

#### End-to-End Expected Result

The complete business workflow should execute successfully from user login or registration through order confirmation and order history without data loss, incorrect calculations, navigation failures, or blocking functional defects.

---

### 7.8 Exploratory Testing

Exploratory testing will be performed to identify defects that may not be covered by predefined test cases.

Testers will simultaneously explore the application, design test ideas, execute tests, and analyze the results.

Exploratory testing will focus on:

- Unexpected user behavior
- Unusual navigation paths
- Invalid input combinations
- Rapid repeated actions
- Browser back and forward navigation
- Refreshing pages during workflows
- Multiple tabs
- Empty states
- Unexpected data
- Boundary conditions
- UI inconsistencies
- Error handling
- Session behavior

#### Exploratory Testing Examples

1. Search for a product using special characters.
2. Enter extremely long text in input fields.
3. Refresh the cart page after adding products.
4. Use browser back navigation during checkout.
5. Open multiple product pages in different tabs.
6. Change product quantity repeatedly.
7. Remove all products from the cart.
8. Attempt checkout with an empty cart.
9. Refresh the order confirmation page.
10. Logout and attempt to access a protected page.

#### Exploratory Testing Expected Result

The application should handle unexpected but realistic user actions gracefully without crashes, data corruption, incorrect calculations, or loss of user information.

---

### 7.9 Usability Testing

Usability testing will verify whether the application is easy to understand, navigate, and use from an end-user perspective.

The testing will focus on the clarity, consistency, and ease of use of the application's user interface.

Usability testing will cover:

- Page layout
- Navigation
- Button placement
- Field labels
- Error messages
- Validation messages
- Readability
- Consistency
- Product information visibility
- Cart visibility
- Checkout flow
- Order confirmation
- Overall user experience

#### Usability Checks

| ID | Usability Check | Expected Result |
|---|---|---|
| UT-001 | Verify navigation menu | Navigation options are clear and understandable |
| UT-002 | Verify button labels | Button labels clearly describe their actions |
| UT-003 | Verify form labels | Input fields have clear and meaningful labels |
| UT-004 | Verify validation messages | Messages clearly explain the required correction |
| UT-005 | Verify product information | Product information is easy to understand |
| UT-006 | Verify cart information | Quantity, price, and total are clearly displayed |
| UT-007 | Verify checkout flow | Checkout steps are easy to follow |
| UT-008 | Verify order confirmation | Confirmation information is clearly displayed |

#### Usability Expected Result

Users should be able to understand the application's functionality and complete the major business workflows without unnecessary confusion or navigation difficulties.

---

### 7.10 Compatibility Testing

Compatibility testing will verify that the application behaves consistently across supported browsers and standard desktop environments.

Initial browser coverage:

- Google Chrome
- Microsoft Edge

#### Compatibility Areas

Testing will verify:

- Application loading
- Login
- Registration
- Product listing
- Search
- Filtering
- Sorting
- Product details
- Shopping cart
- Checkout
- Order placement
- Order history
- Navigation
- UI rendering
- Error messages

#### Compatibility Test Matrix

| Functionality | Chrome | Edge |
|---|---|---|
| Application Launch | Not Executed | Not Executed |
| Registration | Not Executed | Not Executed |
| Login | Not Executed | Not Executed |
| Product Listing | Not Executed | Not Executed |
| Product Search | Not Executed | Not Executed |
| Product Filter | Not Executed | Not Executed |
| Product Sort | Not Executed | Not Executed |
| Product Details | Not Executed | Not Executed |
| Shopping Cart | Not Executed | Not Executed |
| Checkout | Not Executed | Not Executed |
| Order Placement | Not Executed | Not Executed |
| Order History | Not Executed | Not Executed |
| Logout | Not Executed | Not Executed |

#### Compatibility Expected Result

The application should provide consistent functionality and acceptable UI rendering across the supported browsers without browser-specific functional defects.

---

### 7.11 Negative Testing

Negative testing will verify that the application handles invalid, unexpected, incomplete, or incorrect inputs appropriately.

The objective is to ensure that invalid user actions do not result in incorrect processing, application crashes, data corruption, or unexpected behavior.

Negative testing will cover:

- Invalid login credentials
- Invalid email format
- Blank mandatory fields
- Invalid password
- Password mismatch
- Duplicate registration
- Invalid search input
- Invalid filter values
- Invalid quantity
- Zero quantity
- Negative quantity
- Excessive quantity
- Invalid delivery information
- Missing address fields
- Invalid PIN/ZIP code
- Invalid payment information
- Checkout with empty cart
- Unauthorized page access
- Session expiration behavior

#### Negative Testing Examples

| ID | Negative Scenario | Expected Result |
|---|---|---|
| NT-001 | Login with invalid email | Appropriate error message is displayed |
| NT-002 | Login with incorrect password | Login is rejected |
| NT-003 | Submit registration with blank mandatory fields | Validation messages are displayed |
| NT-004 | Enter mismatched passwords | Password mismatch validation is displayed |
| NT-005 | Add invalid quantity | Invalid quantity is rejected |
| NT-006 | Checkout with empty cart | Checkout is prevented or appropriate message is displayed |
| NT-007 | Enter invalid delivery information | Validation message is displayed |
| NT-008 | Access protected page after logout | User is prevented from accessing the protected page |

#### Negative Testing Expected Result

The application should reject invalid input appropriately and provide clear feedback without crashing or processing incorrect information.

---

### 7.12 Boundary Value Testing

Boundary Value Testing will be used to verify application behavior at the minimum, maximum, and boundary values of accepted input ranges.

The objective is to identify defects that commonly occur at input boundaries.

Potential boundary areas include:

- Password length
- Name length
- Search input length
- Product quantity
- PIN/ZIP code length
- Address field length
- Numeric fields
- Character limits

#### Boundary Test Examples

| Field | Boundary Values to Consider |
|---|---|
| Password | Minimum - 1, Minimum, Minimum + 1 |
| Product Quantity | Minimum - 1, Minimum, Minimum + 1, Maximum - 1, Maximum, Maximum + 1 |
| Name | Minimum allowed, maximum allowed, maximum + 1 |
| Search | Empty, minimum characters, maximum characters |
| PIN/ZIP | One less than required length, required length, one more than required length |
| Address | Empty, minimum length, maximum length, maximum + 1 |

The exact boundary values will be determined from the application's documented requirements.

#### Boundary Value Expected Result

The application should accept valid boundary values and reject values outside the permitted range with appropriate validation messages.

---

### 7.13 Equivalence Partitioning

Equivalence Partitioning will be used to divide input data into valid and invalid groups.

Instead of testing every possible input value, representative values from each partition will be selected.

#### Example — Email Field

| Partition | Example | Expected Result |
|---|---|---|
| Valid email | user@example.com | Accepted |
| Invalid format | userexample.com | Rejected |
| Missing username | @example.com | Rejected |
| Missing domain | user@ | Rejected |
| Blank | Empty | Rejected |

#### Example — Product Quantity

| Partition | Example | Expected Result |
|---|---|---|
| Valid quantity | 1 | Accepted |
| Valid quantity | 5 | Accepted |
| Zero quantity | 0 | Rejected or handled according to requirement |
| Negative quantity | -1 | Rejected |
| Non-numeric value | abc | Rejected |
| Excessive quantity | Above allowed limit | Rejected or handled according to requirement |

#### Example — Password

| Partition | Example | Expected Result |
|---|---|---|
| Valid password | Meets all requirements | Accepted |
| Too short | Below minimum length | Rejected |
| Too long | Above maximum length | Rejected |
| Blank | Empty | Rejected |
| Invalid format | Does not meet password rules | Rejected |

#### Equivalence Partitioning Expected Result

Each valid partition should be accepted and each invalid partition should be rejected according to the documented application requirements.

---
### 7.14 Ad Hoc Testing

Ad Hoc testing will be performed without predefined test cases to identify unexpected defects and application behavior.

The tester will use practical experience and product knowledge to perform unscripted checks.

Ad Hoc testing may include:

- Random navigation across application pages
- Repeated clicks on buttons
- Rapid addition and removal of products
- Changing cart quantities repeatedly
- Refreshing pages during transactions
- Using browser back and forward buttons
- Logging in and logging out repeatedly
- Opening multiple browser tabs
- Switching between application modules
- Entering unexpected input values

#### Ad Hoc Testing Expected Result

The application should remain stable and should not produce crashes, data corruption, incorrect calculations, or unexpected behavior during unscripted testing.

---

### 7.15 Retesting

Retesting will be performed after a defect has been fixed to verify that the specific defect has been resolved.

The tester will execute the failed test case or scenario again using the same or equivalent test conditions.

#### Retesting Process

```text
Defect Reported
      |
      v
Developer Fix
      |
      v
New Build Deployed
      |
      v
Execute Failed Test Case
      |
      v
Verify Expected Result
      |
      +---- Pass ----> Close Defect
      |
      +---- Fail ----> Reopen Defect
```

#### Retesting Guidelines

- Retest the exact failed scenario.
- Use the same test data where applicable.
- Verify the expected result.
- Verify that the defect no longer occurs.
- Capture evidence when required.
- Update the defect status.
- Reopen the defect if the issue still exists.

#### Retesting Expected Result

The reported defect should be resolved and the previously failed scenario should pass according to the expected behavior.

---

### 7.16 Defect-Based Testing

Defect-based testing will focus on areas where defects have previously been identified or where similar defects are likely to occur.

The objective is to verify the defect fix and identify related or similar issues.

Defect-based testing may include:

- Retesting the reported defect
- Testing related functionality
- Testing similar input combinations
- Testing related application modules
- Testing boundary conditions
- Testing negative scenarios
- Testing affected workflows

#### Defect-Based Testing Example

If a defect is reported where the cart total is incorrect after changing quantity:

1. Verify the original reported scenario.
2. Change quantity from 1 to 2.
3. Change quantity from 2 to 5.
4. Decrease quantity.
5. Remove the product.
6. Add another product.
7. Verify subtotal.
8. Verify tax.
9. Verify final total.
10. Verify checkout order total.

#### Expected Result

The reported defect and related scenarios should behave correctly without introducing new functional issues.

---

### 7.17 Build Verification Testing

Build Verification Testing will be performed when a new application build is deployed to the test environment.

The objective is to verify that the build is installable, accessible, and stable enough for detailed testing.

Build verification will include:

- Application availability
- Application launch
- Login
- Basic navigation
- Product listing
- Product details
- Add to cart
- Cart access
- Checkout access

#### Expected Result

The new build should be accessible and stable enough to proceed with planned testing.

---

### 7.18 Data Validation Testing

Data validation testing will verify that data displayed and processed by the application is accurate and consistent across related workflows.

Testing will focus on:

- Product names
- Product prices
- Product quantities
- Cart subtotal
- Tax
- Final total
- Customer information
- Delivery information
- Order details
- Order reference
- Order status

#### Data Validation Examples

| Data | Validation |
|---|---|
| Product Name | Product name should remain consistent |
| Product Price | Displayed price should match the applicable product price |
| Quantity | Cart quantity should match the selected quantity |
| Subtotal | Subtotal should be calculated correctly |
| Tax | Tax should be calculated according to the applicable rule |
| Total | Final amount should be accurate |
| Order Details | Order details should match the placed order |
| Order History | Order information should be retained correctly |

#### Expected Result

Data should remain accurate and consistent when transferred between application modules.

---

### 7.19 Session and Authentication Testing

Session and authentication testing will verify that user authentication and session-related behavior work correctly.

Testing will cover:

- Login with valid credentials
- Login with invalid credentials
- Logout
- Session persistence
- Session termination
- Protected page access
- Browser back navigation after logout
- Refresh after logout
- Accessing protected pages without login
- Session timeout where applicable

#### Expected Result

Only authenticated users should be able to access protected functionality, and logout should terminate the active user session according to the application requirements.

---

### 7.20 Error Handling Testing

Error handling testing will verify that the application responds appropriately when unexpected or invalid conditions occur.

Testing will cover:

- Invalid input
- Missing mandatory data
- Invalid credentials
- Invalid product quantity
- Empty cart
- Invalid delivery information
- Invalid payment information
- Page refresh during workflows
- Network-related errors where testable
- Application navigation errors

#### Error Handling Expected Result

The application should display meaningful error messages and should not expose unnecessary technical information or cause application crashes.

---

### 7.21 Test Case Design Techniques

The following test design techniques will be used where applicable:

- Equivalence Partitioning
- Boundary Value Analysis
- Decision Table Testing
- State Transition Testing
- Use Case Testing
- Error Guessing
- Exploratory Testing

#### Technique Selection

| Technique | Application Area |
|---|---|
| Equivalence Partitioning | Form and input validation |
| Boundary Value Analysis | Quantity, length, and numeric fields |
| Decision Table Testing | Business rules and conditions |
| State Transition Testing | Login, order, and status workflows |
| Use Case Testing | End-to-end business workflows |
| Error Guessing | Common user mistakes and historical defects |
| Exploratory Testing | Unscripted defect discovery |

---

# 8. Test Data

Test data will be prepared before execution to support positive, negative, boundary, and integration scenarios.

## 8.1 User Test Data

Test data may include:

- Valid user details
- Invalid user details
- Existing user accounts
- New user accounts
- Invalid email addresses
- Valid passwords
- Invalid passwords
- Password mismatch combinations

## 8.2 Product Test Data

Product test data may include:

- Available products
- Unavailable products
- Products with different prices
- Products from different categories
- Products with different quantities
- Products with long names or descriptions

## 8.3 Cart Test Data

Cart test data may include:

- Single product
- Multiple products
- Minimum quantity
- Maximum allowed quantity
- Invalid quantity
- Zero quantity
- Negative quantity

## 8.4 Checkout Test Data

Checkout test data may include:

- Valid customer information
- Invalid customer information
- Valid delivery address
- Incomplete address
- Invalid PIN/ZIP code
- Valid payment test data
- Invalid payment test data

## 8.5 Order Test Data

Order test data may include:

- Successful orders
- Multiple orders
- Orders with different products
- Orders with different quantities
- Orders with different totals
- Different order statuses where supported

---

# 9. Test Case Management

Test cases will be created and maintained based on application requirements and identified test scenarios.

Each test case should contain:

| Field | Description |
|---|---|
| Test Case ID | Unique identifier |
| Module | Application module |
| Test Scenario | Scenario being validated |
| Preconditions | Conditions required before execution |
| Test Data | Data required for execution |
| Test Steps | Steps to execute |
| Expected Result | Expected application behavior |
| Actual Result | Observed behavior |
| Status | Pass / Fail / Blocked / Not Executed |
| Priority | Business importance |
| Severity | Defect impact where applicable |
| Remarks | Additional information |

---

# 10. Test Execution

Test execution will be performed according to the approved test cases and test schedule.

The execution process will include:

1. Review test case.
2. Verify preconditions.
3. Prepare test data.
4. Execute test steps.
5. Compare actual and expected results.
6. Mark test status.
7. Report defects for failed scenarios.
8. Attach supporting evidence where required.
9. Retest fixed defects.
10. Execute regression testing.
11. Update execution results.

## 10.1 Test Status

The following statuses will be used:

- Pass
- Fail
- Blocked
- Not Executed
- Not Applicable

---

# 11. Defect Management

Defects identified during testing will be documented and tracked until closure.

## 11.1 Defect Reporting Process

```text
Defect Identified
       |
       v
Reproduce Defect
       |
       v
Collect Evidence
       |
       v
Log Defect
       |
       v
Developer Analysis
       |
       v
Defect Fixed
       |
       v
Retesting
       |
       +---- Pass ----> Close
       |
       +---- Fail ----> Reopen
```

## 11.2 Defect Information

Each defect should contain:

- Defect ID
- Summary
- Description
- Module
- Environment
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Evidence
- Reported By
- Assigned To
- Status
- Resolution
- Retest Result

## 11.3 Defect Severity

| Severity | Description |
|---|---|
| Critical | Prevents major business functionality or causes application failure |
| High | Major functionality is not working and significantly impacts testing or users |
| Medium | Functionality is affected but a workaround may exist |
| Low | Minor functional or UI issue with limited impact |

## 11.4 Defect Priority

| Priority | Description |
|---|---|
| P1 - High | Immediate attention required |
| P2 - Medium | Should be fixed in the planned release |
| P3 - Low | Can be addressed based on priority and release scope |

---

# 12. Requirements Traceability

Requirements Traceability will be maintained to ensure that all documented requirements are covered by appropriate test scenarios and test cases.

The RTM will provide traceability between:

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

## 12.1 RTM Fields

| Field | Description |
|---|---|
| Requirement ID | Unique requirement identifier |
| Requirement Description | Requirement being tested |
| Test Scenario ID | Related scenario |
| Test Case ID | Related test case |
| Execution Status | Pass / Fail / Blocked |
| Defect ID | Related defect, if any |

## 12.2 RTM Objective

The objective is to ensure:

- Complete requirement coverage
- No major requirement is missed
- Test cases can be traced to requirements
- Defects can be traced to affected requirements
- Testing progress can be measured

---

# 13. Entry Criteria

Testing can begin when the following conditions are satisfied:

1. Requirements are available and sufficiently clear.
2. Test scope is defined.
3. Test environment is available.
4. Application build is deployed.
5. Required test data is available.
6. Test cases are prepared and reviewed.
7. Required test accounts are available.
8. Critical dependencies are available.
9. Major blocking issues preventing testing are resolved.
10. Test team has access to required tools and environments.

---

# 14. Exit Criteria

Testing may be considered complete when:

1. Planned test cases have been executed.
2. Critical business workflows have been validated.
3. Critical and high-severity defects are resolved or formally accepted.
4. Required regression testing is completed.
5. Defect retesting is completed.
6. Test results are documented.
7. Requirement coverage is reviewed.
8. Remaining known issues are documented.
9. Test summary is prepared.
10. Stakeholders provide the required approval.

---

# 15. Test Deliverables

The following deliverables may be created during the testing lifecycle:

- Test Plan
- Test Scenarios
- Test Cases
- Test Data
- Requirement Traceability Matrix
- Defect Reports
- Test Execution Results
- Regression Test Results
- Retesting Results
- Test Summary Report
- Test Closure Report

---

# 16. Roles and Responsibilities

## 16.1 QA / Tester

Responsibilities include:

- Requirement analysis
- Test planning
- Test scenario preparation
- Test case design
- Test data preparation
- Test execution
- Defect reporting
- Defect retesting
- Regression testing
- Test result documentation
- Test closure activities

## 16.2 Developer

Responsibilities include:

- Analyze reported defects
- Identify root cause
- Fix defects
- Provide updated builds
- Support defect investigation
- Provide technical clarification when required

## 16.3 QA Lead / Test Lead

Responsibilities include:

- Review test strategy
- Review test cases
- Assign testing activities
- Monitor test execution
- Review defects
- Track testing progress
- Coordinate with development and stakeholders
- Review test completion

## 16.4 Product Owner / Business Stakeholder

Responsibilities include:

- Clarify business requirements
- Validate expected business behavior
- Prioritize business-critical defects
- Review release readiness
- Provide acceptance where required

---

# 17. Test Metrics

Testing metrics will be used to monitor test progress, quality, and defect status.

Key metrics may include:

- Total test cases
- Executed test cases
- Passed test cases
- Failed test cases
- Blocked test cases
- Not Executed test cases
- Test execution percentage
- Pass percentage
- Fail percentage
- Total defects
- Open defects
- Closed defects
- Reopened defects
- Critical defects
- High-severity defects
- Medium-severity defects
- Low-severity defects

## 17.1 Test Execution Percentage

```text
Test Execution % =
Executed Test Cases / Total Planned Test Cases × 100
```

## 17.2 Pass Percentage

```text
Pass % =
Passed Test Cases / Executed Test Cases × 100
```

## 17.3 Defect Closure Percentage

```text
Defect Closure % =
Closed Defects / Total Reported Defects × 100
```

---

# 18. Risks and Mitigation

| Risk | Impact | Mitigation |
|---|---|---|
| Requirements are unclear | High | Clarify requirements with stakeholders |
| Test environment unavailable | High | Coordinate environment availability in advance |
| Build instability | High | Perform smoke testing before detailed testing |
| Test data unavailable | Medium | Prepare test data before execution |
| Defect fixes are delayed | High | Track defects regularly and prioritize critical issues |
| Third-party dependency unavailable | Medium | Coordinate with dependent teams and use approved test alternatives |
| Limited testing time | High | Prioritize critical business workflows |
| Frequent application changes | Medium | Perform focused sanity and regression testing |
| Browser-specific issues | Medium | Execute compatibility testing |
| Incomplete requirements | Medium | Review requirements and maintain traceability |

---

# 19. Assumptions

The following assumptions are considered for this test plan:

1. Required application requirements are available.
2. Test environment will be available during planned execution.
3. Test data can be created or provided when required.
4. Required test accounts will be available.
5. Development builds will be deployed to the test environment.
6. Defect fixes will be provided for retesting.
7. Supported browsers will be available.
8. Required stakeholders will be available for clarification.
9. The application will be accessible during scheduled testing.
10. Any changes to scope will be communicated to the testing team.

---

# 20. Dependencies

Testing depends on the following:

- Application build availability
- Test environment availability
- Requirement availability
- Test data availability
- Test account availability
- Development support
- Defect fixes
- Third-party services required for application workflows
- Browser availability
- Network availability
- Stakeholder clarification

Any dependency that prevents testing should be communicated and tracked.

---

# 21. Test Schedule

The testing schedule will be planned according to project requirements, release timelines, and build availability.

A typical testing sequence will be:

```text
Requirement Analysis
        |
        v
Test Planning
        |
        v
Test Scenario Design
        |
        v
Test Case Design
        |
        v
Test Data Preparation
        |
        v
Build Verification / Smoke Testing
        |
        v
Functional Testing
        |
        v
Integration Testing
        |
        v
System Testing
        |
        v
End-to-End Testing
        |
        v
Regression Testing
        |
        v
Retesting
        |
        v
Test Closure
```

The actual dates will be updated based on project timelines.

---

# 22. Test Completion and Closure

Test closure activities will be performed after the planned testing activities are completed.

Closure activities include:

1. Verify execution of planned test cases.
2. Review open and closed defects.
3. Complete required retesting.
4. Complete regression testing.
5. Review requirement coverage.
6. Document known issues.
7. Prepare test summary.
8. Capture lessons learned.
9. Obtain required stakeholder approval.
10. Archive testing documentation.

## 22.1 Test Summary Report

The Test Summary Report may include:

- Testing scope
- Testing period
- Test environment
- Test execution summary
- Pass/fail results
- Defect summary
- Open defects
- Closed defects
- Risk summary
- Requirement coverage
- Known limitations
- Final testing status

---

# 23. Approval

The Test Plan should be reviewed and approved by the appropriate project stakeholders before formal test execution begins.

| Role | Name | Approval | Date |
|---|---|---|---|
| QA / Tester | A P CHANDAN | Pending | TBD |
| QA Lead / Test Lead | TBD | Pending | TBD |
| Product Owner / Stakeholder | TBD | Pending | TBD |

---

# 24. Document Revision History

| Version | Date | Author | Description |
|---|---|---|---|
| 1.0 | TBD | A P CHANDAN | Initial Test Plan |
| 1.1 | TBD | A P CHANDAN | Updated testing strategy and test coverage |
