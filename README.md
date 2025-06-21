# 🛒 Spring Boot E-Commerce Backend Service

A robust and modular E-Commerce backend built with Spring Boot, MySQL, and secured with JWT authentication.  
This project covers essential e-commerce features like user registration, role-based access, order/cart processing, payment handling, and containerized deployment.

## Feature

- **User Registration & Login**: JWT-based authentication with Spring Security.
- **Role-Based Access Control**: Define and enforce user roles (`USER`, `ADMIN`, etc.).
- **Product Catalog (WIP)**: Scalable structure for adding product features.
- **Cart & Order System**: Add items to cart, place orders, and manage order lifecycle.
- **Payment Integration**: Basic implementation with support for payment success/failure callbacks.
- **JWT Authentication**: Secure login with token generation and validation.
- **Database Seeding**: Beginner-friendly approach for initial data setup.
- **Docker Support**: Easily containerized using Docker and Docker Compose.

## 🧰 Tech Stack

- **Language**: Java 17+
- **Framework**: Spring Boot
- **Persistence**: Spring Data JPA, MySQL
- **Security**: Spring Security + JWT
- **Documentation**: Swagger (SpringDoc)
- **Containerization**: Docker + Docker Compose
- **Testing**: JUnit 5 + Mockito

## 🐳 Docker Image

You can use the pre-built Docker image directly from Docker Hub:

🔗 [michellec07/spring-boot-e-commerce-backend](https://hub.docker.com/r/michellec07/spring-boot-e-commerce-backend)

## ⚙️ Setup Instruction (Docker Only)

### 📦 Prerequisites

Ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

Clone this repository to get the necessary files:

- `docker-compose.yml` — defines the backend and MySQL containers  
- `init.sql` — initializes the MySQL database with sample data

### ▶️ Run the Application

```bash
# Step 1: Pull the pre-built backend image from Docker Hub
docker pull michellec07/spring-boot-e-commerce-backend:latest

# Step 2: Start backend and MySQL containers
docker-compose up -d

