# Kubernetes Deployment Using Minikube and Docker  

This project demonstrates the setup of a Kubernetes cluster using Minikube and Docker, followed by the deployment of a Flask application as a service. The commands executed in this project are structured into a narrative to guide you through the entire process.  

## Table of Contents  
- [Features](#features)  
- [Directory Structure](#directory-structure)  
- [Setup Workflow](#setup-workflow)  
- [Commands Breakdown](#commands-breakdown)  
- [Deployment Story](#deployment-story)  
- [Testing the Application](#testing-the-application)  
- [Contributing](#contributing)  
- [Contact](#contact)  

## Features  
- Deploying a Kubernetes cluster locally using Minikube.  
- Docker installation and configuration for Kubernetes compatibility.  
- Flask application deployment as a Kubernetes service.  
- Accessing the application via a NodePort service.  

## Directory Structure  
```bash  
project-folder/  
├── deployment.yaml       # Kubernetes deployment file  
├── service.yaml          # Kubernetes service file  
├── node-port-service.yaml # Service with NodePort configuration  

## Setup Workflow

### Install Docker and Minikube
- **Install Docker**: Enables containerization for application deployment.
- **Install Minikube**: Manages a local Kubernetes cluster.

### Configure Docker
1. **Start and enable Docker service**: Ensure Docker is running.
2. **Add current user to Docker group**: Allows managing Docker without requiring `sudo`.

### Set Up Minikube
1. **Start Minikube**: Use Docker as the driver for the local Kubernetes cluster.
2. **Install kubectl**: Required for managing Kubernetes resources.

### Create Kubernetes Resources
1. **Define YAML files**: Write deployment and service configurations.
2. **Apply configurations**: Use `kubectl` to deploy the resources to the cluster.

### Access the Application
- Use **Minikube's IP** and **NodePort** to access the deployed Flask application.
