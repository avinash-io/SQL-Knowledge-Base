# SQL Basics

This README provides a brief overview of SQL basics, including syntax and examples for SELECT, INSERT, UPDATE, and DELETE statements, as well as SQL keywords like WHERE, ORDER BY, GROUP BY, and HAVING.

## SQL Syntax and Examples

### 1. SELECT Statement:

The SELECT statement is used to retrieve data from a database.

**Syntax:**

```sql
SELECT column1, column2, ...
FROM table_name;
```

Example:

```sql
SELECT * FROM employees;
```

This query retrieves all columns from the "employees" table.

### 2. INSERT Statement:

The INSERT statement is used to insert new records into a table.

**Syntax:**

```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

Example:

```sql
INSERT INTO employees (name, age, department)
VALUES ('John Doe', 30, 'IT');
```

### 3. UPDATE Statement:

The UPDATE statement is used to modify existing records in a table.

**Syntax:**

```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

Example:

```sql
UPDATE employees
SET age = 31
WHERE name = 'John Doe';
```

This query updates the "age" column of the employee named 'John Doe' in the "employees" table.

### 4. DELETE Statement:

The DELETE statement is used to remove records from a table.

**Syntax:**

```sql
DELETE FROM table_name
WHERE condition;
```

Example:

```sql
DELETE FROM employees
WHERE age > 60;
```

This query deletes records from the "employees" table where the age is greater than 60.

## SQL Keywords:

**1. WHERE:** Used to specify conditions while retrieving or modifying data.

Example:

```sql
SELECT * FROM employees WHERE department = 'IT';
```

This query retrieves all employees from the "IT" department.

**2. ORDER BY:** Used to sort the result set in ascending or descending order.

Example:

```sql
SELECT * FROM employees ORDER BY age DESC;
```

This query retrieves all employees and sorts them in descending order based on their age.

**3. GROUP BY:** Used to group rows that have the same values into summary rows.

Example:

```sql
SELECT department, COUNT(*) FROM employees GROUP BY department;
```

This query counts the number of employees in each department.

**4. HAVING:** Used with the GROUP BY clause to specify a condition on grouped items.

Example:

```sql
SELECT department, COUNT(_) FROM employees GROUP BY department HAVING COUNT(_) > 5;
```

This query retrieves departments with more than 5 employees.

These are the basic SQL syntax elements along with some examples. Practice these queries to become more familiar with SQL.
