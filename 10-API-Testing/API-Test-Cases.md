# API Test Cases

| TC ID | Scenario | Request | Expected Result | Priority |
|---|---|---|---|---|
| API-TC-001 | Valid login | Valid username/password | 200/201; token returned; schema valid | P1 |
| API-TC-002 | Invalid password | Valid user + invalid password | 401/expected auth error; no token | P1 |
| API-TC-003 | Missing login field | Omit password | 400/422 validation error | P1 |
| API-TC-004 | Missing token | Protected GET without Authorization | 401 | P1 |
| API-TC-005 | Invalid token | Bearer invalid token | 401 | P1 |
| API-TC-006 | Product list | GET product endpoint | 200; valid array/schema | P2 |
| API-TC-007 | Valid product ID | GET valid ID | 200; correct product data | P2 |
| API-TC-008 | Invalid product ID | GET invalid ID | 404/expected error schema | P2 |
| API-TC-009 | Search keyword | Valid query | 200; matching products | P2 |
| API-TC-010 | No-result search | Unknown keyword | 200/expected empty-result response | P2 |
| API-TC-011 | Add cart | Valid product + quantity | 200/201; cart ID/data returned | P1 |
| API-TC-012 | Invalid cart product | Unknown product ID | 400/404; clear error | P1 |
| API-TC-013 | Update quantity | Valid cart ID + quantity | 200; quantity/total updated | P1 |
| API-TC-014 | Zero quantity | quantity=0 | 400/422; validation error | P1 |
| API-TC-015 | Negative quantity | quantity=-1 | 400/422; validation error | P1 |
| API-TC-016 | Create order | Valid checkout payload | 201; order ID and total returned | P1 |
| API-TC-017 | Missing address | Required address omitted | 400/422 | P1 |
| API-TC-018 | Duplicate order | Same idempotency/reference where supported | Duplicate is prevented/handled | P1 |
| API-TC-019 | Get order | Valid order ID + authorized user | 200; correct order data | P1 |
| API-TC-020 | Unauthorized order access | Another user's order ID | 403/404; no data leakage | P1 |
| API-TC-021 | Malformed JSON | Broken JSON body | 400/expected error | P2 |
| API-TC-022 | Wrong method | Unsupported method | 405/expected error | P2 |
| API-TC-023 | Wrong content type | Invalid Content-Type | 400/415/expected error | P2 |
| API-TC-024 | Required response field | Successful API response | Required fields exist | P1 |
| API-TC-025 | Response time | Normal request | Meets agreed threshold | P2 |
| API-TC-026 | Token chaining | Login → token variable | Token captured and reused | P1 |
| API-TC-027 | Product chaining | Product → cart | Product ID passed correctly | P1 |
| API-TC-028 | Order chaining | Create order → details | Order ID passed correctly | P1 |
| API-TC-029 | Regression | Critical endpoint suite | No unexpected regression | P1 |
| API-TC-030 | Error schema | Invalid request | Consistent error structure | P2 |

## Test Case Design Coverage

Each case should validate, where applicable:

- Request URL and HTTP method
- Path/query parameters
- Headers and authentication
- Request payload
- Status code
- Response body
- Required fields and data types
- Business rules
- Error response
- Response time
- Data consistency
- Defect evidence
