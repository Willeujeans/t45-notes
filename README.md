This is a shortened version of the README found in the t45 project.
### Run Locally
  ```bash
  ./bin/run.sh
  ```
This executes the shell script [[run.sh]]
Starting the client on port 431XX and the server on port 413XX, XX will be the team number
The browser should open and display the project.
### Updating Website
- **Description**: Default mode for developing and testing. The browser auto-refreshes with code changes, but the server needs a restart for updates.
### Production
- **Description**: Optimized for end users. JavaScript is minified and resources are packaged. This helps with performance but may hide code details.
- **How to Run**: Use the script with the `-e prod` flag:
  ```bash
  ./bin/run.sh -e prod
  ```
  This installs dependencies, bundles JavaScript, compiles code, and starts the server on port 413XX.
### Deployment
- **Description**: To prepare for deployment, package the application into a single JAR file.
- **How to Package**: Use the script with the `-d` flag:
  ```bash
  ./bin/run.sh -d
  ```
  This creates a JAR file in the `target` directory that you can deploy on any machine with Java.