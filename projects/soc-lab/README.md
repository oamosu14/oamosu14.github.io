# 🛡️ SOC-Ready Virtual Machine (Security Operations Center Lab)

[⬅ Back to Portfolio](../../)

## 📌 Overview
This project builds a hardened Linux-based SOC environment for monitoring, detection, and incident response operations aligned with industry frameworks such as NIST and CIS Controls.

---

## 🎯 Objectives
- Deploy secure SOC VM
- Enable centralized logging and monitoring
- Implement SIEM capabilities
- Support incident response lifecycle
- Integrate threat intelligence feeds

---

## 🚀 Implementation

### 1. VM Deployment
- Ubuntu Server VM created in VirtualBox
- Host-only network configuration for isolation
- Optimized system resource allocation

---

### 2. System Hardening
```bash
sudo ufw enable
sudo ufw allow ssh
sudo apt install fail2ban -y
