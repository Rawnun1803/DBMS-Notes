# Lecture-03.md

```markdown
# Lecture 3  
## Database Engine and Internals

## Internal Architecture and the Database Engine

---

## Core Components

### 1. Storage Manager
Handles:
- File organization
- Indexing
- Hashing

### 2. Query Processor
- Parses SQL
- Converts to relational algebra
- Optimizes query
- Executes plan

### 3. Transaction Manager
Ensures:
- Consistency
- Recovery
- Concurrency control

---

## Query Processing Steps

1. Query Input
2. Parsing
3. Translation to relational algebra
4. Optimization
5. Execution
6. Result Output

---

## Key Definitions

- Storage Manager
- Query Optimizer
- Transaction
- DBA
- Naive User

---

## Examples

- Two users booking last train seat
- Power failure during transaction
- Query optimization rewriting SQL

---

## Persistent vs Transient Data

Programs → transient data  
Databases → persistent data

---

## Common Mistakes

- Thinking DBAs manage daily data entry
- Assuming queries run exactly as written

---

## Exam Questions

1. Three major DBMS components.
2. Storage manager responsibilities.
3. Steps in query processing.
4. Define transaction.
5. Types of database users.
