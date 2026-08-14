# API Regression Checklist

## Authentication

- [ ] Valid login
- [ ] Invalid credentials
- [ ] Missing token
- [ ] Invalid/expired token
- [ ] Logout/session behavior

## Product

- [ ] Product list
- [ ] Product details
- [ ] Invalid product ID
- [ ] Search
- [ ] Empty/no-result search

## Cart

- [ ] Add item
- [ ] Update quantity
- [ ] Minimum quantity
- [ ] Maximum quantity
- [ ] Zero/negative quantity rejection
- [ ] Remove item
- [ ] Cart totals

## Checkout / Order

- [ ] Valid order
- [ ] Missing required field
- [ ] Invalid address
- [ ] Order total
- [ ] Duplicate submission behavior
- [ ] Order confirmation
- [ ] Order details
- [ ] Order history

## Cross-API Validation

- [ ] Token chaining
- [ ] Product ID chaining
- [ ] Cart ID chaining
- [ ] Order ID chaining
- [ ] UI/API data consistency
- [ ] Response schema consistency
- [ ] Error schema consistency

## Exit

- [ ] Critical APIs pass
- [ ] High-severity defects reviewed
- [ ] Failed cases retested
- [ ] Regression completed
- [ ] Test report updated
