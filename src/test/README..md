# 🧑‍💼 Employee Management System (Microservices Architecture)

## 📘 Overview
The **Employee Management System (EMS)** is a RESTful backend application built using **Spring Boot** and a **microservices architecture**.  
It allows administrators and HR teams to efficiently manage employee records, authentication, and service configurations across distributed components.

This project demonstrates best practices in modular design, configuration management, authentication, and containerization — suitable for enterprise-level environments.

---

## 🏗️ Architecture & Microservices
The project is structured into **six key microservices**:

1. **Discovery Service (Eureka Server)** – Handles service registration and discovery.
2. **API Gateway** – Manages routing, load balancing, and security for incoming requests.
3. **Shared Config Server** – Provides centralized configuration management.
4. **Config Server** – Manages environment-specific properties for microservices.
5. **Authentication Service** – Manages user sign-up, login, and JWT-based authentication.
6. **Employee Service** – Handles all employee CRUD operations and interacts with the PostgreSQL database.

---

## ⚙️ Technologies Used

| Category | Technology |
|-----------|-------------|
| **Backend Framework** | Spring Boot 3.2.2 |
| **Programming Language** | Java 17 |
| **Microservices Framework** | Spring Cloud Netflix (Eureka, Gateway) |
| **Security** | Spring Security, JWT Authentication |
| **Database** | PostgreSQL 16 |
| **JPA / ORM** | Hibernate |
| **Build Tool** | Maven |
| **Version Control** | Git & GitHub |
| **Containerization** | Docker |
| **Dependency Management** | Maven Wrapper |
| **Testing** | JUnit 5, Spring Boot Test |
| **Configuration Management** | Spring Cloud Config Server |
| **IDE** | IntelliJ IDEA / VS Code / Spring Tool Suite (STS) |

---

## 🧩 Features

✅ Employee CRUD Operations (Create, Read, Update, Delete)  
✅ Role-Based Access Control (Admin, HR, Employee)  
✅ Centralized Config Server  
✅ API Gateway for unified routing  
✅ Service Discovery using Eureka  
✅ PostgreSQL integration via Spring Data JPA  
✅ Docker containerization for microservices  
✅ JWT authentication and authorization  

---

## 🚀 Getting Started

### 🧰 Prerequisites
Make sure you have installed:

- [Java 17+](https://adoptium.net/)
- [Maven 3.9+](https://maven.apache.org/)
- [PostgreSQL 16](https://www.postgresql.org/)
- [Docker](https://www.docker.com/) (optional, for containerization)
- Git

---

### ⚡ Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/<your-username>/employee-management-system.git
   cd employee-management-system/employee-service

Set Up the Database

Create a PostgreSQL database named employee_management

Update credentials in src/main/resources/application.properties

Run the Service

mvn clean install
mvn spring-boot:run


Access the Application

URL: http://localhost:8081

Default Login:
Username: admin
Password: 1234

🐳 Docker Support

Each microservice can be containerized individually using its Dockerfile.

Example:

docker build -t employee-service .
docker run -p 8081:8081 employee-service

📡 API Endpoints
Method	Endpoint	Description
POST	/api/auth/login	Authenticate user
GET	/api/employees	Fetch all employees
GET	/api/employees/{id}	Get employee by ID
POST	/api/employees	Add new employee
PUT	/api/employees/{id}	Update employee
DELETE	/api/employees/{id}	Delete employee
🧠 Future Enhancements

Add frontend integration with React or Angular

Implement microservice communication via Feign Clients

Integrate Kafka for event-driven messaging

Add CI/CD pipelines using GitHub Actions

Deploy to AWS / Docker Hub

👨‍💻 Author

Osiaro Famous
Front end and Backend Software Engineer — specializing in Spring Boot, Microservices, and DevSecOps
📧 Email: famous.osiaro@gmail.com
]
🔗 LinkedIn: linkedin.com/in/osiarofamous

🐙 GitHub: github.com/<fosityne007>

## 🧭 Architecture (overview)

Below is the system architecture and the dark-theme portfolio version.

![System Architecture](docs/architecture.png)
![Portfolio Diagram (Dark Theme)](docs/portfolio-diagram-dark.png)
