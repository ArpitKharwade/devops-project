# 🚀 DevOps CI/CD Project – Docker & Kubernetes with GitHub Actions

This project demonstrates an end-to-end DevOps workflow where a Node.js Express application is containerized using Docker, automated with GitHub Actions CI/CD, and prepared for deployment on Kubernetes.

The project is implemented without using AWS, Azure, Google Cloud, or Jenkins, focusing purely on core DevOps tools and concepts.

---

## 📌 Project Overview

- Build a simple Node.js Express web application
- Containerize the application using Docker
- Automate Docker image build & push using GitHub Actions
- Prepare Kubernetes Deployment and Service manifests
- Demonstrate CI/CD, containerization, and orchestration

---

## 🛠️ Tech Stack Used

- Backend: Node.js, Express.js  
- Containerization: Docker  
- CI/CD: GitHub Actions  
- Orchestration: Kubernetes (Minikube)  
- Version Control: Git, GitHub  

---

## ⚙️ Application Details

- Runs a Node.js Express server
- Exposes port 3000
- Includes a health check endpoint for Kubernetes readiness

### Endpoints
- `/` → Application status  
- `/health` → Health check  

---

## 🐳 Docker Workflow

- Application is containerized using a Dockerfile
- Docker image is built and pushed to Docker Hub
- Uses node:18-alpine base image for lightweight containers

---

## 🔄 CI/CD Pipeline (GitHub Actions)

The CI/CD pipeline automatically runs on every push to the main branch.

Pipeline steps:
1. Checkout source code
2. Login to Docker Hub using GitHub Secrets
3. Build Docker image
4. Push Docker image to Docker Hub

Secrets used:
- DOCKER_USERNAME
- DOCKER_PASSWORD (Docker Hub Access Token)

---

## ☸️ Kubernetes Deployment

The application is deployed using Kubernetes manifests:

- Deployment for pod management and self-healing
- Service for exposing the application

Features:
- Replication
- Self-healing
- Service-based networking

---

## 🎯 Key Learnings

- CI/CD automation using GitHub Actions
- Secure credential management using GitHub Secrets
- Docker image build and registry push
- Kubernetes deployments, services, and self-healing
- Real-world DevOps workflow without cloud dependency
