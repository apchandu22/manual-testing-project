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
