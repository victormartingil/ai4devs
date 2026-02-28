---
name: scaffold-feature
description: Scaffolds a new feature following project architecture
context: fork
---

# Scaffold Feature

## Steps
1. Ask for the feature name and description
2. Create the domain entity/value object if needed
3. Create the application use case (command + handler)
4. Create the port interface in the domain layer
5. Create the infrastructure adapter
6. Create unit tests for the use case
7. Do NOT create the HTTP controller — that's a separate step

## File Structure
Each feature should create:
- `domain/model/{{FeatureName}}.java`
- `domain/port/{{FeatureName}}Repository.java`
- `application/usecase/{{FeatureName}}UseCase.java`
- `application/command/{{FeatureName}}Command.java`
- `infrastructure/adapter/{{FeatureName}}RepositoryAdapter.java`
- `test/.../{{FeatureName}}UseCaseTest.java`
