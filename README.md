# Containerization of a 3-tier Web Application

## Project Description
This project involves the containerization of a 3-tier web application consisting of a frontend (Angular), backend (Java/Spring), and a MySQL database. The source code for this application is available in the following repositories: [frontend]([https://github.com/bezkoder/angular-16-crud-example]) and [backend]([https://github.com/bezkoder/spring-boot-data-jpa-mysql]).

## Completed Tasks
1. **MySQL Database Containerization**
   - Created a container for the MySQL database using the official MySQL image.
   - Chose the most suitable storage option and ensured persistent storage for the database.

2. **Backend Dockerization**
   - Created a Dockerfile for the Backend project following best practices.
   - Applied good practices such as using multi-stage builds, minimizing layers, and specifying version pinning for dependencies.

3. **Frontend Dockerization**
   - Created a Dockerfile for the Frontend project and applied best practices (similar to the Backend Dockerfile).

4. **Docker Network**
   - Created a Docker network with an appropriate driver and connected the MySQL database container to this network.

5. **Image Security and Publishing**
   - Scanned Docker images for vulnerabilities and took necessary actions to mitigate them.
   - Published Docker images to Docker Hub for both Backend and Frontend projects.

6. **Application Deployment**
   - Successfully deployed the application using docker-compose.
   - Created docker-compose.yml file defining services for frontend, backend, and MySQL database.
   - Ensured application functionality by testing in the browser.

7. **Kubernetes Deployment**
   - Created Kubernetes manifests (YAML files) for deploying the application in a Kubernetes cluster
   - Configured resource quotas, RBAC controls, health checks, and ingress for the application.
   - Tested application functionality in Kubernetes cluster.

8. **Private Docker Image Registry**
   - Created a local private Docker image registry to store and manage built images.

