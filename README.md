# 📌Spring Boot Greeting Web Application:

## System Requirements:

Before running this project, ensure that your development environment meets the following requirements:

+ Operating System: Windows / macOS / Linux

+ Java Development Kit (JDK): Java 17 or later

+ Build Tool: Maven 3.8+

+ Database: MySQL 8.0+

+ IDE (Recommended): IntelliJ IDEA / Eclipse / VS Code (with Java extensions)

## Required Tools Installation:
🔹 Java Development Kit (JDK)

>                        Install JDK 17

+ Verify installation:
>                        java -version
## 🧰 Technologies Used:

+ Programming Language: Java 17

+ Framework: Spring Boot (Spring MVC, Spring Data JPA)

+ View Engine: Thymeleaf

+ Database: MySQL

+ ORM: Hibernate (via Spring Data JPA)

+ Frontend Interaction: AJAX (jQuery)

+ Build Tool: Maven

+ Development Tool: Spring Boot DevTools

## 🏗 Project Architecture:

The project follows MVC (Model–View–Controller) combined with a Layered Architecture to ensure clean code, scalability, and maintainability.
> Controller  →  Service  →  Repository  →  Database
     ↓            ↓            ↓
   View        Business      JPA
 (Thymeleaf)   Logic
**Architecture Layers:

+ Controller Layer: Handles HTTP requests and responses

+ Service Layer: Contains business logic

+ Repository Layer: Handles database operations using JPA

+ View Layer: Renders UI using Thymeleaf templates**
## Running the Application:
>                 mvn spring-boot:run
**Access the application:

*Home page: http://localhost:8080/

*Greeting page: http://localhost:8080/greeting?name=User
## 🎯 Key Features:

**Handle HTTP GET requests using Spring MVC

Accept request parameters with @RequestParam

Server-side rendering with Thymeleaf

CRUD operations using Spring Data JPA

MySQL database integration

AJAX-based dynamic interaction

MVC and layered architecture implementation**
## Spring Boot Web Application Project:
Developed a web application using Spring Boot MVC and Thymeleaf

Implemented layered architecture (Controller, Service, Repository)

Integrated MySQL database using Spring Data JPA

Applied OOP principles and Dependency Injection

Built AJAX-based frontend interactions using jQuery

Used Maven for dependency management and build automation
