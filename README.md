# Fossa Analyser

This is a simple Node.js application with a GitLab CI/CD pipeline that includes a FOSSA scan.

## Getting Started

1.  Clone the repository.
2.  Install the dependencies:
    ```
    npm install
    ```
3.  Run the application:
    ```
    npm start
    ```
    The application will be available at `http://localhost:3000`.

## GitLab CI/CD

The `.gitlab-ci.yml` file defines the CI/CD pipeline for this project. It includes a `fossa-scan` job that scans the project's dependencies for license and vulnerability issues using FOSSA.

To use the FOSSA scan, you need to set the `FOSSA_API_KEY` CI/CD variable in your GitLab project's settings. You can get this key from your FOSSA account.

The scan will run automatically on every merge request and push to the main branch. 