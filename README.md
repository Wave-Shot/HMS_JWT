

# 🏥 Hospital Management System

## 📌 Overview

The **Hospital Management System** is a Spring Boot backend application designed to manage hospital operations efficiently.

It includes:

* User Authentication (Register & Login)
* Role-based Access Control (Admin / User)
* Patient Management (CRUD Operations)
* JWT-based Authentication & Authorization
* MySQL Database Integration

This project is built using **Spring Boot, Spring Security, JWT, and MySQL**.

---

## 🚀 Tech Stack

* Java 17
* Spring Boot
* Spring Security
* Spring Data JPA
* MySQL
* JWT Authentication
* Maven
* Postman

---

## 📁 Project Structure

```
hospitalmanagement
│
├── config
│   ├── SecurityConfig
│   ├── JwtService
│   └── JwtAuthenticationFilter
│
├── controller
│   ├── AuthController
│   └── PatientController
│
├── dto
│   ├── AuthRequest
│   ├── AuthResponse
│   └── PatientDto
│
├── entity
│   ├── User
│   ├── Role
│   └── Patient
│
├── repository
│   ├── UserRepository
│   └── PatientRepository
│
├── service
│   ├── AuthService
│   └── PatientService
│
└── HospitalManagementApplication
```

---

## ✨ Features

### 🔐 Authentication

* Register User
* Login User
* JWT Token Generation
* Secure APIs using JWT

### 👨‍⚕️ Patient Management

* Add Patient
* Get All Patients
* Get Patient by ID
* Update Patient
* Delete Patient

---

## ⚙️ How to Run

1. Clone the repository

```
git clone <your-repo-url>
cd hospitalmanagement
```

2. Configure MySQL in `application.properties`

```
spring.datasource.url=jdbc:mysql://localhost:3306/hospital_db
spring.datasource.username=your_username
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

3. Run the application

```
mvn spring-boot:run
```

4. Test APIs using Postman

---

## 🔑 Authentication Flow

1. Register a user
2. Login to receive JWT token
3. Use token in headers:

```
Authorization: Bearer <your_token>
```

---

## 📌 Future Enhancements

* Doctor Management
* Appointment Scheduling
* Billing System
* Role-based dashboards

---

## 👨‍💻 Author

Srihari V

