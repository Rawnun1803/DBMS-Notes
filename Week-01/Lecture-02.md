# Lecture 2  
## DBMS Fundamentals and Data Abstraction

## Levels of Abstraction, Data Models, and Database Languages

---

## Core Concepts

### Levels of Abstraction

1. Physical Level  
   Describes how data is stored.

2. Logical Level  
   Describes what data is stored and relationships.

3. View Level  
   Shows only required data to users.

---

### Schema vs Instance

- **Schema**: Structure or design of database.
- **Instance**: Actual data at a given time.

Schema is like a blueprint.  
Instance is like the actual building.

---

### Physical Data Independence

Ability to change physical storage without affecting logical schema.

---

### Data Models

Tools to describe:
- Data
- Relationships
- Constraints

---

### Database Languages

- **DDL**: Defines schema (CREATE, ALTER)
- **DML**: Manipulates data (SELECT, INSERT, UPDATE)
- **SQL**: Most widely used query language

---

## Key Definitions

- Physical Level
- Logical Level
- View Level
- Metadata
- SQL

---

## Example

```sql
CREATE TABLE instructor (
  id INT,
  name VARCHAR(20),
  salary INT
);

---

## Integrity Constraint Example

An account balance must not fall below a specified minimum value.

This rule ensures data integrity by preventing invalid updates.

---

## Abstraction Diagram

Database abstraction is organized into three levels:

1. View Level  
   What the end user or application sees.

2. Logical Level  
   What data is stored and the relationships between data.

3. Physical Level  
   How the data is actually stored on disk.

---

## Common Mistakes

- Confusing Physical Data Independence with Logical Data Independence  
  Physical data independence means changes in storage structure do not affect the logical schema.

- Thinking SQL can solve every computational problem  
  SQL is not computationally complete and often needs to be embedded within general-purpose programming languages.

---

## Exam Questions

1. Explain the three levels of data abstraction in a DBMS.
2. Differentiate between a database schema and a database instance.
3. What is Physical Data Independence and why is it important?
4. What is the role of the DDL compiler in a DBMS?
5. Compare pure query languages with commercial query languages.

