# 🗳 Secure Role-Based Voting System

A full-stack voting application built using Spring Boot that allows users to cast votes securely and enables administrators to manage candidates and view results.

---

## 🚀 Features

- User registration and login
- Role-based access control (USER / ADMIN)
- One-user-one-vote enforcement
- Candidate management (Admin)
- Vote result monitoring (Admin)
- Server-side validation
- Layered architecture (Controller → Service → Repository)

---

## 🛠 Tech Stack

**Backend**
- Java 21
- Spring Boot
- Spring Security
- Spring Data JPA (Hibernate)
- MySQL

**Frontend**
- Thymeleaf
- HTML5
- CSS3

**Build Tool**
- Maven

---

## 🏗 Architecture

The application follows a layered architecture:

Controller → Service → Repository → Database


- Controllers handle HTTP requests
- Service layer contains business logic
- Repository layer interacts with MySQL using JPA

---

## 🔐 Security

- Role-based authorization using Spring Security
- Protected endpoints for Admin operations
- Session-based authentication
- CSRF protection enabled

---

## 🗄 Database Design

### Users Table
- id
- username
- password
- role
- has_voted

### Candidate Table
- id
- name
- party
- vote_count

---

## ⚙️ Configuration

Update your `application.properties` with your database credentials:
spring.datasource.url=jdbc:mysql://localhost**
spring.datasource.username=your_username
spring.datasource.password=your_password


---

## ▶️ How to Run

1. Clone the repository:
git clone https://github.com/swarajjogi/voting-app.git


2. Navigate into project:

   mvn clean install

   
4. Run the application:
   
   mvn spring-boot:run

   

## 📌 Future Improvements

- Password encryption using BCrypt
- Concurrency-safe vote updates
- Docker containerization
- Cloud deployment
- REST API version with React frontend

---

## 👨‍💻 Author

Swaraj Jogi  
Java & Spring Boot Developer
