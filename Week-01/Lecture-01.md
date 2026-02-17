# Lecture 1  
## Course Overview and the Need for Databases

## The Importance of Database Management Systems and the Evolution from File Systems

---

## Core Concepts

### Definition and Purpose of DBMS
A Database Management System (DBMS) is a collection of interrelated data along with programs to access and manipulate that data efficiently.

Its primary goal is to provide a convenient and efficient environment for managing enterprise information.

### Characteristics of Database Applications
Database systems:
- Handle large volumes of data
- Support multiple users
- Are used in banking, airlines, retail, manufacturing, and HR systems

### Transition from File Systems
Before DBMS, enterprises relied on file systems.

Major drawbacks of file systems:
- Data redundancy
- Data inconsistency
- Integrity problems
- No proper concurrency control
- Difficult atomic updates

---

## Key Definitions

- **DBMS**: Software to manage interrelated data.
- **Enterprise Information**: Data related to an organization.
- **Data Redundancy**: Duplication of the same data in multiple files.
- **Data Inconsistency**: Conflicting versions of the same data.
- **Atomicity**: An operation either completes fully or does not execute at all.

---

## Important Examples

- Banking systems handling distributed transactions
- University databases managing students and courses
- Fund transfer where money must not disappear during failure

---

## File System vs DBMS

| File System Problem        | DBMS Solution                  |
|----------------------------|--------------------------------|
| Data Redundancy            | Centralized data control       |
| Integrity Problems         | Integrity constraints          |
| Uncontrolled Concurrency   | Concurrency control manager    |

---

## Real-World Analogy

Small data → Excel sheet  
Enterprise-scale data → DBMS

---

## Common Mistakes

- Believing file systems are sufficient for large enterprises  
- Thinking redundancy only wastes space  
  Redundancy mainly causes inconsistency

---

## Exam Questions

1. List three drawbacks of file systems.
2. Define atomicity with an example.
3. Why is concurrency control necessary?
4. Differentiate redundancy and inconsistency.
5. What are integrity constraints?
