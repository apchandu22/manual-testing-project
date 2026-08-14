# API Test Scenarios

| ID | Module | Scenario | Type | Priority |
|---|---|---|---|---|
| API-SC-001 | Login | Login with valid credentials | Positive | P1 |
| API-SC-002 | Login | Login with invalid credentials | Negative | P1 |
| API-SC-003 | Login | Login without required fields | Negative | P1 |
| API-SC-004 | Auth | Access protected API without token | Negative | P1 |
| API-SC-005 | Auth | Access API with invalid/expired token | Negative | P1 |
| API-SC-006 | Products | Retrieve product list | Positive | P2 |
| API-SC-007 | Products | Retrieve product using valid ID | Positive | P2 |
| API-SC-008 | Products | Retrieve product using invalid ID | Negative | P2 |
| API-SC-009 | Search | Search using valid keyword | Positive | P2 |
| API-SC-010 | Search | Search with no matching keyword | Negative | P2 |
| API-SC-011 | Cart | Add valid product to cart | Positive | P1 |
| API-SC-012 | Cart | Add invalid product to cart | Negative | P1 |
| API-SC-013 | Cart | Update valid quantity | Positive | P1 |
| API-SC-014 | Cart | Validate zero/negative quantity | Boundary | P1 |
| API-SC-015 | Cart | Remove cart item | Positive | P1 |
| API-SC-016 | Order | Create order with valid payload | Positive | P1 |
| API-SC-017 | Order | Create order with missing required data | Negative | P1 |
| API-SC-018 | Order | Duplicate order submission | Negative | P1 |
| API-SC-019 | Order | Retrieve order details | Positive | P1 |
| API-SC-020 | Order | Access another user's order | Authorization | P1 |
| API-SC-021 | Validation | Malformed JSON payload | Negative | P2 |
| API-SC-022 | Validation | Unsupported HTTP method | Negative | P2 |
| API-SC-023 | Validation | Invalid Content-Type | Negative | P2 |
| API-SC-024 | Response | Validate required response fields | Functional | P1 |
| API-SC-025 | Response | Validate response time threshold | Non-functional check | P2 |
| API-SC-026 | Chaining | Capture token and reuse in next request | Integration | P1 |
| API-SC-027 | Chaining | Capture product ID for cart request | Integration | P1 |
| API-SC-028 | Chaining | Capture order ID and verify order | Integration | P1 |
| API-SC-029 | Regression | Execute critical API regression suite | Regression | P1 |
| API-SC-030 | Error Handling | Validate error response structure | Negative | P2 |
