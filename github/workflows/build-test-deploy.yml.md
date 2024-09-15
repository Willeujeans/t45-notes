### Triggers:
- **Pull Request**: This 'workflow' will run on pull requests targeting the `main` branch
- **Release**: This 'workflow' will run when a release is published.
### Runs On:
- self-hosted runner with these specifications.
- Node.js version `18.x`.
#### Steps
1. Release Soundness Checks(correct sprint date release tag)
2. Pull Request Soundness Checks
3. Prepare for Checkout
4. Checks out Code
5. Set Up Node.js
6. Set Up Java
7. Install Client Dependencies
8. Install Server Dependencies
9. Prepare Codeclimate Reporting Tools
10. Run Client Tests
11. Bundle Client with Webpack
12. Build & Test Server with Maven
13. Postman Tests
14. Deploy Server
15. Finish and Report Codeclimate Statistics