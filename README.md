# Next.js JWT Auth - DevOps Demo

A demo Next.js application with JWT authentication used to demonstrate Docker containerization, Kubernetes deployment, and CI/CD practices.

## 🎯 Purpose

This is a sample application created for DevOps learning and demonstration purposes, showcasing:
- Docker containerization
- Kubernetes manifest configuration
- CI/CD pipeline implementation

## 🛠 Tech Stack

- **Application**: Next.js 14 + TypeScript + MongoDB (Prisma)
- **Authentication**: JWT with bcryptjs
- **Containerization**: Docker
- **Orchestration**: Kubernetes
- **CI/CD**: GitHub Actions

## 🚀 Quick Start

### Using Docker

```bash
# Pull the image
docker pull ghcr.io/aadip26/nextjs-jwt-auth-app:latest

# Create .env file with required variables
cp env.example .env

# Run with Docker Compose
docker-compose up -d
```

Access at: http://localhost:3000

### Using Kubernetes

```bash

# Apply configurations
kubectl apply -f k8s/secrets.yaml
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
kubectl apply -f k8s/ingress.yaml

# Verify
kubectl get pods
kubectl get svc

```

