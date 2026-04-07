# usergram-api-gateway

API Gateway POC for USERGRAM, built with Spring Boot and Spring Cloud Gateway.

## Tech Stack

- **Java 25**
- **Spring Boot 4.0.5**
- **Spring Cloud 2025.1.1** (Gateway)
- **Spring Data JPA**
- **Spring WebFlux**
- **MySQL**
- **Lombok**
- **Gradle 9.2.1**

## Prerequisites

Make sure the following are installed on your machine:

- **Java 25** — [Download](https://jdk.java.net/)
- **MySQL** — running locally or via Docker

## Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
cd usergram-api-gateway
```

### 2. Configure the database

Create a MySQL database and update `src/main/resources/application.properties` with your connection details:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/<your-db-name>
spring.datasource.username=<your-username>
spring.datasource.password=<your-password>
spring.jpa.hibernate.ddl-auto=update
```

### 3. Build the project

```bash
./gradlew build
```

### 4. Run the application

```bash
./gradlew bootRun
```

The application will start on `http://localhost:8080` by default.

## Running Tests

```bash
./gradlew test
```

## Project Structure

```
src/
├── main/
│   ├── java/com/bebit/usergram/apigateway/
│   │   └── ApiGatewayApplication.java
│   └── resources/
│       └── application.properties
└── test/
    └── java/com/bebit/usergram/
        └── UsergramApplicationTests.java
```
