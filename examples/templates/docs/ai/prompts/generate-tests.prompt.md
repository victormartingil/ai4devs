---
name: generate-tests
description: Generate comprehensive tests for a given class
input: Class file path
output: Test file
---

# Generate Tests

Given the source file at `{{FILE_PATH}}`, generate comprehensive tests that:

1. Cover all public methods
2. Test happy path scenarios
3. Test error/exception scenarios
4. Test boundary values
5. Mock all external dependencies
6. Follow the naming convention: `method_scenario_expectedResult`
7. Use the project's testing framework

Output the test file with proper imports and setup.
