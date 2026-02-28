# Project Context

## Tech Stack
- Java 21, Spring Boot 3.3
- PostgreSQL 16, Kafka 3.7, Redis 7
- Docker + Kubernetes
- Maven 3.9

## Architecture
Hexagonal (Ports & Adapters). NEVER mix business logic in adapters or controllers.

Package structure:
- `domain/` — entities, value objects, ports, domain events
- `application/` — use cases, commands, queries, DTOs
- `infrastructure/` — adapters, configuration, persistence, messaging

## Code Conventions
- Always inject via constructor, never @Autowired on field
- No Lombok in domain classes
- Records for DTOs and Commands
- Tests: JUnit 5 + Mockito, naming: method_scenario_expectedResult
- Use Optional instead of null for optional return values
- Exceptions: domain exceptions extend DomainException

## What you must NEVER do
- Do not add dependencies without being asked
- Do not make automatic commits
- Do not mix responsibilities between layers
- Do not use @Transactional in domain layer
- Do not expose domain entities in REST responses — use DTOs
