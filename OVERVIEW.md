# SQL Overview

## What is SQL?
**SQL (Structured Query Language)** is used to communicate with a database. It is a **declarative language**, meaning we specify *what* we want to retrieve or manipulate, not *how* the database should perform those operations.

---

## What is a Database?
A database is a structured collection of data. It allows you to search, update, delete, and add data efficiently.

**Logical Structure:**
`Folder` ➔ `Multiple Tables` ➔ `Rows and Columns` ➔ `Data`

---

## Example: Student Database

### Table 1: Student
| Email | Name | Age | City |
| :--- | :--- | :--- | :--- |
| `[EMAIL_ADDRESS]` | Srinibas | 25 | HYD |
| `[EMAIL_ADDRESS]` | Rahul | 26 | HYD |

### Table 2: Course
| Course ID | Course Name | Duration |
| :--- | :--- | :--- |
| 1 | Python | 3 Months |
| 2 | Java | 3 Months |

### Table 3: Student_Course
| Email | Course ID | Fee |
| :--- | :--- | :--- |
| `[EMAIL_ADDRESS]` | 1 | 10,000 |
| `[EMAIL_ADDRESS]` | 2 | 12,000 |

---

## Data Storage in a Server
- **Pages:** Data is stored in fixed-size blocks called **Pages**. A single page can contain thousands of rows.
- **Memory Management:** When data is requested, a specific page is transferred from the **Disk** to the **RAM**.
- **Indexing:** Indexes allow the database to search and retrieve data much faster.

### Terminology:
- **Table:** A collection of rows and columns.
- **Row:** Also known as a **Record**.
- **Column:** Also known as a **Field**.

---

## Types of Databases

### 1. Relational Databases (RDBMS)
Data is organized into multiple tables connected via unique keys (e.g., **Primary Key**).
- **Examples:** MySQL, PostgreSQL, Oracle, SQL Server.

### 2. NoSQL Databases
Can be relational or non-relational, often used for unstructured data.
- **Examples:** MongoDB, Cassandra, Redis.

---

## OLAP vs. OLTP

| Feature | OLAP (Online Analytical Processing) | OLTP (Online Transaction Processing) |
| :--- | :--- | :--- |
| **Primary Use** | Data analysis and reporting | Daily transaction processing |
| **Execution Speed** | Slower (complex queries) | Fast (simple operations) |
| **Data Source** | Historic data | Current, operational data |

---

## What is a Transaction?
A **Transaction** is a single logical unit of work that consists of one or more SQL statements. 
- It is a sequence of operations performed as a single unit.
- Follows **ACID** properties to ensure data integrity.
