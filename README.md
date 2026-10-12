# Smart Library Backend

Spring Boot REST API for Smart Library, using Java 21, Spring Data JPA, Spring Security, JWT, and MySQL.

## Requirements

- Java 21+
- MySQL 8+

Create a database named `smart_library_db`, then configure `DB_URL`, `DB_USERNAME`, `DB_PASSWORD`, `JWT_SECRET`, `ADMIN_EMAIL`, and `ADMIN_PASSWORD` as needed. Never use the built-in development credentials in production.

## Run locally

Windows:

```powershell
.\mvnw.cmd spring-boot:run
```

macOS/Linux:

```sh
./mvnw spring-boot:run
```

The API listens on port 8080 by default. Set `CORS_ALLOWED_ORIGINS` to the frontend origin. Set `SPRING_PROFILES_ACTIVE=prod` for deployment.

The Dockerfile builds and runs the API. See `src/main/resources/application-prod.properties` for production profile defaults.

Frontend repository: https://github.com/kasarla06072005-dev/smart-library-frontend
