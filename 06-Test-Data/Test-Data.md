# 🧾 Test Data

## Purpose

Define reusable synthetic data for manual, API and integration testing.

| Data Type | Example | Usage |
|---|---|---|
| Valid User | qa.user@example.test | Login and checkout |
| Invalid User | invalid.user@example.test | Negative authentication |
| Product | PROD-1001 | Search/cart/order validation |
| Quantity | 1, 2, 10 | Boundary and cart validation |
| Address | 100 Test Street, Bengaluru | Checkout |
| Invalid Address | Missing mandatory fields | Negative checkout |
| Payment Success | Synthetic approved response | Positive payment |
| Payment Failure | Synthetic declined response | Negative payment |
| Order ID | ORD-2026-10001 | Order-history validation |

## Data Rules

- Use synthetic data only.
- Never store real customer credentials, payment information, tokens or production identifiers.
- Reset test data between independent end-to-end executions where required.
- Mask sensitive values in screenshots and logs.
