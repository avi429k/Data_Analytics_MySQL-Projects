[README.md](https://github.com/user-attachments/files/27099209/README.md)
# 🏫 school_db — MySQL Beginner Practice Project

A beginner-friendly SQL project demonstrating essential MySQL operations using a simple student management database.

---

## 📋 Overview

This project walks through the fundamental SQL commands every developer should know — from creating a database and table, to inserting, querying, updating, and deleting records, all the way to dropping the database.

---

## 🗄️ Database Structure

**Database:** `school_db`  
**Table:** `students`

| Column   | Type        | Description              |
|----------|-------------|--------------------------|
| `id`     | INT (PK)    | Unique student ID        |
| `name`   | VARCHAR(50) | Student's name           |
| `age`    | INT         | Student's age            |
| `course` | VARCHAR(50) | Enrolled course name     |

---

## 🚀 Concepts Covered

### 🏗️ Database & Table Setup
- `SHOW DATABASES` — List all databases
- `CREATE DATABASE` — Create a new database
- `USE` — Select a database
- `CREATE TABLE` — Define a new table
- `SHOW TABLES` — List tables in a database
- `DESCRIBE` — View the structure of a table

### ➕ Inserting Data
- `INSERT INTO ... VALUES` — Add multiple rows in a single statement

### 🔍 Querying Data
- `SELECT *` — Retrieve all columns
- `SELECT col1, col2` — Retrieve specific columns
- `WHERE` clause — Filter rows by condition (equality, comparison, ID lookup)

### ✏️ Updating Data
- `UPDATE ... SET ... WHERE` — Modify existing records
- `ALTER TABLE ... ADD PRIMARY KEY` — Add a primary key constraint to an existing table

### 🗑️ Deleting Data
- `DELETE FROM ... WHERE` — Remove a specific row
- `DROP TABLE` — Permanently delete a table
- `DROP DATABASE` — Permanently delete a database

---

## 📁 Sample Data

```sql
INSERT INTO students (id, name, age, course)
VALUES 
(101, 'Sahil',  24, 'MSC'),
(102, 'Ribani', 21, 'Diploma'),
(103, 'Ankita', 20, 'Diploma'),
(104, 'Arushi', 22, 'BSC');
```

---

## ▶️ How to Run

1. Open your MySQL client (MySQL Workbench, DBeaver, or the terminal).
2. Copy and paste the SQL script or run the `.sql` file:

```bash
mysql -u root -p < school_db.sql
```

3. Follow along with each section — the script is ordered top to bottom.

> ⚠️ **Note:** The script ends with `DROP TABLE` and `DROP DATABASE`, which permanently removes all data. Run these only when you're done exploring!

---

## 💡 Key Takeaways

- Always add a **Primary Key** to your tables for reliable `UPDATE` and `DELETE` operations.
- Use `WHERE` clauses carefully — omitting them in `UPDATE` or `DELETE` affects **every row**.
- `DROP` commands are **irreversible** — double-check before executing.

---

## 🛠️ Tech Stack

- **Database:** MySQL
- **Skill Level:** Beginner

---

## 📄 License

This project is open-source and free to use for learning purposes.
