# Library-Management-System-SpringBoot
This project aims to develop a robust Library Management System API using Spring Boot. The system facilitates librarians in efficiently managing books, patrons, and borrowing records.
# Features
- Manage books, patrons, and borrowing records
- RESTful API endpoints
- CRUD operations
- Validation and error handling
- Unit tests
# Tech Used
- Java
- Spring Boot
- Spring Data JPA
- MySQL
- Log4j2
# How to Run the Application
# Prerequisites
 Ensure you have the following installed:
 - Java Development Kit (JDK) 17
 - Maven
 - MySQL
 # Setup
 1. Clone the Repository:
    https://github.com/OmarHariry/Library-Management-System-SpringBoot
 3. Configure the Database:
    CREATE DATABASE library_db;
 5. Build the Project:
    mvn clean install
 7. Run the Application:
    mvn spring-boot:run
# Interact with API Endpoints
 You can use tools like curl, Postman, or any other API client to interact with the endpoints.
# Book Endpoints
### - Get all books:
GET /api/books

Response:

![image](https://github.com/user-attachments/assets/c3c24ca7-80e6-440d-bf61-dbfc92c0c8b8)

### - Get a book by ID:
GET /api/books/{id}
Response:

![image](https://github.com/user-attachments/assets/3b4d1535-6c41-43af-87f5-6dd493375ca4)

### - Add a new book:
POST /api/books/add

Request Body:

![image](https://github.com/user-attachments/assets/0fa3b189-047e-4868-98fc-c039f662db44)

Response:

![image](https://github.com/user-attachments/assets/379098cc-6587-4c47-b570-34823c1de07c)

### - Edit a existing book:
PUT /api/books/edit/{id}

Request Body:

![image](https://github.com/user-attachments/assets/8d82850a-2683-4251-91d9-b2660d5a1027)

Response:

![image](https://github.com/user-attachments/assets/9cfe434b-f7e0-4639-913c-a4d60471fbb5)

### - Delete a book:
DELETE /api/books/delete/{id}

Response:

![image](https://github.com/user-attachments/assets/1331a08d-2a9c-4336-80ec-40182d1792c5)

----
# Patron Endpoints
### - Get all patrons:
GET /api/patrons

Response:

![image](https://github.com/user-attachments/assets/325299b4-7bab-4179-beb3-f9e5c3634e26)

### - Get a patron by ID:
GET /api/patron/{id}
Response:

![image](https://github.com/user-attachments/assets/02524377-f219-4d03-b615-5ddbd750f734)

### - Add a new patron:
POST /api/patron/add

Request Body:

![image](https://github.com/user-attachments/assets/0db6926d-721b-42da-859d-a4f8c49b182f)

Response:

![image](https://github.com/user-attachments/assets/9e259070-3774-4e9a-8496-25b82f1081e8)

### - Edit a existing patron:
PUT /api/patron/edit/{id}
Request Body:

![image](https://github.com/user-attachments/assets/86603757-aac8-452f-8dff-45d420ec68df)

Response:

![image](https://github.com/user-attachments/assets/5b60c846-b8b3-4839-87b0-b8e4839f9baa)

### - Delete a patron:
DELETE /api/patron/delete/{id}

Response:

![image](https://github.com/user-attachments/assets/1595866e-1418-46d3-94a7-cbc8e5f86535)
----
# Borrowing Record Endpoints
### - Borrow a book:
POST api/borrow/{bookId}/patron/{patronId}

Response:

![image](https://github.com/user-attachments/assets/40d5f097-01c3-4293-89fd-546bd4b361fa)

### - Return a book:
PUT api/return/{bookId}/patron/{patronId}

Response:

![image](https://github.com/user-attachments/assets/1635f2ad-e90e-4cf0-aed3-f57d58a7ff09)

