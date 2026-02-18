# Lecture 9: Intermediate SQL (Part 1)

## 1. Overview
This lecture covers joins, views, and transactions.

## 2. Key Concepts

- Inner join
- Left outer join
- Right outer join
- Full outer join
- Views
- Transactions

## 3. Important Definitions

Natural Join  
Automatically joins on common attribute names.

Left Outer Join  
Preserves all tuples from left relation.

Materialized View  
View stored physically.

Transaction  
Logical unit of work.

## 4. Detailed Explanation

Natural Join:

    select *
    from course natural join prereq;

Left Outer Join:

    select *
    from course
    natural left outer join prereq;

Create View:

    create view faculty as
    select ID, name, dept_name
    from instructor;

## 5. Important Rules

- View is updatable if:
  - Single relation in from
  - No aggregates
  - No group by
- Transactions ensure atomicity.

## 6. Common Mistakes

- Misusing natural join.
- Assuming all views are updatable.

## 7. Exam-Oriented Questions

Short Answer
1. Types of outer joins?
2. What is materialized view?

Long Answer
1. Compare inner and outer join.
2. Conditions for updatable view.

Conceptual
1. Importance of transactions?
2. Natural join vs join using on?
