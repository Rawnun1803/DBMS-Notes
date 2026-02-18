# Lecture 8: Introduction to SQL (Part 3)

## 1. Overview
This lecture introduces nested subqueries and data modification commands including insert, delete, and update.

## 2. Key Concepts

- Nested subqueries
- Set comparison using some and all
- Correlated subqueries
- Conditional updates using case

## 3. Important Definitions

Subquery  
A query nested inside another query.

Set Membership (in)  
Checks whether a value belongs to a result set.

Correlation Variable  
Variable in subquery referencing outer query.

## 4. Detailed Explanation

Subquery Example:

    select course_id
    from section
    where year = 2009
    and course_id in (
        select course_id
        from section
        where year = 2010
    );

Set Comparison Example:

    select name
    from instructor
    where salary > all (
        select salary
        from instructor
        where dept_name = Biology
    );

Conditional Update:

    update instructor
    set salary = case
        when salary <= 100000 then salary * 1.05
        else salary * 1.03
    end;

## 5. Important Rules

- Single-value subqueries must return exactly one value.
- Insert-select subquery is evaluated fully before insertion.

## 6. Common Mistakes

- Using multi-row subquery with equality.
- Ignoring order of multiple updates.

## 7. Exam-Oriented Questions

Short Answer
1. What is a correlated subquery?
2. Explain some clause.

Long Answer
1. Explain case statement.
2. Explain subquery placements.

Conceptual
1. Why must insert-select be fully evaluated?
2. Explain subset testing using not exists.
