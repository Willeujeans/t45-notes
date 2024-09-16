Tests the `JSONValidator` class for JSON schema validation
**Dependencies**:
- JUnit (for testing)
- Mockito (for mocking static methods)
- Everit JSON Schema (for schema validation)
**Tests**:
- **`testConfigRequestFail`**: Tests that a minimal JSON (`{}`) fails validation for `ConfigRequest`
- **`testConfigRequestPass`**: Tests that a valid JSON for `ConfigRequest` passes schema validation
- **`testMissingSchema`**: Tests that attempting to validate with an invalid schema fails
	`test("", JSONValidator.class, false);`
- **`testInvalidSchema`**: Tests if the schema loading throws a `SchemaException` validation should fails (Mockito is used to mock `SchemaLoader` to throw an exception)