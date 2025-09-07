# Java EE 7 Hello World Web App

A Java EE 7 web application demonstrating JSF, JAX-RS, JPA, CDI, and EJB technologies.

## Features
- **Web UI**: JSF 2.2 with facelets and CDI beans
- **REST API**: JAX-RS endpoints for Person CRUD operations
- **Database**: JPA with H2 in-memory database
- **Health Check**: `/health` endpoint for monitoring
- **Validation**: Bean validation with constraints

## Quick Start

1. **Build**: `mvn clean package`
2. **Deploy**: Deploy `hello-web.war` to JBoss EAP/WildFly
3. **Access**: 
   - Web: `http://localhost:8080/hello-web/`
   - API: `http://localhost:8080/hello-web/rest/persons`
   - Health: `http://localhost:8080/hello-web/health`

## API Examples

```bash
# Get all persons
curl http://localhost:8080/hello-web/rest/persons

# Create person
curl -X POST http://localhost:8080/hello-web/rest/persons \
  -H "Content-Type: application/json" \
  -d '{"name": "John Doe"}'
```

## Tech Stack
- Java EE 7, Maven, JSF 2.2, JAX-RS, JPA 2.1, CDI, EJB 3.2, H2 Database
