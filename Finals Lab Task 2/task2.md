# FINALS LAB TASK 2
This Lab Task focuses on transforming an Entity-Relationship Model into a Relational Database with three main tables: Students, Assignments, and Submissions. Each table represents a key part of the system, with Submissions linking students to the assignments they've completed.

## Instructions

1. Create the *student table*:
- Define **username** as VARCHAR (50 characters at max), and as PRIMARY KEY.

2. Create the *assignment table*:
- Define **shortname** as VARCHAR (50 characters at max), and as PRIMARY KEY.
- Define **due_date** as DATE, and make it NOT NULL.
- Define **url** as VARCHAR (255 characters at max), and make it optional (can be either NULL or NOT NULL).

3. Create the *submission table*:
- Define **username** as VARCHAR (50 characters at max).
- Define **shortname** as VARCHAR (50 characters at max).
- Define **version** as INTEGER.
- Define **submit_date** as DATE, and make it NOT NULL. 
- Define **data** as TEXT.
- Create COMPOSITE PRIMARY KEYS which are: **username**, **shortname**, and **version**.
- Create FOREIGN KEYS which are: **username**, and **shortname**.

## Relationships of each Table

1. *student table*

Primary Key: **username**

Relationships:
- *submission table*: One-to-Many — One student/username may have Many submissions.

2. *assignment table*

Primary Key: **shortname**

Relationships:
- *submission table*: One-to-Many — One assignment/shortname may have Many submissions.

3. *submission table*

Composite Primary Key: **username, shortname, version**

Relationships:
- *student table*: Many-to-One — Each submission came from one student.
- *assignment table*: Many-to-One — Each submission came from one assignment.

### NOTE:
*This Relational Model is a **Many-to-Many** relationship between **students** and **assignments**; while **version** is tracing many submissions.*

## Screenshots
### A. Query Statements

1. Student Table:

![Image](https://github.com/user-attachments/assets/6890a90e-b778-45e7-b886-90b682f3aac2)

2. Assignment Table:

![Image](https://github.com/user-attachments/assets/f577e7aa-b6ab-42ec-8f0a-2149922e76be)

3. Submission Table:

![Image](https://github.com/user-attachments/assets/4bef385d-90f4-43bf-a607-93ebf6be97ed)

### B. Table Structure

1. Student Table:

![Image](https://github.com/user-attachments/assets/4bb67507-21d8-475a-81d3-33f8882c90e4)A

2. Assignment Table:

![Image](https://github.com/user-attachments/assets/31d8bedf-0fb1-40a2-9028-a9e096b84da5)

3. Submission Table:

![Image](https://github.com/user-attachments/assets/9c9d2037-a11e-4173-bd33-c653e9df5928)

### C. Entity Relationship Diagram

![Image](https://github.com/user-attachments/assets/24aacc83-ef52-4b54-b438-4159b53398e4)

### D. Reference of the Making of the Relational Table

![Image](https://github.com/user-attachments/assets/39f7d174-5224-492f-862c-3260224cdbed)
