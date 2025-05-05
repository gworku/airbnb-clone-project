# Airbnb Clone Project

This is a backend blueprint for the Airbnb Clone, developed as part of the ALX program. It focuses on backend architecture, API security, database design, and CI/CD pipelines.

## Tech Stack
- Django
- MySQL or PostgreSQL
- GraphQL
- Docker
- GitHub Actions
## Team Roles

- **Backend Developer**: Implements APIs, business logic, and handles server-side operations using Django.
- **Database Administrator (DBA)**: Designs the schema, maintains performance, and handles backup/security for MySQL or PostgreSQL.
- **DevOps Engineer**: Sets up CI/CD pipelines, Docker containers, and monitors deployment.
- **Security Engineer**: Implements authentication, data protection, and API security measures.
## Technology Stack

- **Django**: Python-based web framework used to build REST APIs and backend logic.
- **PostgreSQL/MySQL**: Relational database to store users, bookings, reviews, etc.
- **GraphQL**: API query language for efficient frontend-backend communication.
- **Docker**: Containerization tool to ensure consistent environments across dev/staging/prod.
- **GitHub Actions**: CI/CD tool to automate testing and deployment.
## Database Design

### Entities:
- **Users**: id, name, email, password, role
- **Properties**: id, owner_id (FK), title, description, location
- **Bookings**: id, property_id (FK), user_id (FK), check_in, check_out
- **Reviews**: id, booking_id (FK), rating, comment
- **Payments**: id, booking_id (FK), amount, status, timestamp

### Relationships:
- A user can list many properties.
- A booking is made by a user for a specific property.
- A booking can have one review and one payment.
