# FINALS LAB TASK 1
This Lab Task involves writing SQL queries, creating table structures, and developing relational schemas or ER diagrams.  To demonstrate the database's construction, the portfolio will also contain SQL copies of the database and table structures.

## Instructions

1. Create the *employees table*:
- Define **employee_id** as a UNIQUE INTEGER, AUTO_INCREMENT, and PRIMARY KEY.
- Define **employee_name** as a VARCHAR (255 characters at max), and make it NOT NULL.
- Define **manager_id** as an INTEGER, which will be a FOREIGN KEY referencing **employee_id** from the same table.

2. Create the *departments table*:
- Define **department_id** as a UNIQUE INTEGER, AUTO_INCREMENT, and PRIMARY KEY.
- Define **department_name** as a VARCHAR (255 characters at max), and make it NOT NULL.

3. Create the *employee_departments table*:
- Define **employee_id** as an INTEGER, which will be a FOREIGN KEY referencing **employee_id** in the *employees table*.
- Define **department_id** as an INTEGER, which will be a FOREIGN KEY referencing **department_id** in the *departments table*.
- Set a COMPOSITE PRIMARY KEY on the combination of **employee_id** and **department_id** (optional).

4. Create the employee_projects table:
- Define **employee_id** as an INTEGER, which will be a FOREIGN KEY referencing **employee_id** in the *employees table*.
- Define **project_name** as a VARCHAR (255 characters at max), and make it NOT NULL.

5. Create the managers table:
- Define **manager_id** as a UNIQUE INTEGER, AUTO_INCREMENT, and PRIMARY KEY.
- Define **employee_id** as an INTEGER, which will be a FOREIGN KEY referencing **employee_id** in the *employees table*.

## Screenshots
### A. Query Statements

1. Employee Table:

![Image](https://github.com/user-attachments/assets/5c40896b-3ec1-4aa3-9385-30e50efd2716)

2. Department Table:

![Image](https://github.com/user-attachments/assets/90f6d08e-f49c-4999-91c6-d26aa396fa93)

3. Employee-Department Table:

![Image](https://github.com/user-attachments/assets/e24bef92-c996-4ea9-bf59-703da7b702dd)

4. Employee Project Table:

![Image](https://github.com/user-attachments/assets/05840404-0542-4573-b7a8-b1a5876ddc50)

5. Manager Table:


### B. Table Structure

1. Employee Table:

![Image](https://github.com/user-attachments/assets/29d85d2e-ddf1-453a-9661-d66dc81947cf)

2. Department Table:

![Image](https://github.com/user-attachments/assets/a4da5424-2c11-4885-86f7-25d4a9478d66)

3. Employee-Department Table:

![Image](https://github.com/user-attachments/assets/b0eff757-edfc-4a95-856e-bf529d57bddf)

4. Employee Project Table:

![Image](https://github.com/user-attachments/assets/71fa586c-1200-4cd2-ac17-4cf670c78d97)

5. Manager Table:


