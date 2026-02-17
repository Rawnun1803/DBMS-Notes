# Lecture 5  
## Relational Algebra Operations

---

## Relational Algebra

A formal query language based on set theory.

Takes relations as input.
Produces relations as output.

---

## Fundamental Operators

- Select (sigma)
- Project (pi)
- Union
- Set Difference
- Cartesian Product

---

## Derived Operators

- Intersection
- Natural Join

---

## Examples

Select:
sigma salary > 80000 (instructor)

Project:
pi name, salary (instructor)

Natural Join:
Instructor join Department on dept_name

---

## Natural Join Steps

1. Cartesian product
2. Select matching attributes
3. Remove duplicate columns

---

## Aggregate Functions

- SUM
- AVG
- COUNT

---

## Common Mistakes

- Union on incompatible relations
- Forgetting projection removes duplicates
- Thinking intersection is fundamental

---

## Exam Questions

1. List fundamental operations.
2. Select vs Project.
3. Conditions for Union.
4. Natural Join vs Cartesian Product.
5. Aggregate operators.
