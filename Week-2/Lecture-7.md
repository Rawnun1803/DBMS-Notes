# Lecture 7: Introduction to SQL (Part 2)

## 1. Overview
This lecture discusses advanced SQL features including string matching, ordering, set operations, aggregate functions, and grouping.

## 2. Key Concepts

String Matching
- like operator
- % matches any substring
- _ matches single character

Set Operations
- union
- intersect
- except
- union all retains duplicates

Aggregate Functions
- avg
- min
- max
- sum
- count

Group By
Applies aggregate functions to groups of tuples.

## 3. Important Definitions

Cartesian Product  
All possible combinations of tuples from two relations.

Null Value  
Represents unknown or missing information.

Equi-Join  
Join based on equality of attributes.

## 4. Detailed Explanation

Ordering Example:

    select *
    from instructor
    order by salary desc, name asc;

Aggregation Example:

    select dept_name, avg(salary)
    from instructor
    group by dept_name;

Grouping Rule  
Every attribute in select that is not aggregated must appear in group by.

## 5. Important Rules

- count(*) counts all rows.
- count(attribute) ignores null values.
- Aggregate functions ignore null except count(*).

## 6. Common Mistakes

- Forgetting grouping rule.
- Misunderstanding null handling.
- Assuming string comparison is always case-insensitive.

## 7. Exam-Oriented Questions

Short Answer
1. Difference between count(*) and count(attribute)?
2. What are wildcards in like?

Long Answer
1. Explain group by with example.
2. Explain Cartesian product.

Conceptual
1. How are nulls treated in aggregates?
2. Purpose of as clause?
