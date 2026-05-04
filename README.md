# BugnBass Music Store

Full-stack web application for managing and purchasing musical instruments.  
The platform provides functionality for browsing products, managing a shopping cart, placing orders, and handling product reviews.

---

## Overview

BugnBass is an e-commerce-style application designed for music instrument retail.  
It demonstrates a complete full-stack architecture with a Java Spring Boot backend and a React frontend application.

Users can:
- Browse and search products
- Add items to cart
- Place and manage orders
- Leave and view product reviews

---

## My Contribution

**Team project (3 developers)**  
I contributed approximately **50% of the implementation**, focusing primarily on core application logic and database design.

Key contributions:
- Designed and implemented REST APIs using **Spring Boot**
- Developed core business logic for:
  - product management
  - order processing
  - review system
- Designed and structured the **PostgreSQL database schema**
- Developed React components for:
  - product listing
  - shopping cart
  - review handling
- Integrated frontend with backend REST APIs
- Participated in debugging, feature enhancements, and testing
- Contributed to overall application architecture and integration

---

## Architecture

- Backend: RESTful API built with Spring Boot  
- Frontend: React SPA consuming backend APIs  
- Database: PostgreSQL relational database  

---

## Tech Stack

### Backend
- Java 21
- Spring Boot
- Maven
- PostgreSQL

### Frontend
- React / TypeScript
- Vite
- npm

### Tools & Workflow
- Git (version control)
- CI/CD (GitHub Workflows)
- RESTful API design

---

## Features

- Product catalog with detailed views  
- Shopping cart functionality  
- Order creation and management  
- Product reviews and ratings  
- RESTful API for frontend-backend communication  
- Admin-level operations for managing products and orders  
- Full-stack integration between frontend and backend  

---

## Screenshots

<img width="1471" height="601" alt="Screenshot 2026-05-04 at 17 24 56" src="https://github.com/user-attachments/assets/e35efa72-6ae6-4b86-92a4-32bd18f78e47" />
<img width="1446" height="777" alt="Screenshot 2026-05-04 at 17 24 00" src="https://github.com/user-attachments/assets/afbc31d1-9660-4601-8632-fa59c581e593" />
<img width="1471" height="747" alt="Screenshot 2026-05-04 at 17 23 21" src="https://github.com/user-attachments/assets/84976ee5-18c2-4475-b4ae-1540b2b89f45" />

---

## Build & Run

### Prerequisites

- JDK 21+
- Maven
- PostgreSQL (running on port 5432)
- Node.js
- npm

### 1. Database Setup

Create the database:

```sql
CREATE DATABASE bugnbass OWNER bugnbass;
```

### 2. Run Backend

#### Option A — Run with Maven (development)

```bash
cd backend
mvn spring-boot:run
```

Backend will start on: http://localhost:8080

#### Option B — Build and run JAR

```bash
cd backend
mvn clean package
java -jar target/backend-0.0.1-SNAPSHOT.jar
```

### 3. Run Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend will start on: http://localhost:5173

### Notes

- The database will be initialized automatically on first run  
- Ensure PostgreSQL is running before starting the backend  

---

## Disclaimer

This project was developed collaboratively as part of a team effort.  
