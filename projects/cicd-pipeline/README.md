# ⚙️ Multi-Node CI/CD Pipeline (DevSecOps Architecture)

[⬅ Back to Portfolio](../../)

## 📌 Overview
This project implements a multi-node CI/CD pipeline in a Linux-based environment to automate secure software delivery. The pipeline integrates code quality checks, security scanning, containerization, deployment automation, and monitoring.

---

## 🏗️ Architecture
GitHub → CI Server → Security Scanners → Docker Build → Registry → Deployment Node → Monitoring Stack

---

## 🚀 Implementation Steps

### 1. Source Code Management
- Code is hosted on GitHub
- Webhooks trigger CI pipeline on push events

### 2. CI Pipeline (Jenkins / GitHub Actions)
- Pull latest code from repository
- Trigger automated build stages

### 3. Code Quality Check (Linting)
- Installed and executed ESLint for code validation
- Enforced coding standards before build stage

### 4. Security Scanning
- Integrated static and dependency vulnerability scanning tools

### 5. Containerization
- Application packaged using Docker
- Built images stored in container registry

### 6. Deployment
- Automated deployment to target Linux nodes
- Zero-touch deployment workflow

### 7. Monitoring
- Integrated system monitoring for deployed services

---

## 📊 Outcome
- Fully automated CI/CD pipeline
- Integrated security into delivery lifecycle (DevSecOps)
- Reduced manual deployment errors
