---
applyTo: "**/*_test.go"
---
# Project general coding standards
Write in Go. Use latest available Go version.

## Naming Conventions
- Use github.com/golang/mock/gomock and github.com/stretchr/testify/assert and github.com/stretchr/testify/require.
- Name test cases in snake_case.
- Do not use Finish method on instances of gomock.Controller.
- For error assertions use testutil package and include the error message from the function and the error from the mock if present.
- Do not use explicit 'if' or 'switch' conditional statements.
- When creating mock objects, return the created object from the function rather than using output parameters.
- Always guard calls to yield function with 'if' and 'return' instructions.
