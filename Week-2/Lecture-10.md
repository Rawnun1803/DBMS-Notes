# Lecture 10: Intermediate SQL (Part 2)

## 1. Overview
This lecture covers advanced integrity constraints, referential integrity actions, SQL data types, and authorization mechanisms.

## 2. Key Concepts

- Check constraint
- Unique constraint
- Referential integrity actions
- User-defined types
- Authorization

## 3. Important Definitions

Check Clause  
Ensures attribute satisfies condition.

Referential Integrity  
Foreign key must reference existing primary key.

Privilege  
Permission to perform an action.

## 4. Detailed Explanation

Check Constraint Example:

    check (semester in (Fall, Winter, Spring, Summer));

Referential Integrity Actions:
- cascade
- set null
- set default

Example:

    foreign key (dept_name)
    references department
    on delete cascade
    on update cascade;

Unique Constraint  
Allows null values but enforces uniqueness.

## 5. Important Rules

- Primary key = unique + not null.
- Unique allows null.
- Foreign key must match referenced primary key.

## 6. Common Mistakes

- Violating foreign key without cascade.
- Confusing type and domain.

## 7. Exam-Oriented Questions

Short Answer
1. Primary key vs unique?
2. What is referential integrity?

Long Answer
1. Explain referential integrity actions.
2. Explain SQL authorization.

Conceptual
1. When to use unique instead of primary key?
2. Role of check clause?
