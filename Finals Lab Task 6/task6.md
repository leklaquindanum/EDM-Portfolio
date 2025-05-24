# FINALS LAB TASK 6
This activity is different from the previous ones, as this time, it is about using a NoSQL DBMS, MongoDB. Here, I will tackle on how to create databases, insert documents, and its built-in features (find, update, search, and delete). At the last part, I will show the relationships of the inserted documents.

## Procedures
1. Create a Database
   - Start by creating or switching to a specific database.
   - The selected database becomes the active workspace for all upcoming operations.
2. Insert Documents
   - Within the database, a collection is created.
   - Multiple documents are inserted into the collection, each containing structured data fields such as name, age, or address.
3. FIND Documents
   - Display all documents stored in the collection.
   - Use filters to find specific documents based on certain values like name or ID.
4. UPDATE Documents
   - Locate the document that needs modification using a condition (e.g., name or ID).
   - Specify the field(s) to be changed and apply the update.
   - Confirm the update by checking the document again.
5. SEARCH Documents
   - Use specific criteria to locate documents that match particular conditions (e.g., age greater than a value or status equals a specific string).
   - Review the matched results for accuracy.
6. DELETE Documents
   - Identify the document(s) to be removed using a condition.
   - Remove the document(s) from the collection.
   - Verify deletion by checking the collection contents.

## Screenshots
1. Create database and collection:

