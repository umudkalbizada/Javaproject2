My First Spring Boot API: Product Management

This project was developed by **Umud Kalbizada** to learn the fundamentals of backend development using Java and Spring Boot. It was created as part of Task 2.A for studies at Vistula University.

What Is This Project?

The goal of this project is to build a functional REST API that can manage product data. Currently, it uses a simulated backend—instead of a real database, a `HashMap` and an auto-incrementing counter are used to store and manage products in memory.

This approach makes it possible to focus on application logic, API structure, and clean architecture before introducing a database.

 How I Built It

The project follows a layered architecture to keep the code organized and professional:

Controller Layer
  `ProductController` handles incoming HTTP requests and returns appropriate responses.

Service Layer
  `ProductService` contains the business logic and processes data before it is stored.
Data Layer
  `ProductRepository` acts as a temporary in-memory database, managing how products are saved and retrieved.

Mapping & DTOs
  `ProductRequest` and `ProductResponse` classes ensure that data entering and leaving the API is clean, validated, and well-structured.

How It Works in Practice

1. A POST request is sent to the API endpoint (for example, to add a new product).
2. The incoming JSON data is converted into a Java object.
3. A unique ID is assigned to the product.
4. The product is stored in the in-memory repository.
5. The API responds with HTTP 201 (Created) and returns the newly created product details.

How to Test It

You can run this project in IntelliJ IDEA and use a tool like Postman to test the available endpoints.

Author:Umud Kalbizada

![PHOTO-2026-01-14-08-51-42](https://github.com/user-attachments/assets/8b802800-3749-447c-8da1-abd1aea18e9e)
![PHOTO-2026-01-14-08-51-42](https://github.com/user-attachments/assets/f47d3b92-e9f6-42ec-8492-7e14cf8d2b5f)
![PHOTO-2026-01-14-08-51-43](https://github.com/user-attachments/assets/66d2704a-1c3b-4d6c-99b2-4dbe2811dc4a)
![PHOTO-2026-01-14-08-51-43](https://github.com/user-attachments/assets/10b14fa3-4cb4-4e10-9dcb-f6ee773e8426)
![PHOTO-2026-01-14-08-51-44](https://github.com/user-attachments/assets/5894cd83-c083-4539-9bf2-ae16cc997f4f)
![PHOTO-2026-01-14-08-51-45](https://github.com/user-attachmen![PHOTO-2026-01-14-08-51-45](https://github.com/user-attachments/assets/88c60a43-ecbf-4367-b6ab-e63c94288a39)
ts/assets/20b6f1ab-ac57-4f4a-9da6-e41fc2db6b20)

