# Lecture 6: Introduction to SQL (Part 1)

## 1. Overview
This lecture introduces Structured Query Language (SQL), its historical background, schema definition using Data Definition Language (DDL), and the basic structure of queries using Data Manipulation Language (DML).

## 2. Key Concepts

### SQL Evolution
- Developed by IBM as SEQUEL under the System R project.
- Standardized by ANSI and ISO.
- Became the standard relational database query language.

### Data Definition Language (DDL)
Used to define:
- Relations
- Attributes
- Domain types
- Integrity constraints

### Data Manipulation Language (DML)
Used for:
- Querying data
- Inserting tuples
- Deleting tuples
- Updating tuples

### Integrity Constraints
Rules enforced to maintain data consistency:
- Primary Key
- Foreign Key
- Not Null

## 3. Important Definitions

Primary Key  
An attribute or set of attributes that uniquely identifies each tuple in a relation. It cannot contain null values.

Foreign Key  
An attribute that references the primary key of another relation.

Metadata  
Data describing the structure of the database, stored in the data dictionary.

Relation Instance  
The content of a relation at a specific point in time.

## 4. Detailed Explanation

### Create Table Command

    create table instructor (
        ID char(5),
        name varchar(20) not null,
        dept_name varchar(20),
        salary numeric(8,2),
        primary key (ID)
    );

Common domain types:
- char(n)
- varchar(n)
- numeric(p,d)
- int

### Basic Query Structure

Three main clauses:
- select
- from
- where

Example:

    select name
    from instructor
    where dept_name = Comp. Sci.
    and salary > 80000;

## 5. Important Rules

- Primary keys enforce uniqueness and not null automatically.
- select distinct removes duplicates.
- select all retains duplicates.
- delete removes tuples but keeps relation.
- drop removes entire relation.

## 6. Common Mistakes

- Confusing delete and drop.
- Inserting null into primary key.
- Forgetting distinct when duplicate elimination is required.

## 7. Exam-Oriented Questions

Short Answer
1. Difference between char and varchar?
2. What is metadata?

Long Answer
1. Explain table creation with constraints.
2. Explain SQL query structure.

Conceptual
1. Schema vs instance.
2. Why is metadata important?
