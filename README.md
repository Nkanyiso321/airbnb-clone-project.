# Airbnb Clone Project

## Project Overview
The Airbnb Clone Project is a full-stack application that simulates a booking platform similar to Airbnb. This project focuses on backend development, database design, API development, security, and deployment. Learners will gain hands-on experience building a scalable web application and understanding real-world workflows.

**Project Goals:**
- Build a secure backend for an accommodation booking platform.
- Implement database design and API endpoints for core functionality.
- Learn collaborative workflows using GitHub.
- Apply modern security practices and CI/CD pipelines.

---

## Team Roles
- **Backend Developer:** Designs and implements server-side logic, APIs, and database interactions.
- **Database Administrator (DBA):** Plans and manages database schemas, relationships, and optimizations.
- **Frontend Developer:** Builds user interfaces and integrates frontend with backend APIs.
- **DevOps Engineer:** Sets up CI/CD pipelines, manages deployment automation, and ensures system reliability.
- **QA Engineer:** Tests application features, verifies API functionality, and ensures code quality.

---

## Technology Stack
- **Django:** Web framework for building secure and scalable RESTful APIs.
- **MySQL/PostgreSQL:** Relational database to manage user, property, booking, and payment data.
- **GraphQL:** Flexible API query language for fetching only the required data.
- **Docker:** Containerization tool for consistent development and deployment environments.
- **GitHub Actions:** Automates testing, building, and deployments via CI/CD pipelines.
- **JWT Authentication:** Provides secure token-based authentication for users.

---

## Database Design

**Entities & Fields:**

1. **User**
   - id, name, email, password, profile_picture
   - Relationships: A user can have multiple bookings and multiple properties (as a host)

2. **Property**
   - id, title, description, location, price, host_id
   - Relationships: Belongs to one user (host); can have multiple bookings and reviews

3. **Booking**
   - id, user_id, property_id, start_date, end_date, total_price
   - Relationships: Belongs to a user and a property

4. **Review**
   - id, user_id, property_id, rating, comment
   - Relationships: Linked to both a user and a property

5. **Payment**
   - id, booking_id, amount, payment_method, status
   - Relationships: Each payment belongs to a booking

---

## Feature Breakdown
- **User Management:** Register, login, and manage profiles securely.
- **Property Management:** Hosts can create, update, and delete property listings.
- **Booking System:** Users can book properties and track reservations.
- **Review System:** Users can leave feedback on properties they have stayed in.
- **Payment Integration:** Handles secure payments for bookings.
- **Search & Filtering:** Users can search properties by location, price, and availability.

---

## API Security
- **Authentication:** JWT-based token authentication for secure user sessions.
- **Authorization:** Role-based access control to protect sensitive operations.
- **Rate Limiting:** Prevents abuse of API endpoints.
- **Data Validation:** Ensures safe inputs and prevents injection attacks.

**Importance:** Security measures protect user data, secure financial transactions, and maintain system integrity.

---

## CI/CD Pipeline
- **Continuous Integration/Continuous Deployment (CI/CD):** Automates testing, building, and deployment.
- **Tools Used:** GitHub Actions, Docker

**Benefits:**
- Reduces manual errors during deployment
- Ensures code quality and system reliability
- Speeds up delivery of new features and bug fixes

---

## Manual Review
- Ensure all features are implemented and documented.
- Submit your GitHub repository link for peer and manual QA review.


