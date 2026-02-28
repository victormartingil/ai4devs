# Backend Rules

## Architecture
- All business logic MUST live in domain/ or application/ layers
- Infrastructure adapters MUST NOT contain business logic
- Ports are interfaces defined in the domain layer
- Adapters implement ports in the infrastructure layer

## Dependencies
- Domain layer has ZERO external dependencies
- Application layer depends only on domain
- Infrastructure depends on application and domain

## Naming
- Use cases: `{Verb}{Noun}UseCase` (e.g., `CreateOrderUseCase`)
- Commands: `{Verb}{Noun}Command`
- Ports: `{Noun}Repository`, `{Noun}Publisher`
- Adapters: `{Port}Adapter` (e.g., `OrderRepositoryAdapter`)
