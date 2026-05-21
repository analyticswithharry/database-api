# Database API Lab

Design and implement persistence-focused APIs with safe queries, transactions, and performance awareness.

## Why this lab matters

Most business APIs are database APIs in disguise. Correctness, consistency, and speed all depend on your data layer design choices.

## Core concepts to master

- Entity modeling and relationship mapping
- Migrations and schema evolution
- Query safety and parameterized statements
- Transaction design and rollback behavior
- Pagination, indexing, and query performance tuning

## Suggested Stack

- Node.js + Prisma/Sequelize/Knex or Python + SQLAlchemy
- PostgreSQL (or SQLite for local learning)

## Practical endpoints for this lab

- `GET /api/health` (starter)
- `GET /api/lesson` (starter)
- `POST /api/demo` (starter)
- CRUD endpoints for one domain (products/orders/users)

## Learning roadmap

1. Define schema and relationships
2. Add migrations and seed data
3. Implement CRUD with validation
4. Add filtering/sorting/pagination patterns
5. Add transaction-based operations
6. Measure and optimize slow queries

## Suggested mini implementation

- Entities: users, categories, products, orders
- Operations: CRUD + aggregate endpoints
- Transaction demo: order create + inventory decrement

## Common pitfalls

- SQL injection through dynamic query strings
- Missing indexes on frequent filters
- N+1 queries from naive ORM usage
- Partial writes due to missing transaction boundaries

## Validation checklist

- [ ] Migrations run cleanly
- [ ] CRUD works with validation errors handled
- [ ] Transactional flow tested with rollback
- [ ] Pagination and sort controls implemented
- [ ] Query performance measured on sample dataset
