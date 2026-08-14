# API Test Execution Report

## 1. Execution Summary

| Metric | Result |
|---|---:|
| Total API Test Cases | 30 |
| Executed | 30 |
| Passed | 25 |
| Failed | 3 |
| Blocked | 2 |
| Pass Rate | 83.33% |
| Critical Defects | 1 |
| High Defects | 2 |

> These are synthetic portfolio metrics, not production measurements.

## 2. Execution Coverage

- Authentication
- Authorization
- Product APIs
- Search APIs
- Cart APIs
- Checkout/order APIs
- Positive testing
- Negative testing
- Boundary validation
- Response validation
- API chaining
- Regression testing

## 3. Failed Tests

| Test Case | Result | Defect |
|---|---|---|
| API-TC-016 | Fail | API-BUG-001 |
| API-TC-020 | Fail | API-BUG-002 |
| API-TC-015 | Fail | API-BUG-003 |

## 4. Blocked Tests

Blocked scenarios are dependent on unavailable downstream/test-environment behavior. Blocked tests should be re-executed once the dependency is available.

## 5. QA Assessment

The critical authorization defect and high-impact checkout/cart defects require attention before release. Retesting should be followed by impacted API regression.

## 6. Closure Criteria

- Failed tests retested after fixes.
- Critical/high defects resolved or formally accepted.
- API regression completed.
- Execution results updated.
- Remaining risks communicated.
