# Mikes Java Project Template

A basic starting point for a Java application built with Maven.

## Requirements

- Java 17 or later (JDK)
- Maven 3.8 or later

## Project Structure

```
.
├── pom.xml                  # Maven build configuration and dependencies
├── README.md
└── src
    ├── main
    │   ├── java             # Application source code
    │   │   └── com/example/App.java
    │   └── resources        # Config files and other non-code assets
    └── test
        ├── java             # Unit tests (JUnit 5)
        │   └── com/example/AppTest.java
        └── resources        # Test-only resources
```

## Getting Started

Clone the repository and build the project:

```bash
git clone <repository-url>
cd <project-directory>
mvn clean install
```

## Common Commands

| Task                   | Command                                   |
|------------------------|-------------------------------------------|
| Compile                | `mvn compile`                             |
| Run all tests          | `mvn test`                                |
| Run a single test class| `mvn test -Dtest=AppTest`                 |
| Run a single test      | `mvn test -Dtest=AppTest#methodName`      |
| Package a JAR          | `mvn package`                             |
| Run the application    | `java -cp target/classes com.example.App` |
| Clean build output     | `mvn clean`                               |

## Contributing

1. Create a feature branch from `main`.
2. Make your changes and add tests.
3. Make sure `mvn test` passes.
4. Open a pull request.
