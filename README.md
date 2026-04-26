# TaskMind - Deployment & Infrastructure

## 📝 Overview
This repository serves as the central hub for **Infrastructure-as-Code (IaC)**, containerization strategies, and orchestration manifests for the TaskMind ecosystem. It provides the necessary tools to provision, manage, and deploy the entire microservices architecture seamlessly across different environments.

## 🚀 Key Responsibilities
* **Container Orchestration:** Managing `docker-compose` configurations for local development and cohesive integration testing.
* **Production Readiness:** Providing robust orchestration manifests (e.g., **Kubernetes** YAMLs, Helm charts) for deploying services to staging and production.
* **Configuration Management:** Centralizing environment variables, networking policies, and persistent volume definitions across the distributed system.
* **Security & Secrets:** Implementing secure strategies for managing sensitive data and service-to-service communication.

## 🛠 Tech Stack
* **Containerization:** Docker & Docker Desktop
* **Orchestration:** Docker Compose 
* **CI/CD:** GitHub Actions



## 🏗 Architecture Context
This repository provides the "blueprint" for the TaskMind platform. It allows developers to spin up the following stack with a single command:
1.  **Infrastructure:** Databases (PostgreSQL/MongoDB) & Discovery Services.
2.  **Core Services:** User, Task, and AI Agent services.
3.  **Entry Point:** API Gateway & UI Client.

## 📦 Getting Started

### Prerequisites
* **Docker** and **Docker Compose** installed.
* [אופציונלי] **kubectl** for Kubernetes deployments.

### Local Spin-up
To launch the entire TaskMind ecosystem locally, navigate to the root directory and run:

```bash
# Pull images and start the distributed system
docker-compose up -d

# Check the status of all services
docker-compose ps
