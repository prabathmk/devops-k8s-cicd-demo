# DevOps CI/CD Pipeline with Kubernetes Deployment

## Overview
This project demonstrates a simple DevOps pipeline integrating Docker, Kubernetes, and CI/CD concepts.

## Architecture

GitHub → Jenkins → Docker → Docker Hub → Kubernetes (Minikube)

## Tech Stack
- Docker
- Kubernetes
- Jenkins / GitLab CI
- AWS (optional)

## CI/CD Pipeline

This project includes a Jenkins pipeline that:

- Builds Docker image from source code
- Pushes image to Docker Hub
- Deploys application to Kubernetes cluster

Note: For local testing, deployment was executed manually using kubectl and Minikube.

## Features
- Containerized application using Docker
- Kubernetes deployment with YAML configuration
- Automated CI/CD pipeline for build and deployment

## Project Structure
- app/
- Dockerfile
- deployment.yaml
- service.yaml
- Jenkinsfile (optional)

## How to Run

### 1. Build Docker image:
docker build -t prabathmkdocker/devops-demo:v2 .
   
Docker Image: prabathmkdocker/devops-demo:v2
   
### 2. Push to Docker Hub:
docker push prabathmkdocker/devops-demo:v2

### 3. Deploy to Kubernetes
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

### 4. Access Application
minikube service devops-demo-service

## Outcome
Successfully deployed a containerized application to Kubernetes using Minikube, demonstrating end-to-end DevOps workflow including containerization, orchestration, and CI/CD pipeline integration.

## Screenshots

### Application Output
![App Output](screenshots/app-output.png)

*Application deployed on Kubernetes using Minikube*

### Kubernetes Pods
![Pods](screenshots/k8s-pods.png)

### Kubernetes Service
![Service](screenshots/k8s-service.png)

## Author
Prabath Kariyawasam
