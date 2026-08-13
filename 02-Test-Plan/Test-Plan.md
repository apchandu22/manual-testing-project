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

---

# 2. Objective

The objective of this test plan is to define the testing approach, scope, resources, test environment, test types, entry criteria, exit criteria, risks, and deliverables for validating the E-Commerce Web Application.

The primary goal is to verify that the application meets the defined functional requirements and provides a reliable and user-friendly shopping experience.

---

# 3. Test Objectives

The following objectives will be achieved through testing:

- Verify that users can successfully register and log in.
- Verify product listing functionality.
- Verify product search functionality.
- Verify product filtering functionality.
- Verify product sorting functionality.
- Verify product details functionality.
- Verify shopping cart functionality.
- Verify checkout functionality.
- Verify order placement functionality.
- Verify order history functionality.
- Verify navigation between application modules.
- Validate mandatory field and input validations.
- Verify appropriate error and validation messages.
- Verify basic authentication and authorization behavior.
- Verify supported browser compatibility.
- Identify, document, and track defects.
- Perform retesting of fixed defects.
- Perform regression testing to ensure existing functionality is not impacted by changes.

---

# 4. Scope

## 4.1 In Scope

The following modules are included in the testing scope:

### User Management
- User Registration
- User Login
- User Logout
- Authentication validation
- Mandatory field validation
- Input validation

### Product Management
- Product Listing
- Product Search
- Product Filtering
- Product Sorting
- Product Details
- Product Availability

### Shopping Cart
- Add Product
- Remove Product
- Update Quantity
- Multiple Products
- Subtotal Calculation
- Tax Calculation
- Final Total
- Empty Cart

### Checkout
- Checkout Navigation
- Customer Information
- Delivery Address
- Address Validation
- Payment Method Selection
- Order Summary
- Order Review
- Checkout Validation

### Order Management
- Order Placement
- Order Confirmation
- Order Reference
- Order Details
- Order History
- Order Status

### UI and Navigation
- Application Navigation
- Header Navigation
- Cart Navigation
- Account Navigation
- Validation Messages
- Button Behavior
- Field Labels
- Basic Usability

### Compatibility
- Google Chrome
- Microsoft Edge
- Supported screen sizes where applicable

---

# 5. Out of Scope

The following activities are outside the scope of this project:

- Performance Testing
- Load Testing
- Stress Testing
- Security Penetration Testing
- Vulnerability Assessment and Penetration Testing (VAPT)
- API Automation
- Mobile Application Testing
- Database Performance Testing
- Infrastructure Testing
- Production Monitoring
- Third-Party Service Certification
- Payment Gateway Certification

Basic security-related functional checks such as authentication, logout behavior, and user data isolation are included.

---

# 6. Testing Types

The following testing types will be performed.

## 6.1 Functional Testing

Verify that each application feature works according to the defined requirements.

Examples:

- Registration
- Login
- Search
- Cart
- Checkout
- Order Placement

---

## 6.2 Smoke Testing

Smoke testing will be performed on a new build to verify that the critical application functionality is stable enough for detailed testing.

Critical smoke flow:

```text
Launch Application
        ↓
Login
        ↓
Browse Products
        ↓
View Product
        ↓
Add to Cart
        ↓
Checkout
        ↓
Place Order

## 6.3 Sanity Testing

Sanity testing will be performed after specific changes or bug fixes to verify that the affected functionality works correctly.

---

## 6.4 Regression Testing

Regression testing will be performed after application changes or defect fixes to ensure that existing functionality has not been negatively affected.

Regression areas include:

- Login
- Product Search
- Product Details
- Cart
- Checkout
- Order Placement
- Order History

---

## 6.5 Retesting

Retesting will be performed after defects are fixed to verify that the reported defects have been successfully resolved.

---

## 6.6 Integration Testing

Integration testing will validate interactions between major application modules.

Examples:

```text
Login → Product Listing
Product → Cart
Cart → Checkout
Checkout → Order
Order → Order History

6.7 UI and Usability Testing

The application UI will be checked for:

Consistent layout
Correct labels
Readable messages
Proper button behavior
Appropriate field validation
Correct image display
Navigation consistency
User-friendly error messages
6.8 Compatibility Testing

The application will be tested on supported browsers to identify browser-specific issues.

Initial browser coverage:

Browser	Coverage
Google Chrome	Primary
Microsoft Edge	Secondary
6.9 Negative Testing

Negative testing will verify how the application behaves with invalid, unexpected, or incomplete inputs.

Examples:

Invalid email
Invalid password
Blank mandatory fields
Incorrect password confirmation
Invalid search keyword
Invalid quantity
Missing address
Invalid PIN/ZIP code
Invalid payment information
7. Test Approach

