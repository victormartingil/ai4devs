# Testing Instructions

## Unit Tests
- Test each use case independently
- Mock all external dependencies
- Follow naming convention: `method_scenario_expectedResult`
- One assertion per test when possible

## Integration Tests
- Test adapter implementations against real infrastructure (testcontainers)
- Verify database queries, message publishing, HTTP calls

## Coverage
- Minimum 80% line coverage on application layer
- 100% coverage on domain layer business rules
