# 🤖 RoboShop Microservices Architecture

![RoboShop Architecture](./roboshop.jpg)

## 📌 Overview

RoboShop is a sample e-commerce application built using a Microservices Architecture. Each service is independently developed, deployed, and scaled while communicating with other services through APIs and messaging systems.

This repository provides detailed documentation for each microservice, database, and supporting component used in the RoboShop ecosystem.

---

## 🏗️ Architecture

The RoboShop application consists of:

### Frontend
- User-facing web application
- Acts as the entry point for customers
- Communicates with backend services through APIs

### Backend Services

#### Catalogue Service
- Manages product catalog information
- Stores product data in MongoDB

#### User Service
- Handles user registration and authentication
- Uses Redis for user-related data

#### Cart Service
- Manages shopping cart operations
- Stores cart data in Redis

#### Shipping Service
- Calculates shipping costs
- Manages shipping information
- Uses MySQL database

#### Payment Service
- Processes customer payments
- Publishes events to RabbitMQ

#### Dispatch Service
- Consumes messages from RabbitMQ
- Handles order dispatch operations

---

## 🗄️ Databases & Messaging

| Component | Purpose |
|------------|----------|
| MongoDB | Product catalog storage |
| Redis | User sessions and cart data |
| MySQL | Shipping data storage |
| RabbitMQ | Asynchronous communication between services |

---

## 🔄 Application Flow

1. User accesses the Frontend.
2. Frontend communicates with backend APIs.
3. Catalogue Service retrieves product information from MongoDB.
4. User Service handles authentication and user management.
5. Cart Service stores cart information in Redis.
6. Shipping Service calculates shipping details using MySQL.
7. Payment Service processes payments.
8. Payment events are sent to RabbitMQ.
9. Dispatch Service consumes messages and completes order dispatch.

---

## 📂 Repository Structure

```text
.
├── 01-mongoDB.MD
├── 02-catalogue.MD
├── 03-frontend.MD
├── 04-redis.MD
├── 05-User.MD
├── 06-CART.MD
├── 07-MySql.MD
├── 08-Shipping.MD
├── 09-RabbitMQ.MD
├── 10-Payment.MD
├── 11-Dispatch.MD
└── roboshop.jpg
```

---

## 📖 Documentation

| File | Description |
|--------|-------------|
| 01-mongoDB.MD | MongoDB Setup & Configuration |
| 02-catalogue.MD | Catalogue Service |
| 03-frontend.MD | Frontend Service |
| 04-redis.MD | Redis Setup |
| 05-User.MD | User Service |
| 06-CART.MD | Cart Service |
| 07-MySql.MD | MySQL Setup |
| 08-Shipping.MD | Shipping Service |
| 09-RabbitMQ.MD | RabbitMQ Setup |
| 10-Payment.MD | Payment Service |
| 11-Dispatch.MD | Dispatch Service |

---

## 🎯 Learning Objectives

This repository helps you understand:

- Microservices Architecture
- Service-to-Service Communication
- API Integration
- Event-Driven Architecture
- Database Management
- Message Queues
- DevOps Concepts
- Cloud-Native Application Design

---

## 👨‍💻 Ideal For

- DevOps Engineers
- Cloud Engineers
- Site Reliability Engineers (SREs)
- Platform Engineers
- Kubernetes Practitioners
- Students Learning Microservices

---

## ⭐ Support

If you find this repository useful:

- Star ⭐ the repository
- Fork 🍴 the project
- Share it with fellow DevOps Engineers

---

### Connect With Me

If you're interested in DevOps, Cloud, Kubernetes, CI/CD, Infrastructure as Code, and Microservices Architecture, feel free to connect and follow my learning journey.