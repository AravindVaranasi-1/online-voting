
# Online Voting System (Backend)

## Features
- User Registration & Login with JWT
- Cast one vote per registered user
- Real-time vote count per candidate

## Technologies
- Java 17
- Spring Boot 3.1.0
- Spring Security + JWT
- MySQL
- Maven

## Setup

1. Create MySQL database:
```
CREATE DATABASE banking_app;
```

2. Update MySQL password in `application.properties`.

3. Run the project:
```
mvn spring-boot:run
```

## Endpoints (Test in Postman)
- POST `/api/auth/register` — Register a user
- POST `/api/auth/login` — Login and get JWT
- POST `/api/vote` — Cast a vote (use JWT in header)
- GET `/api/results` — See vote counts