Testing will follow a structured manual testing approach.

Requirement Analysis
        ↓
Test Scenario Identification
        ↓
Test Case Design
        ↓
Test Data Preparation
        ↓
Test Case Review
        ↓
Test Execution
        ↓
Defect Reporting
        ↓
Defect Retesting
        ↓
Regression Testing
        ↓
Test Closure

Testing will be performed using risk-based prioritization, with critical business flows receiving higher execution priority.

8. Test Design Techniques

The following test design techniques will be used.

8.1 Equivalence Partitioning

Input data will be divided into valid and invalid groups.

Example:

Valid:
user@example.com

Invalid:
userexample.com
user@
@example.com
8.2 Boundary Value Analysis

Boundary values will be tested for fields that have defined limits.

Example, if a field accepts 1–50 characters:

0 characters
1 character
2 characters
49 characters
50 characters
51 characters
8.3 Decision Table Testing

Decision tables will be used where multiple conditions affect the expected result.

Example:

Valid Email + Valid Password
        ↓
Login Successful

Valid Email + Invalid Password
        ↓
Login Failed

Invalid Email + Valid Password
        ↓
Login Failed

Invalid Email + Invalid Password
        ↓
Login Failed
8.4 State Transition Testing

State transitions will be validated for workflows such as order processing.

Example:

Order Placed
     ↓
Order Confirmed
     ↓
Order Processing
     ↓
Order Shipped
     ↓
Order Delivered

Where the application supports these statuses.

8.5 Error Guessing

Experience-based testing will be used to identify common failure conditions.

Examples:

Double-clicking Place Order
Refreshing checkout
Removing all cart items
Using invalid quantities
Navigating back after logout
Using expired sessions
Submitting forms multiple times
9. Test Scenarios

Major test scenarios will cover the following areas.

Registration
Verify successful registration.
Verify mandatory field validation.
Verify email format validation.
Verify duplicate email handling.
Verify password validation.
Verify password confirmation.
Login
Verify successful login.
Verify invalid credentials.
Verify blank fields.
Verify password masking.
Verify logout.
Verify protected page access.
Product
Verify product listing.
Verify product search.
Verify no-result search.
Verify product filtering.
Verify product sorting.
Verify product details.
Verify product availability.
Cart
Verify adding products.
Verify removing products.
Verify quantity updates.
Verify multiple products.
Verify subtotal calculation.
Verify tax calculation.
Verify final total.
Verify empty cart.
Checkout
Verify checkout navigation.
Verify address validation.
Verify payment method selection.
Verify order summary.
Verify total amount.
Verify order review.
Verify successful checkout.
Verify duplicate submission prevention.
Orders
Verify order placement.
Verify order confirmation.
Verify order reference.
Verify order details.
Verify order history.
Verify order status.
Verify unauthorized order access.
10. Test Environment

Testing will be performed in a controlled test environment.

Hardware
Item	Configuration
Device	Desktop/Laptop
Operating System	Windows
Screen	Standard desktop resolution
Software
Component	Details
Browser 1	Google Chrome
Browser 2	Microsoft Edge
Testing Type	Manual
Defect Tracking	JIRA / GitHub Issues
Documentation	Markdown
11. Test Data

Test data will be prepared for all major functional areas.

User Data
Valid User
Invalid User
Duplicate User
New User
Login Data
Valid Email + Valid Password
Valid Email + Invalid Password
Invalid Email + Valid Password
Invalid Email + Invalid Password
Blank Email
Blank Password
Product Data
Valid Product
Unavailable Product
Multiple Products
Products with Different Prices
Cart Data
Single Product
Multiple Products
Quantity = 1
Quantity > 1
Invalid Quantity
Empty Cart
Checkout Data
Valid Address
Invalid Address
Blank Mandatory Fields
Valid PIN/ZIP
Invalid PIN/ZIP
Valid Payment Information
Invalid Payment Information
12. Test Case Priorities

Test cases will be prioritized as follows:

Priority	Description
P0	Critical business flow; execution is mandatory
P1	High business impact
P2	Medium business impact
P3	Low business impact

Critical P0 areas include:

Login
Product Selection
Add to Cart
Checkout
Order Placement
13. Defect Management

Defects identified during testing will be documented with sufficient information for investigation and resolution.

Each defect should contain:

Defect ID
Summary
Description
Environment
Preconditions
Steps to Reproduce
Test Data
Expected Result
Actual Result
Severity
Priority
Evidence
Status
Assigned To
Reported By
14. Defect Severity
Severity	Description
Critical	Application or critical business flow is unusable
High	Major functionality is not working
Medium	Functionality is partially affected
Low	Minor functional or UI issue
15. Defect Priority
Priority	Description
P0	Immediate resolution required
P1	High priority fix
P2	Normal priority
P3	Low priority
16. Defect Life Cycle

