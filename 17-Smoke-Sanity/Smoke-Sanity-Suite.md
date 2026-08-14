# 🚦 Smoke & Sanity Testing

## Smoke Testing

Smoke testing validates whether a new build is stable enough for detailed testing.

| ID | Check | Expected |
|---|---|---|
| SMK-001 | Application launches | Application opens successfully |
| SMK-002 | Login | Valid user can authenticate |
| SMK-003 | Product search | Search returns results |
| SMK-004 | Add to cart | Product is added |
| SMK-005 | Checkout navigation | User reaches checkout |
| SMK-006 | Order flow | Critical order workflow is available |

## Sanity Testing

Sanity testing focuses on a specific changed area after a targeted fix.

| ID | Changed Area | Validation |
|---|---|---|
| SAN-001 | Payment fix | Success/failure payment behavior |
| SAN-002 | Cart fix | Quantity and totals |
| SAN-003 | Search fix | Search and no-result behavior |

## Decision

- **Smoke Pass:** Proceed with detailed testing.
- **Smoke Fail:** Reject build and report blocking defect.
- **Sanity Pass:** Continue impacted regression.
- **Sanity Fail:** Reopen or reject the fix as appropriate.
