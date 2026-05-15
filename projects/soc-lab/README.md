# 🛡️ SOC-Ready Virtual Machine (Security Operations Center Lab)

[⬅ Back to Portfolio](../../)

## 📌 Overview
This project simulates a lightweight Security Operations Center (SOC) environment with SIEM-like behavior, focusing on real-time event monitoring, detection logic, and incident response workflows.

Unlike traditional static labs, this project includes a **browser-based SIEM simulation engine** that models how SOC analysts interact with security telemetry.

---

## 🎯 Objectives
- Simulate real-time security event ingestion
- Model SIEM-style log processing and alerting
- Demonstrate detection engineering concepts
- Implement basic correlation logic for threat detection
- Replicate SOC analyst workflows in a controlled environment

---

## 🧠 Core Capabilities (SIMULATED SIEM)

### 🔴 1. Event Ingestion Engine
- Continuous generation of system security events
- Authentication, system, and network logs simulated in real time

### 🟡 2. Detection Rules Engine
- Brute-force detection simulation
- SSH failure pattern recognition
- CPU and system anomaly simulation
- Privilege escalation indicators

### 🔵 3. Correlation Layer
- Multi-event pattern detection
- Threshold-based alert escalation
- Behavior-based anomaly grouping

### 🟢 4. SOC Dashboard Simulation
- Live event stream
- Severity classification (INFO / WARN / CRITICAL)
- Event frequency tracking

---

## 🚀 Implementation

### 1. VM Deployment
- Ubuntu Server VM in VirtualBox
- Host-only network isolation
- Minimal resource SOC simulation node

---

### 2. System Hardening
```bash
sudo ufw enable
sudo ufw allow ssh
sudo apt install fail2ban -y
