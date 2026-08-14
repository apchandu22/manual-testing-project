# API Defect Examples

> All examples are synthetic portfolio defects.

## API-BUG-001 – Create Order Returns 500 for Valid Payload

| Field | Details |
|---|---|
| Module | Checkout / Order |
| Endpoint | `POST /orders` |
| Severity | High |
| Priority | P1 |
| Environment | QA |
| Preconditions | Authenticated user with valid cart |
| Expected | 201 Created with order ID |
| Actual | 500 Internal Server Error |
| Reproducibility | 3/3 |

### Steps

1. Authenticate using a valid test account.
2. Add a valid product to cart.
3. Submit a valid order payload.
4. Send `POST /orders`.
5. Observe response.

### QA Evidence

- Request payload validated against the API contract.
- Required fields were present.
- Response returned HTTP 500.
- No sensitive production data included.

### Expected Fix Validation

Retest the same payload, then execute checkout/order regression scenarios.

---

## API-BUG-002 – Unauthorized User Can Access Another Order

| Field | Details |
|---|---|
| Module | Order Management |
| Endpoint | `GET /orders/{orderId}` |
| Severity | Critical |
| Priority | P1 |
| Expected | 403/404 without exposing another user's order |
| Actual | 200 response containing unauthorized order data |

### Security-Relevant Functional Observation

This example demonstrates authorization validation. It is **not** a penetration-testing exercise. The portfolio only documents the expected functional authorization behavior.

### Retest

Verify that an authenticated user can access their own order but cannot retrieve another user's order by changing the resource ID.

---

## API-BUG-003 – Negative Cart Quantity Accepted

| Field | Details |
|---|---|
| Module | Cart |
| Endpoint | `PUT /cart/{cartId}` |
| Severity | High |
| Priority | P1 |
| Expected | 400/422 validation error |
| Actual | 200 response and negative quantity accepted |

### Steps

1. Create a valid cart.
2. Send quantity `-1`.
3. Submit update request.
4. Verify response and cart data.

### Impact

Invalid business data can enter the cart workflow and may affect totals and checkout behavior.

### Retest

Validate zero, negative, minimum valid and maximum valid quantities, followed by cart and checkout regression.
