# 🔌 API Testing Project – E-Commerce REST APIs

## 1. Project Overview

This project demonstrates an end-to-end **Manual API Testing** approach using **Postman** for an e-commerce REST API.

It covers API requirement analysis, test planning, positive/negative testing, authentication, request/response validation, JSON/schema checks, boundary testing, API chaining, environment variables, defect reporting, execution reporting and API-to-UI consistency validation.

> **Portfolio note:** This is a portfolio project. Credentials, tokens and customer information are never stored. Sample values are synthetic.

## 2. API Testing Objectives

- Validate APIs against business requirements.
- Verify HTTP methods and status codes.
- Validate headers, parameters and payloads.
- Validate response body and JSON structure.
- Verify mandatory and optional fields.
- Validate authentication and authorization.
- Verify positive and negative scenarios.
- Validate boundary and invalid inputs.
- Verify response time against agreed thresholds.
- Validate data consistency across dependent APIs.
- Chain APIs using Postman variables.
- Verify duplicate request behavior and idempotency where applicable.
- Validate error handling.
- Document defects with complete evidence.
- Support API regression after changes.

## 3. API Testing Scope

### In Scope

Authentication, users, products, search, cart, checkout/order workflows, request/response validation, status codes, headers, tokens, JSON validation, negative testing, boundary testing, API chaining, environment variables, response-time checks and regression testing.

### Out of Scope

Production API testing, destructive testing against live customer data, penetration testing, load/stress testing, infrastructure performance testing and payment gateway certification.

## 4. API Test Strategy

Testing follows a **requirement-based and risk-based approach**.

| Priority | API Area | Coverage |
|---|---|---|
| P1 | Authentication, Checkout/Order | Extensive positive, negative, authorization and regression testing |
| P2 | Cart, Product | Functional, validation, negative and integration testing |
| P3 | Search, User Profile | Functional and negative testing |

### API Testing Flow

```text
API Requirements
      ↓
Endpoint / Contract Review
      ↓
Test Scenario Design
      ↓
Test Case Design
      ↓
Environment & Test Data Setup
      ↓
Positive Testing
      ↓
Negative Testing
      ↓
Boundary / Validation Testing
      ↓
Authentication & Authorization
      ↓
API Chaining / Integration Testing
      ↓
Defect Reporting
      ↓
Retesting
      ↓
API Regression
      ↓
Test Summary
```

## 5. API Test Coverage

| Module | Method | Key Validation |
|---|---|---|
| Login | POST | Credentials, token, status, schema |
| Current User | GET | Authentication, user data, authorization |
| Product List | GET | Status, pagination, product fields |
| Product Details | GET | Valid/invalid product ID |
| Product Search | GET | Query, empty result, special characters |
| Add Cart | POST | Product ID, quantity, cart ID |
| Update Cart | PUT | Quantity, totals, consistency |
| Delete Cart | DELETE | Deletion behavior and response |
| Create Order | POST | Payload, order ID, total, status |
| Order Details | GET | Authorization and order data |
| Order History | GET | User-specific data and pagination |

## 6. HTTP Methods

| Method | Usage | Example |
|---|---|---|
| GET | Retrieve data | Product details |
| POST | Create/authenticate | Login / Create order |
| PUT | Update resource | Update cart |
| PATCH | Partial update | Update profile field |
| DELETE | Remove resource | Delete cart/item |

## 7. Status Code Validation

| Code | Expected Meaning | QA Validation |
|---:|---|---|
| 200 | Successful request | Response and business data are correct |
| 201 | Resource created | Created resource/ID is returned |
| 400 | Bad request | Invalid payload is rejected |
| 401 | Unauthorized | Missing/invalid authentication is rejected |
| 403 | Forbidden | Restricted resource is rejected |
| 404 | Not found | Invalid resource returns expected error |
| 409 | Conflict | Duplicate/conflicting request is handled |
| 422 | Validation error | Invalid business input is rejected |
| 429 | Too many requests | Rate-limit behavior is handled |
| 500 | Server error | Error is handled without sensitive leakage |

## 8. Request Validation

