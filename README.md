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

### Local Development

#### Prerequisites

- JDK 21+
- Maven
- PostgreSQL
- Node.js
- npm

#### 1. Database Setup

Create the database:

```sql
CREATE DATABASE bugnbass OWNER bugnbass;
```

#### 2. Start Backend

```bash
cd backend
mvn spring-boot:run
```

Backend will be available at:

```text
http://localhost:8080
```

#### 3. Start Frontend

Open a second terminal:

```bash
cd frontend
npm install
npm run dev
```

Frontend will be available at:

```text
http://localhost:5173
```

---

### Docker Deployment

#### Prerequisites

- Docker
- Docker Compose
- Maven

#### 1. Build the Application

```bash
cd backend
mvn clean package
```

This builds the Spring Boot application and bundles the frontend into the generated JAR.

#### 2. Start Docker Containers

From the project root:

```bash
docker compose up --build
```

The following containers will be started:

- Spring Boot application
- PostgreSQL database

Application URL:

```text
http://localhost:8080
```

#### Persistent Storage

- PostgreSQL data is stored in a Docker volume.
- Product images are stored in the project's `product_images` directory through a Docker bind mount.

---

### Notes

- The frontend is bundled into the Spring Boot application during packaging.
- Database schema is initialized automatically on application startup.
- PostgreSQL must be running before starting the application in local development mode.
- Docker Compose automatically creates a dedicated network between the application and database containers.
- For local development, the frontend can be run independently using Vite for hot reloading.

## Disclaimer

This project was developed collaboratively as part of a team effort.
