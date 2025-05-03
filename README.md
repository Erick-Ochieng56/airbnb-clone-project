# 🏡 Airbnb Clone Project

## 🚀 Project Overview
The Airbnb Clone project is a backend system designed to mimic the core features of Airbnb, enabling users to register, list properties, make bookings, process payments, and leave reviews. Built with scalability and performance in mind, it provides RESTful and GraphQL APIs for seamless frontend integration.

---

## 🏆 Project Goals
- **User Management:** Handle secure user authentication and profile handling.
- **Property Management:** Allow hosts to manage property listings.
- **Booking System:** Enable users to book available properties.
- **Payment Processing:** Manage transactions for bookings.
- **Review System:** Allow reviews and ratings for properties.
- **Data Optimization:** Ensure efficient data access and storage.

---

## 👥 Team Roles

| Role | Responsibilities |
|------|------------------|
| **Backend Developer** | Designs and builds the API endpoints, handles business logic, and integrates external services. |
| **Database Administrator** | Designs and manages the database schema, optimizes queries, and implements indexing. |
| **DevOps Engineer** | Manages CI/CD pipelines, Docker containers, deployments, and monitoring. |
| **QA Engineer** | Ensures all features are well-tested and bugs are caught early. Writes automated and manual test cases. |

---

## ⚙️ Technology Stack

| Technology | Purpose |
|------------|---------|
| **Django** | A high-level Python web framework used to build the RESTful API. |
| **Django REST Framework** | Extends Django for building APIs easily with CRUD functionality. |
| **PostgreSQL** | A robust relational database for storing structured data. |
| **GraphQL** | Provides a flexible query language to retrieve nested or filtered data. |
| **Celery** | Handles background tasks like sending emails or processing asynchronous payments. |
| **Redis** | Used for caching and improving performance by reducing database load. |
| **Docker** | Ensures consistent development and production environments using containers. |
| **CI/CD Tools (GitHub Actions)** | Automates testing and deployment workflows for faster and safer delivery. |

---

## 🗃️ Database Design

| Entity | Key Fields |
|--------|------------|
| **User** | id, username, email, password, is_host |
| **Property** | id, title, location, price, host (FK to User) |
| **Booking** | id, user (FK), property (FK), check_in, check_out |
| **Payment** | id, booking (FK), amount, status, payment_date |
| **Review** | id, property (FK), user (FK), rating, comment |

**Relationships:**
- A user can own multiple properties.
- A property can have many bookings and reviews.
- A booking is linked to a user and a property.
- A payment is associated with a booking.
- A review is tied to a user and a property.

---

## 🧩 Feature Breakdown

- **User Management:** Enables secure user registration, login, and profile updates.
- **Property Management:** Hosts can create, update, and delete property listings.
- **Booking System:** Users can reserve properties, modify bookings, and manage check-ins/outs.
- **Payment Processing:** Supports payment transactions and stores payment data.
- **Review System:** Users can provide ratings and feedback for properties they’ve booked.
- **API Access:** RESTful and GraphQL endpoints available for frontend consumption.
- **Database Optimization:** Indexes and caching strategies implemented for speed and efficiency.

---

## 🔐 API Security

- **Authentication:** JWT or session-based mechanisms to verify users.
- **Authorization:** Role-based access control to prevent unauthorized actions (e.g., only hosts can list properties).
- **Rate Limiting:** Protects against brute-force attacks and API overuse.
- **Input Validation & Sanitization:** Prevents SQL injections and XSS attacks.
- **HTTPS Enforcement:** Ensures all data transfer is encrypted.
- **Secure Payment Handling:** Protects financial transactions and sensitive booking information.

**Importance:** Secures user data, prevents data leaks, protects against fraud, and builds trust with users.

---

## 🔁 CI/CD Pipeline

**CI/CD (Continuous Integration / Continuous Deployment)** automates the build, test, and deployment process. It ensures every code change is verified by automated tests and deployed quickly and reliably.

**Tools:**
- **GitHub Actions:** For running tests and deploying on push.
- **Docker:** Containerizes the application for consistency.
- **PostgreSQL & Redis in Docker Compose:** For testing the full stack in a simulated environment.

**Benefits:**
- Reduces human error during deployment.
- Speeds up delivery cycles.
- Enables automated rollback on failure.

---

✅ **Manual Review Completed**

All mandatory README tasks have been completed and committed.

📌 GitHub Repository: [airbnb-clone-project](https://github.com/Erick-Ochieng56/airbnb-clone-project)
