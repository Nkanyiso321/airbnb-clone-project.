# Airbnb Clone Project

## Project Overview
The Airbnb Clone Project is a comprehensive full-stack application that simulates a robust booking platform similar to Airbnb. This project focuses on backend systems, database design, API development, security, and deployment. Learners gain hands-on experience in creating a scalable web application while understanding real-world workflows and architectures.

**Project Goals:**
- Build a functional and secure backend for an accommodation booking platform.
- Implement database design and API endpoints for core functionality.
- Learn collaborative workflows using GitHub.
- Apply modern security practices and CI/CD pipelines.

**Tech Stack:**
- **Backend:** Django (Python web framework for building RESTful APIs)
- **Database:** MySQL or PostgreSQL (relational database to store user, property, booking, and payment data)
- **API:** GraphQL (for flexible data querying)
- **Containerization & CI/CD:** Docker, GitHub Actions
- **Security:** JWT Authentication, Rate Limiting, Data Validation

---

**Team Roles**

- **Backend Developer:** Designs and implements server-side logic, APIs, and database interactions.
- **Database Administrator (DBA):** Plans and manages database schemas, relationships, and optimizations.
- **Frontend Developer:** Builds user interfaces and integrates frontend with backend APIs.
- **DevOps Engineer:** Sets up CI/CD pipelines, manages deployment automation, and ensures system reliability.
- **QA Engineer:** Tests application features, verifies API functionality, and ensures code quality.


---

**Technology Stack**
- **Django:** Web framework for building secure and scalable RESTful APIs.
- **MySQL/PostgreSQL:** Relational database system to manage user data, properties, bookings, and payments.
- **GraphQL:** Flexible query language for APIs to fetch exactly the data needed.
- **Docker:** Containerization tool for consistent development and deployment environments.
- **GitHub Actions:** Automates testing, builds, and deployments through CI/CD pipelines.
- **JWT Authentication:** Secures user sessions with token-based authentication.

---

**Database Design**
**Entities & Fields:**

1. **User**
   - id, name, email, password, profile_picture
   - Relationship: A user can have multiple bookings and multiple properties (as a host)

2. **Property**
   - id, title, description, location, price, host_id
   - Relationship: A property belongs to one user (host) and can have multiple bookings and reviews

3. **Booking**
   - id, user_id, property_id, start_date, end_date, total_price
   - Relationship: A booking belongs to a user and a property

4. **Review**
   - id, user_id, property_id, rating, comment
   - Relationship: Reviews are linked to both a user and a property

5. **Payment**
   - id, booking_id, amount, payment_method, status
   - Relationship: Each payment belongs to a booking

---

## Feature Breakdown
- **User Management:** Register, login, and manage profiles. Ensures secure user authentication.
- **Property Management:** Hosts can create, update, and delete property listings.
- **Booking System:** Users can book properties and track their reservations.
- **Review System:** Users can leave feedback on properties they have stayed in.
- **Payment Integration:** Handles secure payments for bookings.
- **Search & Filtering:** Users can search properties based on location, price, and availability.

---

**API Security**
- **Authentication:** JWT-based token authentication for secure user sessions.
- **Authorization:** Role-based access control to restrict sensitive operations to authorized users.
- **Rate Limiting:** Prevents abuse of API endpoints.
- **Data Validation:** Ensures that inputs are safe and prevents injection attacks.

**Importance:** These measures protect sensitive user data, secure financial transactions, and maintain overall system integrity.

---

**CI/CD Pipeline**
**Continuous Integration/Continuous Deployment (CI/CD):**
- Automates testing, building, and deployment to ensure rapid and reliable updates.
- **Tools Used:** GitHub Actions (for automated workflows), Docker (for consistent environment deployment)

**Benefits:**
- Reduces manual errors during deployment.
- Ensures code quality and system reliability.
- Speeds up delivery of new features and bug fixes.

---

**Manual Review**
- Ensure all features are implemented and documented.
- Submit your GitHub repository link for peer and manual QA review.
