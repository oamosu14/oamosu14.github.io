# ⚙️ Multi-Node CI/CD Pipeline (DevSecOps Architecture)

## 📌 Overview

This project implements a multi-node CI/CD pipeline in a Linux-based environment to automate secure software delivery. The pipeline integrates code quality checks, security scanning, containerization, deployment automation, and monitoring.

---

# 🏗️ Architecture

The pipeline follows a distributed DevSecOps model:

GitHub → CI Server → Security Scanners → Docker Build → Registry → Deployment Node → Monitoring Stack

---

# 🚀 Step-by-Step Implementation

## 1. Source Code Management

- Code is hosted on GitHub
- Webhooks trigger CI pipeline on push events

---

## 2. CI Pipeline Setup (Jenkins / GitHub Actions)

- Pull latest code from repository
- Trigger automated build stages

---

## 3. Code Quality Check (Linting)

```bash
npm install eslint
npx eslint .
