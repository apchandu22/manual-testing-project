# 🔗 Requirements Traceability Matrix (RTM)

## Purpose

The RTM ensures that business requirements are covered by test scenarios and test cases and that execution status can be traced back to requirements.

| Requirement ID | Requirement | Scenario ID | Test Case IDs | Priority | Coverage |
|---|---|---|---|---|---|
| REQ-LOGIN-001 | User shall be able to securely log in and log out | TS-LOGIN-001 | TC-LOGIN-001, TC-LOGIN-002, TC-LOGIN-003, TC-LOGOUT-001 | High | Covered |
| REQ-SEARCH-001 | User shall be able to search products | TS-SEARCH-001 | TC-SEARCH-001, TC-SEARCH-002 | High | Covered |
| REQ-CART-001 | User shall add, update and remove cart items | TS-CART-001 | TC-CART-001, TC-CART-002, TC-CART-003 | High | Covered |
| REQ-CHECKOUT-001 | User shall complete checkout using a valid address | TS-CHECKOUT-001 | TC-CHECKOUT-001 | Critical | Covered |
| REQ-PAY-001 | Payment processing shall handle success and failure correctly | TS-PAY-001 | TC-PAY-001, TC-PAY-002 | Critical | Covered |
| REQ-ORDER-001 | User shall view successfully placed orders | TS-ORDER-001 | TC-ORDER-001 | High | Covered |

## Traceability Flow

```text
Business Requirement
        ↓
Test Scenario
        ↓
Test Case
        ↓
Execution Result
        ↓
Defect (if applicable)
        ↓
Retest / Regression
```

## Coverage Review

- Every critical business requirement has at least one test case.
- Negative scenarios are included for key workflows.
- Failed test cases must reference the related defect ID.
- Requirement coverage is reviewed before release sign-off.
