Tests the behavior and validation of the `WebApplication` class in [[WebApplication.java]]
**Dependencies**:
- JUnit (for testing)
- SystemLambda (to capture system exit)
**Tests**:
- **`testTooManyCommandLineArgs`**: Tests if command-line arguments > 1: application exits with status 1
- **`testPortIsValid`**: Tests that a port number within the valid range is considered valid
- **`testPortIsInvalidLow`**: Tests that a port number below the minimum valid range is considered invalid
- **`testPortIsInvalidHigh`**: Tests that a port number above the maximum valid range is considered invalid
- **`testGetServerPortDefault`**: Tests that no command-line arguments defaults to the predefined server port
- **`testGetServerPortSpecifiedValid`**: Tests that a specified port number is used correctly if it’s within the valid range
- **`testGetServerPortSpecifiedNotInteger`**: Tests that a non-integer command-line argument defaults to the predefined server port
- **`testGetServerPortSpecifiedOutOfRange`**: Tests that a port number out of the valid range defaults to the predefined server port
