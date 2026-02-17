# Lecture 4  
## Foundations of the Relational Model and Keys

---

## Relational Model Basics

- Relation = Table
- Attribute = Column
- Tuple = Row

Relations are unordered sets.

---

## Domains

Each attribute has a domain.
Values must be atomic.

---

## Key Theory

- Superkey: Uniquely identifies tuple.
- Candidate Key: Minimal superkey.
- Primary Key: Selected candidate key.
- Foreign Key: References primary key of another table.
- Surrogate Key: Artificial identifier.

---

## Examples

Foreign Key:
Enrollment table referencing Student table.

Composite Key:
First Name + Last Name.

---

## Mathematical Definition

A relation r is a subset of:

D1 x D2 x ... x Dn

---

## Common Mistakes

- Assuming row order matters
- Using NULL as primary key
- Confusing composite and compound keys

---

## Exam Questions

1. Define relation, attribute, tuple.
2. What is domain?
3. Superkey vs Candidate key.
4. What is foreign key?
5. Procedural vs Declarative query languages.
