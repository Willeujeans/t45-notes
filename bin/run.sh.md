contains the shell script to run the website

1. **Setup and Environment Configuration:**
    - Sets file creation permissions to `077` (`umask 077`).
    - Sources a configuration script if available (`/etc/profile.d/modules.sh`).
    - Loads a specific module (`courses/cs314`) if on a CS-department machine.
    - Defines and exports server and client ports based on environment variables.
2. **Utility Functions:**
    - **`check_error`**: Checks if a command failed and exits with an error if so.
    - **`realpath`**: Resolves the absolute path of a file.
    - **`get_repo_root_dir`**: Finds the root directory of a Git repository.
    - **`get_nfs_mounted`**: Checks if the repository is on an NFS mount.
    - **`get_default_prefix`**: Sets a default build directory prefix depending on NFS mount status.
3. **Dependency Installation:**
    - **`install_client_dependencies`**: Installs Node.js dependencies for the client application.
    - **`install_server_dependencies`**: Installs Maven dependencies for the server application.
4. **Build and Test Functions:**
    - **`bundle_client`**: Bundles the client-side code for production.
    - **`build_server`**: Builds the server-side code using Maven.
    - **`run_client_tests`**: Runs tests for the client application.
    - **`run_server_and_hotloader`**: Starts the server with hot reloading in development mode.
    - **`run_server`**: Starts the server in production mode.
    - **`postman_tests`**: Runs Postman tests on the server if Postman collections are present.
5. **Script Execution:**
    - Parses command-line arguments for environment options (development or production).
    - Cleans and sets up target directories depending on whether the build is on an NFS mount.
    - Installs dependencies, runs client tests, builds the server, and then runs the appropriate server mode based on the environment.