# ☁️ Spring Boot Cloud Starter

<p align="center">
  <img src="https://img.shields.io/badge/Java-17%2F21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot-3.2-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white" />
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" />
</p>

> A **production-ready Spring Boot 3 microservice template** with everything you need out-of-the-box — Docker, Kubernetes, CI/CD, monitoring, security, and best practices. Clone and build in minutes, not days.

---

## 🚀 What's Included

- ✅ **Spring Boot 3.2** with Java 17/21 support
- ✅ **Spring Security** — JWT-based authentication pre-configured
- ✅ **Spring Data JPA** — Repository pattern with PostgreSQL
- ✅ **Flyway** — Database migration management
- ✅ **MapStruct** — Type-safe DTO mappings
- ✅ **OpenAPI 3 / Swagger UI** — Auto-generated API docs
- ✅ **Actuator + Prometheus** — Health checks and metrics
- ✅ **Grafana Dashboard** — Pre-built monitoring dashboards
- ✅ **Docker + Docker Compose** — One-command local dev setup
- ✅ **Kubernetes Helm Chart** — Production-ready K8s manifests
- ✅ **GitHub Actions CI/CD** — Build, test, Docker push, K8s deploy
- ✅ **SonarQube Integration** — Code quality gates
- ✅ **Testcontainers** — Integration tests with real dependencies
- ✅ **Structured Logging** — JSON logging with Logback + ELK ready
- ✅ **Global Exception Handling** — RFC 7807 Problem Details format

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Java 17 / 21 |
| Framework | Spring Boot 3.2 |
| Security | Spring Security + JWT |
| Database | PostgreSQL 15 |
| Migrations | Flyway |
| Build Tool | Maven 3.9 |
| Containerization | Docker + Docker Compose |
| Orchestration | Kubernetes (Helm 3) |
| CI/CD | GitHub Actions |
| Monitoring | Prometheus + Grafana |
| Testing | JUnit 5 + Testcontainers + Mockito |
| Code Quality | SonarQube + JaCoCo |
| API Docs | SpringDoc OpenAPI 3 |
| Logging | Logback + Loki-ready |

---

## 🚀 Quick Start

```bash
# Use as template
git clone https://github.com/Pcveldi22/springboot-cloud-starter.git my-service
cd my-service

# Start dependencies
docker-compose up -d postgres

# Run the service
mvn spring-boot:run

# API docs available at:
# http://localhost:8080/swagger-ui.html
# http://localhost:8080/actuator/health
```

---

## 📁 Project Structure

```
springboot-cloud-starter/
├── src/
│   ├── main/java/com/starter/
│   │   ├── config/          # Security, OpenAPI, CORS config
│   │   ├── controller/      # REST controllers
│   │   ├── service/         # Business logic
│   │   ├── repository/      # JPA repositories
│   │   ├── model/           # Entities + DTOs
│   │   ├── exception/       # Global exception handling
│   │   └── security/        # JWT filter + auth
│   └── test/                # Unit + integration tests
├── k8s/
│   └── helm/                # Kubernetes Helm chart
├── .github/
│   └── workflows/           # CI/CD pipelines
│       ├── ci.yml
│       └── deploy.yml
├── docker-compose.yml
├── Dockerfile
└── pom.xml
```

---

## ⚙️ CI/CD Pipeline

```yaml
# Automated pipeline on every PR / push to main:
Build → Unit Tests → Integration Tests → SonarQube → Docker Build → Push to Registry → Deploy to K8s
```

---

## 📄 License

MIT License — free to use as a base for your projects.

<p align="center">Made with ❤️ by <a href="https://github.com/Pcveldi22">Pc Veldi</a> | Senior Software Engineer</p>
