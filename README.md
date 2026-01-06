# 🎓 Student Management Web Application (Spring Boot)

## 📌 Giới Thiệu:

Ứng dụng quản lý sinh viên là một ứng dụng console được phát triển bằng ngôn ngữ **Java**, nhằm mô phỏng hệ thống quản lý sinh viên tại các trường đại học. Giao diện được xây dựng trên nền **console** đơn giản, trực quan. Dự án áp dụng mô hình **Lập trình Hướng Đối Tượng (OOP)**, sử dụng các cấu trúc dữ liệu như **ArrayList** để quản lý dữ liệu, và lưu trữ thông tin bằng **file nhị phân**.

## 🚀 Mục tiêu dự án:

- Giao diện <b>Java Spring Boot</b>.
- Có chức năng quản lý sinh viên, môn học và bảng điểm.
- Và các chức năng khác(tìm kiếm, CRUD).
- Lưu trữ và truy xuất dữ liệu thông qua hệ quản trị cơ sở dữ liệu **MySQL**.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 📌 Cụ thể:

### 1. Người dùng:(`User`)

#### • **Gồm các thuộc tính:** `username`, `password`, `role`

#### • **Chức năng**:

   🔑 **ADMIN**: có quyền truy cập đầy đủ vào hệ thống
   
                ○ Thêm, sửa, xóa dữ liệu: sinh viên, môn học, bảng điểm.
                ○ Xem toàn bộ danh sách sinh viên, môn học, bảng điểm.
                ○ Tìm kiếm bảng điểm, sinh viên, môn học để CRUD và theo dõi, quản lí.

   🎓 **STUDENT(Đang phát triển)**: có quyền truy cập hạn chế

                ○ Chỉ xem và theo dõi được thông tin về sinh viên,môn học, bảng điểm của mình.

### 2. Sinh viên:(`Student`)

#### • **Gồm các thuộc tính:** `student_id`, `fullname`, `gender`, `date_of_birth`, `major`


#### • **Chức năng**:

       ○ Thêm mới sinh viên, Sửa, Xóa thông tin sinh viên, Lưu dữ liệu, Hệ thống phản hồi và hiển thị lại danh sách sinh viên. 

### 3. Môn học:(`Course`)

#### • **Gồm các thuộc tính:** `course_id`, `course_name`, `credits`, `status`

#### • **Chức năng**:

       ○ Thêm mới môn học, Sửa,Xóa thông tin môn học, Lưu dữ liệu, Hệ thống phản hồi và hiển thị lại danh sách môn học.

### 4. Bảng điểm(`Transcript`)

#### • **Gồm các thuộc tính:** `id`, `student_id`, `course_id`, `grade10`, `semester`

#### • **Chức năng**: 

       ○ Tự động quy đổi điểm hệ 10 sang hệ 4, điểm chữ, và đánh giá đạt / không đạt.
       ○ Thêm mới bảng điểm, Sửa,Xóa thông tin bảng điểm, Lưu dữ liệu, Hệ thống phản hồi và hiển thị lại danh sách bảng điểm.

### ⚙️ Phương thức hoạt động chính:

#### Student Manager:

     • Hiển thị toàn bộ danh sách sinh viên, danh sách môn học, danh sách bảng điểm và theo dõi thông tin.
     • Tìm kiếm bảng điểm bằng mã sinh viên, mã môn học, tên học kì, tích hợp CRUD bảng điểm sau khi tìm kiếm.
     • Có chức năng đăng ký sinh viên vào các khóa học tương ứng.
     
- Dữ liệu được lưu trữ xuống file nhị phân.
- Cần tạo các lớp liên quan đến “Sinh viên”, “Môn học”, “Bảng điểm” để đọc, ghi dữ liệu vào một hoặc nhiều file.
- Khi làm việc với dữ liệu trong bộ nhớ, dữ liệu cần được lưu trữ dưới dạng các Collection tùy chọn như ArrayList, LinkedList, Map, ....

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

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

The project follows MVC (Model–View–Controller) combined with a Layered Architecture to ensure clean code, scalability, and maintainability

+ Controller Layer: Handles HTTP requests and responses

+ Service Layer: Contains business logic

+ Repository Layer: Handles database operations using JPA

+ View Layer: Renders UI using Thymeleaf templates**
## Running the Application:
>                 mvn spring-boot:run
- Access the application:

+ Home page: http://localhost:8080/

+ Greeting page: http://localhost:8080/greeting?name=User
## 🎯 Key Features:

Handle HTTP GET requests using Spring MVC

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
