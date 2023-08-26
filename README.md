🔒 Spring Boot JWT Authentication with Spring Security 5.7.14

Welcome to the Spring Boot JWT Authentication project, powered by Spring Security 5.7.14! This repository serves as a comprehensive guide and practical implementation for establishing secure authentication using JSON Web Tokens (JWT) in a Spring Boot application. By employing JWT-based authentication, this project demonstrates industry best practices for securing your web application's endpoints.

**Features:**

**Cutting-Edge Spring Boot & Spring Security:** Utilize the power of Spring Boot 2.7.14 and Spring Security 5.7.14 for a robust and up-to-date security foundation.

**JWT-Based Authentication:** Dive deep into configuring and implementing JSON Web Token (JWT) authentication, offering a secure and stateless mechanism for user authentication.

**User Authentication and Authorization:** Learn how to efficiently manage user authentication and authorization using JWTs, enhancing the overall security posture of your application.

**Clean and Maintainable Configuration:** Experience well-organized configuration classes that adhere to separation of concerns principles, improving code readability and maintainability.

**Sample User Interface:** Interact with a user interface that demonstrates the seamless integration of JWT-based authentication, showcasing protected endpoints accessible only to authenticated users.

**Educational Resource:** This repository serves as an educational resource, guiding you through the process of understanding and implementing JWT authentication in Spring Security.

**Step 1: Running the Application**

1) Clone the repository to your local machine.
2) Run the application using your preferred Integrated Development Environment (IDE) or through the command line: ./mvnw          spring-boot:run.
3) The application will start on http://localhost:8080.

**Step 2: Obtaining a JWT Token**

1) Open Postman (or your preferred API testing tool).
2) Create a POST request and set the URL to http://localhost:8080/token.
3) In the request body, provide the following JSON:
    {
        "username": "Haris",
        "password": "123"
    }
4) Send the POST request.
5) You will receive a JWT token in the response. Copy this token.

**Step 3: Accessing Protected Endpoints**

1) Create a GET request in Postman.
2) Set the URL to http://localhost:8080/welcome.
3) In the Headers section, add a new key-value pair:
    Key: Authorization
    Value: Bearer {your-copied-jwt-token}

    For example, if your copied token is eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9..., your Authorization header value should be Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9....

4) Send the GET request.
    You have now successfully accessed a protected endpoint using JWT authentication! This process demonstrates the interaction between your Spring Boot application, Postman, and the JWT tokens for user authentication.

**Contributions:**

Feel free to contribute to this project by submitting pull requests that enhance JWT authentication, introduce additional features, or address security considerations.

**Note:**

This guide assumes that you have a basic understanding of Spring Boot, Spring Security, and API testing with tools like Postman. Refer to the official Spring Boot and Spring Security documentation for more comprehensive explanations and advanced configurations. Always prioritize security and best practices when implementing authentication in your applications.