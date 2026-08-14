# 🔌 API Testing – Postman

## Objective

Validate backend APIs supporting login, product search, cart, checkout and order workflows.

## API Test Coverage

| API | Method | Validation |
|---|---|---|
| Login | POST | Status code, token, response schema, invalid credentials |
| Product Search | GET | Status code, response time, result data |
| Add to Cart | POST | Status code, product/quantity persistence |
| Update Cart | PUT | Updated quantity and totals |
| Create Order | POST | Order ID, status and response schema |
| Order Details | GET | Correct order information and authorization |

## Postman Checks

- HTTP status codes
- Response body validation
- Required fields
- Headers
- Authentication/token handling
- Negative responses
- Response time
- Data consistency between API and UI
- Duplicate request behavior

## Example Assertions

```javascript
pm.test("Status code is successful", function () {
    pm.expect(pm.response.code).to.be.oneOf([200, 201]);
});

pm.test("Response contains required field", function () {
    const body = pm.response.json();
    pm.expect(body).to.have.property("id");
});
```

## API + UI Validation

For checkout defects, QA can compare the UI result with API responses and database/application evidence to determine whether the issue originates in the frontend, service layer or downstream integration.

> Endpoints, payloads and responses in this repository are illustrative and contain no production credentials or customer data.
