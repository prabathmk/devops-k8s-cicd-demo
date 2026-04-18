# DevOps CI/CD Pipeline with Kubernetes Deployment

## Overview
This project demonstrates a simple DevOps pipeline integrating Docker, Kubernetes, and CI/CD concepts.

## Tech Stack
- Docker
- Kubernetes
- Jenkins / GitLab CI
- AWS (optional)

## Features
- Containerized application using Docker
- Kubernetes deployment with YAML configuration
- Automated CI/CD pipeline for build and deployment

## How to Run

1. Build Docker image:
   docker build -t my-app .

2. Deploy to Kubernetes:
   kubectl apply -f deployment.yaml
   kubectl apply -f service.yaml

## Project Structure
- Dockerfile
- deployment.yaml
- service.yaml
- Jenkinsfile (optional)

## Screenshots

### Application Output
screenshots/app-output.png

### Kubernetes Pods
screenshots/k8s-pods.png

### Kubernetes Service
screenshots/k8s-service.png

## Author
Prabath Kariyawasam
