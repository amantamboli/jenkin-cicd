
# Jenkins Pipeline for Python Flask Application with Argo CD and Kubernetes

## Introdcution
A Monitoring App, developed using Flask and empowered by a streamlined CI/CD pipeline orchestrated with Jenkins, Docker, Argo CD, and Kubernetes. This monitoring application is designed to provide real-time insights into your system's performance, offering a seamless experience for tracking and managing key metrics.


## CI/CD Pipeline Overview


CI/CD pipeline, created with Jenkins and ArgoCD, ensures the smooth and automated delivery of updates to the Monitoring App. The pipeline consists of the following key stages:

### 1.  Building Docker Image
Jenkins orchestrates the creation of a Docker image for the Monitoring App from the provided Dockerfile. This guarantees a consistent and reproducible environment for your application.

### 2. Pushing Image to Docker Hub
Once the Docker image is built, Jenkins seamlessly pushes it to Docker Hub, making it readily available for deployment and distribution.

### 3. Running SonarQube Analysis
Before deployment, our pipeline includes a stage for SonarQube analysis. This ensures code quality and identifies potential issues early in the development process. Jenkins interacts with SonarQube to provide detailed insights into the codebase.

### 4. Updating Manifests Repository
The next stage involves updating the manifests repository with the latest version of the Monitoring App. Jenkins takes charge here, ensuring that the manifests are always synchronized with the most recent changes.

## Continuous Deployment with Argo CD and Kubernetes
CD process is managed by Argo CD, which automates the deployment of the Monitoring App to a Kubernetes cluster. Argo CD reads the updated manifests files updated by Jenkins, ensuring that Kubernetes environment is always up to date with the latest version of the application.

This collaborative integration of Jenkins, Docker, SonarQube, Argo CD, and Kubernetes establishes a powerful and efficient workflow.


## Project Structure

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)


## Author

- [@amantamboli](https://amantamboli.github.io/portfolio/)

