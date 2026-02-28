# Domain Glossary

## Core Entities
- **Product**: Logical grouping of articles. Has a name, category, and status (ACTIVE/INACTIVE).
- **Article**: Physical SKU with stock and price. Belongs to one Product. Has size and color attributes.
- **Order**: A customer purchase containing one or more order lines. Has lifecycle states.

## Value Objects
- **Money**: Amount + currency. Immutable. Used for prices and totals.
- **SKU**: Stock Keeping Unit identifier. Format: `{CATEGORY}-{ID}-{SIZE}-{COLOR}`.

## Order Lifecycle
DRAFT → PENDING → CONFIRMED → SHIPPED → DELIVERED
                → CANCELLED (from PENDING or CONFIRMED only)

## Invariant Business Rules
- An article cannot have negative stock
- An order can only be cancelled in PENDING or CONFIRMED status
- A product must have at least one article to be ACTIVE
- Order total is calculated from order lines, never stored directly
- Price changes do not affect existing confirmed orders
