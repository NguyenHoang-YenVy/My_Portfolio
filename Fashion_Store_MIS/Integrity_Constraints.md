# Integrity Constraints

## Entity Integrity

- Each table uses a unique primary key that cannot be NULL.

## Referential Integrity

- Foreign key values must reference existing records in related tables to ensure data consistency.

## Domain Constraints

- Data values must satisfy predefined rules, such as valid email formats, non-negative salaries, supported payment methods, and valid payment statuses.


## Uniqueness Constraints

- Primary keys, customer emails, and phone numbers must be unique.

## Check Constraints

- Discount rates must be between 0% and 100%.
- Ordered quantities must be greater than zero and cannot exceed available inventory.