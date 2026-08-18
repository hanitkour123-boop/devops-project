# End-to-End DevOps CI/CD and Infrastructure Automation

## Project Overview

This project demonstrates an end-to-end DevOps lifecycle for deploying a containerized application using AWS, Docker, Jenkins, Kubernetes, Terraform, and Ansible.

The project implements source-code management, automated builds, containerization, container image management, Kubernetes deployment, CI/CD automation, infrastructure provisioning, and configuration management.

## Architecture

**GitHub → AWS CodeBuild → Docker → Docker Hub → Kubernetes**

**Jenkins → CI/CD Pipeline**

**Terraform → AWS Infrastructure**

**Ansible → Server Configuration**

## Technologies Used

- Git & GitHub
- AWS CodeBuild
- Docker
- Docker Hub
- Jenkins
- Kubernetes
- Terraform
- Ansible
- AWS

## DevOps Lifecycle

### 1. Git Workflow

Git and GitHub were used for source-code management and version control.

The workflow was designed around development changes being committed to the repository, with releases following the specified release schedule.

### 2. AWS CodeBuild

AWS CodeBuild was configured to trigger the build process when changes were pushed to the designated GitHub branch.

### 3. Docker Containerization

A Dockerfile was used to containerize the application.

A custom Docker image was built from the Dockerfile and the resulting image was published to Docker Hub.

### 4. Kubernetes Deployment

The containerized application was deployed to a Kubernetes cluster.

The deployment was configured with:

- 2 replicas
- Kubernetes Deployment
- NodePort Service
- NodePort: `30008`

### 5. Jenkins CI/CD

A Jenkins Pipeline was created to automate the application build and deployment workflow.

The pipeline coordinates the different stages of the DevOps lifecycle.

### 6. Ansible Configuration Management

Ansible was used for configuration management and automation of server setup.

Playbooks were used to automate the installation and configuration of required software.

### 7. Terraform Infrastructure

Terraform was used to provision infrastructure in AWS using Infrastructure as Code.

This allowed infrastructure resources to be defined and managed through Terraform configuration.

## Project Flow

1. Developer changes are committed to GitHub.
2. AWS CodeBuild is triggered by the repository change.
3. The application is containerized using Docker.
4. A custom Docker image is built.
5. The image is pushed to Docker Hub.
6. Jenkins automates the CI/CD workflow.
7. Kubernetes deploys the container with 2 replicas.
8. A NodePort service exposes the application on port 30008.
9. Terraform is used for AWS infrastructure provisioning.
10. Ansible automates server configuration.

## Key Learning Outcomes

- Practiced Git-based version control and workflow management.
- Implemented automated builds using AWS CodeBuild.
- Containerized applications using Docker.
- Worked with Docker Hub for container image management.
- Deployed containerized applications using Kubernetes.
- Created Jenkins CI/CD pipelines.
- Practiced infrastructure provisioning using Terraform.
- Practiced configuration management using Ansible.
- Gained hands-on experience with an end-to-end DevOps lifecycle.

## Project Screenshots

Screenshots demonstrating the different stages of the DevOps implementation are available in the `screenshots` folder.
