# FINALS LAB TASK 3
This Lab Task shows on how to manipulate a MySQL table (Product Table).This includes creating, altering, and modifying the said table.

## Instructions

1. Create the *product table*:
- Define **id** as INTEGER, AUTO INCREMENT, AND as PRIMARY KEY.
- Define **productName** as VARCHAR (100 characters at max), and make it NOT NULL.
- DEFINE **price** as DECIMAL.
  
2. ADD a *CONSTRAINT* to *CHECK* the prices to make sure there are no negative values and they are greater than 0
- ADD CONSTRAINT chkPricePositive.
- CHECK (price > 0).

3. Only insert the products that meet the requirements, from the given table *(price > 0)*:

4. *MODIFY* the **productName** column and set the VARCHAR limit to 120, and make it NOT NULL. 


## Screenshots
### A. Query Statements

Task 1: 

![Image](https://github.com/user-attachments/assets/95e7a142-00c7-4d62-8ee8-ec2d3c6cd24f)

Task 2:

![Image](https://github.com/user-attachments/assets/68699cad-f7e4-4f44-a6a7-c9a0008659e5)

Task 3:

![Image](https://github.com/user-attachments/assets/8093a63a-bf3d-42e3-a7b8-7e7d4b9835f7)

Task 4:

![Image](https://github.com/user-attachments/assets/b32837e9-9076-44d6-a653-0ee47e554b1a)

### B. Table Structure

Product Table:

![Image](https://github.com/user-attachments/assets/bef1f626-1585-4354-8c11-2154dfb942f5)

Insert Values:

![Image](https://github.com/user-attachments/assets/fec01bbf-180c-45bc-8be5-5dded66ae933)

### C. Entity Relationship Diagram

![Image](https://github.com/user-attachments/assets/09d8c92a-43b2-49cb-8434-96da00ac5d63)

