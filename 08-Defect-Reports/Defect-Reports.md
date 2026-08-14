# 🐞 Defect Reports

## Defect Lifecycle

```text
New → Assigned → In Progress → Fixed → Ready for QA → Retest → Closed
                                      ↓
                                  Reopened
```

## DEF-001 – Order Created After Payment Failure

| Field | Details |
|---|---|
| Defect ID | DEF-001 |
| Jira Key | ECOM-101 |
| Module | Payment / Order |
| Severity | High |
| Priority | High |
| Environment | QA |
| Status | Retest |
| Reproducibility | 3/3 |
|
| Preconditions | Valid user and item in cart |

**Steps:**
1. Add an item to the cart.
2. Proceed to payment.
3. Submit a synthetic declined payment response.
4. Refresh Order History.

**Expected:** Payment failure is displayed and no order is created.

**Actual:** Payment failure is displayed, but an order record is temporarily created.

**Evidence:** Timestamp, order reference, application log entry and API response.

## DEF-002 – Cart Total Not Refreshed After Quantity Change

| Field | Details |
|---|---|
| Defect ID | DEF-002 |
| Jira Key | ECOM-102 |
| Module | Cart |
| Severity | Medium |
| Priority | High |
| Status | Closed |

**Expected:** Cart total reflects the updated quantity immediately.

**Actual:** Total remains stale until page refresh.

## DEF-003 – Search Results Timeout for Repeated Requests

| Field | Details |
|---|---|
| Defect ID | DEF-003 |
| Jira Key | ECOM-103 |
| Module | Product Search |
| Severity | High |
| Priority | High |
| Status | Open |

**Expected:** Search returns results within the agreed response threshold.

**Actual:** Repeated searches intermittently return a timeout.

## Defect Quality Checklist

- Clear summary
- Correct module and environment
- Preconditions
- Reproducible steps
- Expected vs actual result
- Severity and priority
- Build/version
- Evidence
- Related test case
- Retest result
