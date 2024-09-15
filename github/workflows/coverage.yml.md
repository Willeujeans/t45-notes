### Scheduled:
Runs daily at 9:14 AM UTC.
### Runs On:
Self-hosted Linux x64 runner.
### Steps:
1. **Checkout Code**: Uses `actions/checkout@v2` to check out the code from the repository.
2. **Run Verification**: Executes the `verify_workflows` script.
3. **Set Up Node.js**: Uses Node.js version 18.x.
4. **Set Up Java**: Uses JDK 11.
5. **Log Commit ID**: Logs the full commit SHA to the GitHub environment.
6. **Install Client Dependencies**: Installs dependencies for the client.
7. **Install Server Dependencies**: Installs dependencies for the server.
8. **Prepare Codeclimate**: Sets up Codeclimate reporting tools.
9. **Run Client Tests**: Executes client-side tests.
10. **Build & Test Server**: Builds and tests server code with Maven.
11. **Report Codeclimate Statistics**: Formats and uploads coverage reports to Codeclimate
