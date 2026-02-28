# Backend Instructions

These instructions apply when working on backend code.

## Patterns
- Follow {{ARCHITECTURE}} pattern
- All business logic goes in the domain/application layer
- Infrastructure adapters are thin wrappers
- Use dependency injection via constructor

## Testing
- Unit tests for all use cases
- Integration tests for adapters
- Use {{TEST_FRAMEWORK}} with {{MOCK_FRAMEWORK}}
- Naming: method_scenario_expectedResult
