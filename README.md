## Project Description

This repository contains **30 practical SQL queries** commonly asked in technical interviews. The queries cover a wide range of SQL concepts, including table creation, data manipulation, filtering, aggregation, joins, and subqueries. It serves as a valuable resource for developers preparing for SQL-based interviews or seeking to enhance their database management skills.

---

## Key Concepts Covered

### **1. Basic SQL Operations**
- Table creation, deletion, and data insertion.
- Adding constraints like primary keys and foreign keys.

### **2. Data Querying**
- Selecting rows with filters and conditions.
- Using `DISTINCT`, `LIKE`, `BETWEEN`, and logical operators (`AND`, `OR`, `NOT`).
- Sorting and limiting results with `ORDER BY` and `LIMIT`.

### **3. Aggregation and Comparison**
- Finding minimum, maximum, and specific value ranges.
- Comparing rows with subqueries and conditional logic.

### **4. Joins**
- Writing queries with both implicit joins (comma-separated) and explicit joins (`JOIN`, `ON`).
- Combining data from multiple tables effectively.

### **5. Advanced Querying**
- Nested subqueries.
- Using `EXCEPT` (PostgreSQL specific).
- Complex filtering based on conditions.

---

## Problem Highlights and Examples

### **1. Create and Populate Tables**
- **Tables Created:**
  - `Employee`: Stores employee details like name, city, department, and salary.
  - `Department`: Lists departments available in the company.
  - `Company`: Contains details of companies and their revenue.

*Example: Creating the `Employee` table:*
```sql
CREATE TABLE Employee(
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(150) NOT NULL,
    city VARCHAR(150) NOT NULL,
    department_id INT NOT NULL,
    salary INT NOT NULL,
    FOREIGN KEY (department_id) REFERENCES department(id)
);
