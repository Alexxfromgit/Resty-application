# Resty

A RESTful web application built with Spring Boot.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Java 1.8 |
| Framework | Spring Boot 2.1.1 |
| Build | Gradle 4.10.2 |
| Server | Embedded Tomcat (via `spring-boot-starter-web`) |
| Testing | JUnit 4, Spring Boot Test |

## Getting Started

### Prerequisites

- JDK 1.8+

### Build

```bash
gradlew build
```

Produces a runnable JAR at `build/libs/resty-0.0.1-SNAPSHOT.jar`.

### Run

```bash
gradlew bootRun
```

The application starts on `http://localhost:8080` by default.

Alternatively, run the built JAR directly:

```bash
java -jar build/libs/resty-0.0.1-SNAPSHOT.jar
```

### Test

```bash
# All tests
gradlew test

# Specific test class
gradlew test --tests RestyApplicationTests
```

## Configuration

Application settings go in `src/main/resources/application.properties`. Common overrides:

```properties
server.port=8081
spring.application.name=Resty
logging.level.com.alexxrw.resty=DEBUG
```

## Project Structure

```
src/
├── main/
│   ├── java/com/alexxrw/resty/   # Application source
│   └── resources/
│       └── application.properties
└── test/
    └── java/com/alexxrw/resty/   # Test source
```

## License

This project is open source. See [LICENSE](LICENSE) for details.
