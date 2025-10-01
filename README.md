```
# Legacy EGP Application

A legacy Java EE (J2EE) enterprise application built with EJB 3.x, JSP/Servlets, and JPA. This multi-module Maven project represents a typical enterprise government portal (EGP) system from the mid-2000s era.

## Architecture

- **egp-core-ejb**: Core business logic with EJB 3.x stateless session beans, JPA entities, and DAOs.
- **egp-portal-war**: Web presentation layer with JSP pages and servlets.
- **egp-ear**: Enterprise Archive packaging both WAR and EJB JAR modules.

## Modernization Strategy

To modernize this legacy application, we aim to achieve the following objectives:
1. **Migrate to Spring Boot**: Replace EJBs with Spring beans and JPA with Spring Data JPA.
2. **Use Thymeleaf for Views**: Replace JSP with Thymeleaf templates.
3. **Leverage Spring Security**: Implement modern security practices.
4. **Containerization**: Dockerize the application for easy deployment.
5. **Logging and Monitoring**: Integrate with modern logging and monitoring tools like Logback and Prometheus.

## Getting Started

### Prerequisites

- Java 17 or later
- Maven 3.8.1 or later
- Docker (optional, for containerization)

### Building the Project

```bash
mvn clean install
```

### Running the Application

```bash
mvn spring-boot:run
```

### Docker Support

To build and run the application using Docker:

```bash
docker build -t legacy-egp-application:latest .
docker run -p 8080:8080 legacy-egp-application:latest
```

## Contributing

We welcome contributions! Please see `CONTRIBUTING.md` for more information on how to get started.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
```