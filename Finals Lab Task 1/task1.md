# FINALS LAB TASK 1
This Lab Task involves writing SQL queries, creating table structures, and developing relational schemas or ER diagrams.  To demonstrate the database's construction, the portfolio will also contain SQL copies of the database and table structures.

## Instructions

1. Create the *employees table*:
- Define **employee_id** as a UNIQUE INTEGER, AUTO_INCREMENT, and PRIMARY KEY.
- Define **employee_name** as a VARCHAR (255 characters at max), and make it NOT NULL.
- Define **manager_id** as an INTEGER, which will be a FOREIGN KEY referencing **employee_id** from the same table.

2. Create the *departments table*:
- Define **department_id** as a unique integer, auto-increment, and primary key.
- Define **department_name** as a VARCHAR (up to 255 characters), and make it not null.

3. Create the *employee_departments table*:
- Define **employee_id** as an integer, which will be a foreign key referencing employee_id in the employees table.
- Define **department_id** as an integer, which will be a foreign key referencing department_id in the departments table.
- Set a composite primary key on the combination of employee_id and department_id (optional).

4. Create the employee_projects table:
- Define **employee_id** as an integer, which will be a foreign key referencing employee_id in the employees table.
- Define **project_name** as a VARCHAR (up to 255 characters), and make it not null.

5. Create the managers table:
- Define **manager_id** as a UNIQUE INTEGER, AUTO_INCREMENT, and PRIMARY KEY.
- Define **employee_id** as an INTEGER, which will be a FOREIGN KEY referencing **employee_id** in the employees table.

## Screenshots
### A. Query Statements

1. Employee Table:
![Image](https://github.com/user-attachments/assets/5c40896b-3ec1-4aa3-9385-30e50efd2716)

2. Department Table:
