# 🔁 Regression Testing

## Objective

Verify that new fixes or changes do not break existing business-critical functionality.

## Regression Scope

| Area | Regression Checks |
|---|---|
| Login | Valid/invalid login, session, logout |
| Search | Search, filters, sorting, no-result behavior |
| Cart | Add, update, remove, totals |
| Checkout | Address, summary and navigation |
| Payment | Success, failure and retry behavior |
| Orders | Confirmation, history and details |

## Risk-Based Regression

### P0 – Critical

Checkout, payment and order creation.

### P1 – High

Login, cart and product search.

### P2 – Medium

Secondary UI and usability scenarios.

## Retest vs Regression

**Retesting:** Verify the specific failed test case after the defect is fixed.

**Regression:** Execute related existing functionality to confirm the fix did not introduce side effects.

## Exit Criteria

- Critical regression cases passed.
- No unresolved blocker/critical defects.
- High-severity issues reviewed with stakeholders.
- Test results documented.
