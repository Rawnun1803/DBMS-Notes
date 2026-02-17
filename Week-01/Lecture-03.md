# Lecture 3  
## Database Engine and Internals

---

## Core Components of a DBMS

A DBMS consists of three major components:

### 1. Storage Manager
Responsible for:
- File organization
- Indexing
- Data storage
- Disk management

---

### 2. Query Processor

Responsible for:
- Parsing SQL queries
- Translating them into relational algebra
- Optimizing execution plans
- Executing queries

---

### 3. Transaction Manager

Responsible for:
- Maintaining database consistency
- Handling concurrent access
- Recovery from failures

---

## Query Processing Steps

1. Query Input
2. Parsing and Syntax Checking
3. Translation to Relational Algebra
4. Query Optimization
5. Execution Plan Generation
6. Evaluation
7. Result Output

---

## Key Definitions

### Storage Manager
Interface between stored data and queries.

### Query Optimizer
Chooses the most efficient execution plan.

### Transaction
A sequence of operations performing a single logical task.

### Naive User
User who interacts through predefined applications.

### Database Administrator (DBA)
Person responsible for database security, backups, and maintenance.

---

## Examples

- Two users booking the last train seat  
- Power failure during a fund transfer  
- Query rewritten by optimizer for efficiency  

---

## Persistent vs Transient Data

Transient data:
- Temporary
- Exists during program execution

Persistent data:
- Stored permanently
- Survives system restarts

Databases manage persistent data.

---

## Common Mistakes

- Thinking DBAs handle routine data entry  
- Assuming SQL queries execute exactly as written  

---

## Exam Questions

1. Explain the three major components of a DBMS.
2. What are the responsibilities of the Storage Manager?
3. Describe the query processing steps.
4. Define a transaction.
5. List different types of database users.