Validate URL, method, path/query parameters, headers, authorization, Content-Type, body, required/optional fields, data types, field lengths, null/empty values, special characters and duplicates.

## 9. Response Validation

Validate status code, response time, headers, Content-Type, JSON syntax, required fields, data types, field values, array/object structure, error structure, business rules and data consistency.

## 10. Authentication & Authorization Testing

### Authentication

- Valid credentials
- Invalid username/password
- Missing credentials
- Empty payload
- Expired token
- Invalid token
- Missing token

### Authorization

- Authenticated user accessing permitted resource
- Unauthenticated access to protected resource
- Access to another user's resource
- Insufficient permission
- Manipulated resource ID

## 11. Positive Testing

Examples include valid login, valid product retrieval, valid cart creation, valid quantity update and valid order creation.

## 12. Negative Testing

Examples include invalid credentials, missing fields, invalid IDs, negative/zero quantity, non-numeric quantity, invalid/missing token, malformed JSON, invalid Content-Type, unsupported methods and duplicate order submission.

## 13. Boundary Testing

Example for quantity allowed from **1–10**:

| Input | Expected |
|---:|---|
| 0 | Reject |
| 1 | Accept |
| 2 | Accept |
| 9 | Accept |
| 10 | Accept |
| 11 | Reject |

## 14. API Chaining

```text
Login
  ↓
Capture Token
  ↓
Get Product
  ↓
Create / Update Cart
  ↓
Create Order
  ↓
Capture Order ID
  ↓
Get Order Details
  ↓
Validate Order
```

Example:

```javascript
pm.environment.set("authToken", pm.response.json().token);
```

Next request:

```text
Authorization: Bearer {{authToken}}
```

## 15. Postman Test Scripts

### Status Code

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

### Response Time

```javascript
pm.test("Response time is below 2000 ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(2000);
});
```

### Required Field

```javascript
const body = pm.response.json();

pm.test("Response contains id", function () {
    pm.expect(body).to.have.property("id");
});
```

### Store ID for Chaining

```javascript
const body = pm.response.json();
pm.environment.set("productId", body.id);
```

### Content Type

```javascript
pm.test("Response is JSON", function () {
    pm.expect(pm.response.headers.get("Content-Type")).to.include("application/json");
});
```

## 16. Environment Variables

| Variable | Example | Purpose |
|---|---|---|
| `baseUrl` | `https://example.test` | Environment base URL |
| `username` | `qa_user@example.test` | Test account |
| `password` | `REPLACE_ME` | Environment secret |
| `authToken` | Runtime value | Authentication token |
| `productId` | Runtime value | Chained product ID |
| `cartId` | Runtime value | Chained cart ID |
| `orderId` | Runtime value | Chained order ID |

Never commit real credentials, tokens, API keys or customer data.

## 17. API + UI Validation

API testing should complement UI testing.

```text
UI shows order total
        ↓
GET Order API
        ↓
Compare API total
        ↓
Validate consistency
```

Validate product name, price, quantity, subtotal, tax, discount, total, order status and order ID.

## 18. Defect Reporting

An API defect should contain endpoint, method, environment, sanitized URL/payload, actual response, expected response, status code, reproduction steps, severity, priority, evidence and related test case.

See `API-Defect-Examples.md` for portfolio examples.

## 19. API Regression Strategy

Run API regression after API contract changes, backend deployment, authentication changes, database changes affecting API behavior, checkout/order changes, bug fixes and new integrations.

```text
Authentication
    ↓
Product
    ↓
Cart
    ↓
Checkout / Order
    ↓
Order History
```

## 20. Test Completion Criteria

- Planned API test cases executed.
- Critical APIs validated.
- Required negative scenarios covered.
- Authentication/authorization validated.
- Defects documented and retested.
- Regression completed.
- Critical blockers resolved or formally accepted.
- Execution results documented.
- Known risks communicated.

## 21. Project Deliverables

- API Test Strategy
- API Test Scenarios
- API Test Cases
- Postman Collection
- Postman Environment Template
- Test Scripts
- API Defect Examples
- API Execution Report
- API Regression Checklist
- API Testing README
