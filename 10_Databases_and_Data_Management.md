# 10. Databases & Data Management

---

## What is a Database?

A database is an organized collection of structured data, managed by a Database Management System (DBMS). It enables efficient storage, retrieval, and management of data.

---

## Types of Databases

- **Relational (SQL):** Data organized in tables (MySQL, PostgreSQL, Oracle).
- **NoSQL:** Non-tabular, flexible schemas (MongoDB, Redis, Cassandra, Neo4j).
    - Key-Value
    - Document
    - Columnar
    - Graph

---

## Relational Database Concepts

- **Tables:** Rows and columns.
- **Primary Key:** Uniquely identifies each row.
- **Foreign Key:** Links rows between tables.
- **Normalization:** Remove redundancy, ensure data integrity.
- **ACID Properties:** Atomicity, Consistency, Isolation, Durability.

---

## NoSQL Database Concepts

- **Schema-less:** Flexible data models.
- **BASE Properties:** Basically Available, Soft state, Eventual consistency.
- **Sharding:** Distribute data across multiple servers.

---

## CRUD Operations

- **Create:** `INSERT`
- **Read:** `SELECT`
- **Update:** `UPDATE`
- **Delete:** `DELETE`

---

## Example SQL Queries

```sql
CREATE TABLE users (id INT PRIMARY KEY, name VARCHAR(50));
INSERT INTO users VALUES (1, 'Alice');
SELECT * FROM users WHERE id = 1;
UPDATE users SET name = 'Bob' WHERE id = 1;
DELETE FROM users WHERE id = 1;
```

---

## Indexing

- Speeds up data retrieval.
- Trade-off: increases write time and storage.

---

## Transactions

- All-or-nothing operations.
- Ensure data integrity.
- Use `BEGIN`, `COMMIT`, `ROLLBACK`.

---

## ORMs (Object-Relational Mappers)

- Map database tables to code objects (SQLAlchemy, Django ORM, Hibernate).
- Simplify data access, improve portability.

---

## Data Management Best Practices

- **Backups:** Regular, automated.
- **Security:** Access controls, encryption.
- **Monitoring:** Query performance, errors.
- **Scaling:** Sharding, replication, partitioning.
- **Consistency:** Use transactions and ACID for critical data.

---

## Database Design

- Requirements gathering.
- Entity-relationship diagrams (ERD).
- Normalization: 1NF, 2NF, 3NF.

---

## Interview Questions

1. Explain normalization and denormalization.
2. How do you prevent SQL injection?
3. What is a transaction and its properties?
4. Differences between SQL and NoSQL databases?
5. How would you optimize a slow query?

---

## References

- [SQLZoo](https://sqlzoo.net/)
- [MongoDB Docs](https://docs.mongodb.com/)
- [PostgreSQL Tutorial](https://www.postgresqltutorial.com/)
- [ACID vs BASE](https://en.wikipedia.org/wiki/ACID)

---

## Exercises

1. Design a relational schema for a library system.
2. Write SQL queries for CRUD operations on a "books" table.
3. Model a social network using a graph database.
4. Normalize a table with redundant data to 3NF.
5. Simulate a transaction and demonstrate rollback.

---

## Summary

Databases and data management are the backbone of all modern applications. Mastering them is essential for both backend and full-stack engineers.

---