![Image](https://github.com/user-attachments/assets/2d2cf971-986f-4314-9aef-a2538d9ae3f3)

2. Insert documents:

2a. Fight Club
![Image](https://github.com/user-attachments/assets/d7ea6008-491e-43c4-9438-b71fa6a3118b)

2b. Pulp Fiction
![Image](https://github.com/user-attachments/assets/20bcf42c-4158-43ad-9bdc-83b727059c08)

2c. Inglorious Basterds
![Image](https://github.com/user-attachments/assets/fb95f3dc-5987-4fa1-8e56-28f9a1251f9e)

2d. The Hobbit: An Unexpected Journey
![Image](https://github.com/user-attachments/assets/a0f665b9-beb4-4413-b5ec-6cdd8b569b3d)

2e. The Hobbit: The Desolation of Smaug
![Image](https://github.com/user-attachments/assets/3cd3fa37-a3aa-4403-be86-111573a39222)

2f. The Hobbit: The Battle of the Five Armies
![Image](https://github.com/user-attachments/assets/616346b2-43af-48a3-89b1-f24994840320)

2g. Pee Wee Herman's Big Adventures
![Image](https://github.com/user-attachments/assets/ebd96481-37c9-486c-aff3-57c4a5efd072)

2h. Avatar
![Image](https://github.com/user-attachments/assets/e3049964-1d1c-4f7d-98fe-7a9fc3ada58b)

3. FIND Documents:

3a. Get all documents via find() command
![Image](https://github.com/user-attachments/assets/d3aad3e4-1437-4d2e-9945-e4bf3641919f)

3b. Get all documents with 'writer' set to "Quentin Tarantino"
![Image](https://github.com/user-attachments/assets/a63ddd76-adc3-49ba-9004-789ea5b38dfb)

3c. Get all documents where 'actors' include "Brad Pitt"
![Image](https://github.com/user-attachments/assets/a28ac1fe-7585-43d2-9715-768233a6f89f)

3d. Get all documents with 'franchise' set to "The Hobbit"
![Image](https://github.com/user-attachments/assets/1b3935be-37cf-4bf3-8970-eed955a88d54)

3e. Get all movies released in the 90s
![Image](https://github.com/user-attachments/assets/a7f367ee-e8c0-486f-9ac7-0986c1d6f265)

3f. Get all movies released before the year 2000 or after 2010
![Image](https://github.com/user-attachments/assets/018491ad-6acd-41e7-9399-f9ab9779f580)

4. UPDATE Documents:

4a. Add synopsis to "The Hobbit: An Unexpected Journey"
![Image](https://github.com/user-attachments/assets/b845cd3a-97c2-4d9d-ab95-d68dea989abc)
![Image](https://github.com/user-attachments/assets/2ca2d0f3-e054-4222-be16-864ebeafb2e3)

4b. Add a synopsis to "The Hobbit: The Desolation of Smaug"
![Image](https://github.com/user-attachments/assets/cfd0595e-1604-4f4b-beb4-12fc90a210e7)
![Image](https://github.com/user-attachments/assets/f42947da-e6fc-436d-89a2-dc721179eddd)

4c. Add an actor named "Samuel L. Jackson" to the movie "Pulp Fiction"
![Image](https://github.com/user-attachments/assets/3b0e128b-99d5-43ad-8cc2-772eb0211034)
![Image](https://github.com/user-attachments/assets/32706faf-9da5-4004-95d6-c47f4cb47b76)

5. Text Search:

5a. Find all movies that have a synopsis that contains the word "Bilbo"
![Image](https://github.com/user-attachments/assets/2511be44-69e1-48ce-9bfc-982fb9f72eb9)

5b. Find all movies that have a synopsis that contains the word "Gandalf"
![Image](https://github.com/user-attachments/assets/dccc03be-dd2d-4c47-9f7f-62761ef27297)

5c. Find all movies that have a synopsis that contains the word "Bilbo" and not the word "Gandalf"
![Image](https://github.com/user-attachments/assets/0cb774ea-052f-469d-8533-4d3fbba68cab)

5d. Find all movies that have a synopsis that contains the word "dwarves" or "hobbit"
![Image](https://github.com/user-attachments/assets/2b29c2dc-24ba-4e23-ac9c-c7f3ccc5c1ef)

5e. Find all movies that have a synopsis that contains the word "gold" and "dragon"
![Image](https://github.com/user-attachments/assets/d2138eab-b775-491d-a0e0-cee836f8ab4a)

6. DELETE Documents:

6a. Delete the movie "Pee Wee Herman's Big Adventure"
![Image](https://github.com/user-attachments/assets/2e8d6574-d6b0-4dfd-918d-efbe60eddfbf)

6b. Delete the movie "Avatar"
![Image](https://github.com/user-attachments/assets/674e8716-1674-4742-af5e-6414719a2f22)

## Relationships
1. Insert the following documents into a “users” collection

1a. Create collection named “users”
![Image](https://github.com/user-attachments/assets/d740f184-6155-4aee-8b3b-c2373bb2f3e4)

1b. Insert documents
![Image](https://github.com/user-attachments/assets/5a109ef0-26f5-4197-aa4a-f1940b4f2722)
![Image](https://github.com/user-attachments/assets/3a4f0574-1234-486f-863b-bd6d312e83d1)

2. Insert the following documents into a “posts” collection

2a. Create collection named “posts”
![Image](https://github.com/user-attachments/assets/25153972-26e5-477d-ae4d-2387906321ad)

2b. Insert documents
![Image](https://github.com/user-attachments/assets/e8c0b25a-ccaf-40ab-aa33-8488078e69e8)
![Image](https://github.com/user-attachments/assets/27a8ab71-c548-4536-a1c5-29af950166be)
![Image](https://github.com/user-attachments/assets/040fcd2e-5428-4b35-b2c1-c3e7e3d2aaab)
![Image](https://github.com/user-attachments/assets/3e125ea4-e8d6-4032-8e12-3367ade0c379)
![Image](https://github.com/user-attachments/assets/6ca76eb5-f88e-4d79-bfe8-0f24918e273a)
![Image](https://github.com/user-attachments/assets/9896f3bc-cdcc-47b6-a47f-54ec382dfef1)

3. Insert the following documents into a “comments” collection

3a. Create collection named “comments”
![Image](https://github.com/user-attachments/assets/d3a8cbf4-1bff-4bbf-be97-a029f98636ba)

3b. Insert documents
![Image](https://github.com/user-attachments/assets/48ba0ff4-909d-4049-8465-b6efb3c0d921)
![Image](https://github.com/user-attachments/assets/2c45031d-d232-4587-a93a-d742243f4a73)
![Image](https://github.com/user-attachments/assets/2e460efc-abec-4190-950f-afa883dac05f)
![Image](https://github.com/user-attachments/assets/abe10abf-ba75-4b26-b0db-c68897f287ac)
![Image](https://github.com/user-attachments/assets/b333c322-4f09-4e4e-8686-c09d21983b3e)

4. Querying/finding related collections

4a. Find all users via find command
![Image](https://github.com/user-attachments/assets/2ad8beef-d3a8-4fa1-a525-86e0bb56d4f3)

4b. Find all posts via find command
![Image](https://github.com/user-attachments/assets/4ff29227-a4c3-4b39-9a57-da43c5a2a04b)

4c. Find all posts that was authored by "GoodGuyGreg"
![Image](https://github.com/user-attachments/assets/cee08eed-fe5e-4f6c-8779-c477ca9c07a5)

4d. Find all posts that was authored by "ScumbagSteve"
![Image](https://github.com/user-attachments/assets/715b8a32-51ea-4f3f-b6c3-a5d6bcd5fc3a)

4e. Find all comments via find command
![Image](https://github.com/user-attachments/assets/20356342-85cc-4fac-9556-4aa305762ec9)

4f. Find all comments that was authored by "GoodGuyGreg"
![Image](https://github.com/user-attachments/assets/67c95016-46a1-4b9b-85a7-a04c7ac9a424)

4g. Find all comments that was authored by "ScumbagSteve"
![Image](https://github.com/user-attachments/assets/f745a862-3d06-4480-8aba-97168d2a55be)

4h. Find all comments belonging to the post "Reports a bug in your code"
![Image](https://github.com/user-attachments/assets/72707354-897d-436c-897e-b0b3bdf75d2f)
