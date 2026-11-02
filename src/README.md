
# Hospital Management System

A REST API-based Hospital Management System built using Java, Spring Boot, MySQL and JWT authentication.

## Tech Stack

- Java 17
- Spring Boot 4.1.2
- Spring Data JPA
- Hibernate
- MySQL
- Spring Security
- JWT Authentication
- Maven
- Postman

## Features

- User registration and login
- JWT-based authentication
- Patient management (Add, View, Update, Delete, Search)
- Doctor management
- Appointment booking
- Appointment cancellation
- MySQL database integration

## Project Structure

```text
src/main/java/hms
├── config
├── controller
├── entity
├── repository
├── service
└── HmsApplication.java
```

## Database Setup

1. Install MySQL.
2. Create the database:

```sql
CREATE DATABASE hospital_db;
```

3. Configure your local database credentials in `application.properties`.

Do not commit passwords or JWT secrets to GitHub.

## How to Run

1. Install Java 17 and Maven.
2. Open the project folder containing `pom.xml`.
3. Configure MySQL.
4. Run:

```bash
mvn spring-boot:run
```

5. Server runs at:

```text
http://localhost:8080
```

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | /api/auth/register | Register user |
| POST | /api/auth/login | Login and generate JWT |
| POST | /api/patients | Add patient |
| GET | /api/patients | Get all patients |
| GET | /api/patients/search?name=Arjun | Search patients |
| PUT | /api/patients/{id} | Update patient |
| DELETE | /api/patients/{id} | Delete patient |
| POST | /api/doctors | Add doctor |
| GET | /api/doctors | Get all doctors |
| POST | /api/appointments | Book appointment |
| PUT | /api/appointments/cancel/{id} | Cancel appointment |

## API Testing

APIs were tested using Postman.

## Future Improvements

- React frontend
- Admin dashboard
- Doctor and patient login roles
- Appointment notifications
- Deployment

## Author

Sibhiraaj

B.Tech Artificial Intelligence and Data Science
