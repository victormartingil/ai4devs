<!-- This file is tool-agnostic. Copy as CLAUDE.md, GEMINI.md, or use directly as AGENTS.md. -->

# Project Context

## Tech Stack
- {{STACK}}

## Architecture
{{ARCHITECTURE}}. NEVER mix business logic in adapters or controllers.

Package structure:
- `{{DOMAIN_PACKAGE}}/` — entities, value objects, ports, domain events
- `{{APPLICATION_PACKAGE}}/` — use cases, commands, queries, DTOs
- `{{INFRASTRUCTURE_PACKAGE}}/` — adapters, configuration, persistence, messaging

## Code Conventions
- {{INJECTION_CONVENTION}}
- {{IMMUTABILITY_CONVENTION}}
- {{DTO_CONVENTION}}
- Tests: {{TEST_FRAMEWORK}}, naming: {{TEST_NAMING_CONVENTION}}
- {{NULL_HANDLING_CONVENTION}}
- {{EXCEPTION_CONVENTION}}

## What you must NEVER do
- Do not add dependencies without being asked
- Do not make automatic commits
- Do not mix responsibilities between layers
- {{CUSTOM_CONSTRAINT_1}}
- {{CUSTOM_CONSTRAINT_2}}
- {{CUSTOM_CONSTRAINT_3}}
