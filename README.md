# Car Rental Backend

A robust backend system for managing a car rental business, built with Spring Boot, JPA, and MySQL. This project provides RESTful APIs for handling car rentals, user authentication, and more.

## Features

- **User Authentication & Authorization**: Secure JWT-based authentication and Spring Security.
- **Car Management**: Add, update, delete, and view available cars.
- **Rental Management**: Book, manage, and track car rentals.
- **Database Integration**: Uses MySQL for persistent storage via Spring Data JPA.
- **RESTful API**: Cleanly structured endpoints for frontend integration.
- **Testing**: Includes test dependencies and setup.
- **Docker Support**: Containerized deployment with a provided Dockerfile.
- **Developer Tools**: Hot reload and devtools for streamlined development.

## Tech Stack

- Java 21
- Spring Boot 3.x
- Spring Data JPA
- Spring Security
- JWT (JSON Web Token)
- MySQL
- Maven
- Docker

## Getting Started

### Prerequisites

- Java 21+
- Maven 3.x
- MySQL database instance
- Docker (optional)

### Clone the Repository

```bash
git clone https://github.com/krHimanshu123/CarRentalBackend.git
cd CarRentalBackend/carrental-backend-main
```

### Configure Database

Edit your `src/main/resources/application.properties` with your MySQL credentials:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/carrental
spring.datasource.username=YOUR_DB_USER
spring.datasource.password=YOUR_DB_PASSWORD
```

### Build and Run (Maven)

```bash
./mvnw clean install
./mvnw spring-boot:run
```

### Run with Docker

Build and run the container:

```bash
docker build -t carrental-backend .
docker run -p 8080:8080 carrental-backend
```

## API Overview

- `/api/auth/*` — User registration and login endpoints
- `/api/cars/*` — CRUD operations for cars
- `/api/rentals/*` — Manage car rentals

Refer to the source code in `src/main/java/` for controller and model details.

## Development

- Hot reload enabled via Spring Boot DevTools.
- Use `src/test/java/` for writing and running tests.

## Dependencies

Key dependencies (see [pom.xml](https://github.com/krHimanshu123/CarRentalBackend/blob/81868eacbe37375e52391f7cb05308f0e923cd1d/carrental-backend-main/pom.xml)):

- `spring-boot-starter-data-jpa`
- `spring-boot-starter-security`
- `spring-boot-starter-web`
- `mysql-connector-j`
- `jjwt` (JWT support)

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to fork, open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

---

**Author**: [krHimanshu123](https://github.com/krHimanshu123)