The expected defect life cycle is:

New
 ↓
Assigned
 ↓
Open
 ↓
Fixed
 ↓
Retest
 ↓
Verified
 ↓
Closed

Possible alternate states:

Rejected
Duplicate
Deferred
Reopened
Not a Bug
17. Entry Criteria

Testing can begin when:

Requirements are available and reviewed.
Test environment is available.
Application build is deployed.
Major application modules are accessible.
Test data is available.
Test scenarios are prepared.
Test cases are reviewed.
Required testing tools are available.
18. Exit Criteria

Testing can be considered complete when:

Planned test cases have been executed.
Critical test cases have passed.
Critical and high-severity defects are resolved or formally accepted.
Failed test cases have been analyzed.
Retesting is completed for fixed defects.
Regression testing is completed.
Test execution results are documented.
Test summary report is prepared.
RTM is updated.
19. Suspension Criteria

Testing may be temporarily suspended when:

Application is unavailable.
Critical functionality is completely blocked.
Test environment is unavailable.
Major build instability prevents meaningful execution.
Required test data is unavailable.
A critical defect blocks the majority of test cases.
20. Resumption Criteria

Testing will resume when:

A stable application build is available.
Blocking defects are fixed or an approved workaround is provided.
Test environment is restored.
Required test data is available.
Affected test cases can be executed successfully.
21. Deliverables

The following testing deliverables will be maintained:

Requirements Document
        ↓
Test Plan
        ↓
Test Scenarios
        ↓
Test Cases
        ↓
Test Data
        ↓
Requirement Traceability Matrix
        ↓
Defect Reports
        ↓
Test Execution Report
        ↓
Test Summary Report
22. Roles and Responsibilities
Role	Responsibility
QA/Test Engineer	Requirement analysis, test design, execution, defect reporting, retesting and regression
Developer	Defect investigation and resolution
Business/Stakeholder	Requirement clarification and acceptance
QA Lead	Test planning, review and test status tracking

For this portfolio project, the testing activities are demonstrated from the perspective of a Manual Test Engineer.

23. Risks
Risk	Impact	Mitigation
Unstable application build	High	Perform smoke testing before detailed execution
Environment unavailable	High	Maintain a stable test environment
Requirement changes	Medium	Review and update test cases
Insufficient test data	Medium	Prepare test data before execution
Critical defect	High	Prioritize critical defects
Browser-specific issue	Medium	Perform cross-browser testing
Third-party dependency failure	Medium	Document dependency-related failures separately
24. Assumptions

The following assumptions are made:

The application is available for testing.
Requirements are sufficiently defined.
Test users can be created.
Product data is available.
Checkout functionality is available in the test environment.
Test environment is representative of supported application behavior.
Required browser versions are available.
Defects can be reported and tracked.
Test data can be created or reset when required.
25. Traceability Approach

Each requirement will be mapped to one or more test cases using the Requirement Traceability Matrix.

Example:

REQ-LOGIN-001
      ↓
TS-LOGIN-001
      ↓
TC-LOGIN-001
      ↓
Execution Result
      ↓
Defect ID (if applicable)

The RTM will be created after test scenarios and test cases are finalized.

26. Test Execution Approach

Each test case will be executed using the following process:

Read Preconditions
       ↓
Prepare Test Data
       ↓
Execute Test Steps
       ↓
Compare Actual vs Expected Result
       ↓
Record Status
       ↓
Report Defect if Failed
       ↓
Retest after Fix
       ↓
Update Final Status

Test case statuses:

Not Executed
Pass
Fail
Blocked
Not Applicable
27. Metrics

The following metrics will be tracked during test execution.

Test Case Metrics
Total Test Cases
Executed Test Cases
Passed Test Cases
Failed Test Cases
Blocked Test Cases
Not Applicable Test Cases
Defect Metrics
Total Defects
Critical Defects
High Defects
Medium Defects
Low Defects
Open Defects
Closed Defects
Reopened Defects
Coverage Metrics
Requirement Coverage
Test Case Coverage
Functional Coverage
Regression Coverage
28. Test Closure

Test closure activities will include:

Completing planned test execution.
Verifying critical defects are resolved or accepted.
Completing regression testing.
Updating RTM.
Preparing test execution metrics.
Preparing the test summary report.
Documenting known issues.
Recording lessons learned.
Archiving final testing documentation.
29. Final Testing Flow

The complete testing process for this project is:

Requirement Analysis
        ↓
Test Planning
        ↓
Test Scenario Design
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
Regression Testing
        ↓
Defect Reporting
        ↓
Defect Retesting
        ↓
Regression Verification
        ↓
Test Closure

