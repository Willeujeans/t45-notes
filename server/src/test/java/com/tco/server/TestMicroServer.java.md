Tests the functionality of the Micro server
**Dependencies**
- Spark framework
- Apache HttpClient
- JUnit (for testing)

**Setup**:
- **`startTheMicroServer`**: before any tests, it starts the `MicroServer` on a dynamic port 
- **`WaitForMicroServerToBeReady`**: Ensures the server is ready before each test
- **`stopTheMicroServer`**: Stops the server after all tests are complete.
**Tests**:
- **`testValidConfigRequest`**: Checks that a valid config request returns a 200 status
- **`testInvalidRequest`**: Checks that an invalid request returns a 400 status
- **`testInvalidEndpoint`**: Checks that an invalid endpoint returns a 404 status