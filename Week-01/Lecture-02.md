# Lecture 2  
## DBMS Fundamentals and Data Abstraction

---

## Levels of Abstraction

To manage complexity, databases are organized into three abstraction levels:

### 1. View Level
- What the user sees
- Hides internal complexity
- Provides security and customization

### 2. Logical Level
- Describes what data is stored
- Defines relationships between data
- Used by database designers

### 3. Physical Level
- Describes how data is stored on disk
- Involves file structures and indexing

---

## Schema vs Instance

### Schema
The logical design or blueprint of the database.

### Instance
The actual data stored in the database at a particular time.

Schema rarely changes.  
Instance changes frequently.

---

## Physical Data Independence

The ability to modify physical storage without changing the logical schema or application programs.

Example:
Changing indexing technique should not affect SQL queries.

---

## Data Models

A data model provides tools to describe:

- Data
- Relationships
- Constraints

---

## Database Languages

### DDL (Data Definition Language)
Used to define structure.

Examples:
- CREATE
- ALTER
- DROP

Example:

CREATE TABLE instructor (
  id INT,
  name VARCHAR(20),
  salary INT
);

---

### DML (Data Manipulation Language)
Used to access and modify data.

Examples:
- SELECT
- INSERT
- UPDATE
- DELETE

---

## Integrity Constraint Example

An account balance must not fall below a specified minimum value.

This ensures correctness and consistency of data.

---

## Abstraction Diagram

View Level  
↓  
Logical Level  
↓  
Physical Level  

---

## Common Mistakes

- Confusing physical and logical data independence  
- Assuming SQL can solve every computational problem  

---

## Exam Questions

1. Explain the three levels of data abstraction.
2. Differentiate between schema and instance.
3. Define physical data independence.
4. What is the role of a DDL compiler?
5. Compare pure query languages with commercial query languages.