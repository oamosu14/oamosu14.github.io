# 🖥️ Home Lab Mini Data Center (Virtualized Infrastructure Platform)

[⬅ Back to Portfolio](../../)

## 📌 Overview
This project builds a scalable virtual infrastructure platform that simulates an enterprise data center environment using Linux virtualization.

It is designed to run multiple services, support automation, and simulate real-world enterprise infrastructure.

---

## 🏗️ Architecture
Physical Host → Hypervisor → Multiple Linux VMs → Service Layer → Automation Layer

---

## 🚀 Implementation

### 1. Hypervisor Setup
- Installed VirtualBox / Proxmox
- Enabled virtualization (VT-x / AMD-V)
- Configured networking:
  - Bridged network (external access)
  - Internal network (isolated services)

### 2. VM Deployment Strategy
- Web Server Node
- Database Node
- Security Node
- Automation Node

### 3. Network Segmentation
- Isolates traffic between services
- Improves security posture
- Mimics enterprise architecture

### 4. Central Services
- SSH remote management
- File sharing (NFS / Samba)
- Optional DNS services

### 5. Automation Layer
- Ansible for configuration management
- Cron jobs for scheduled automation tasks

### 6. Remote Access
- SSH key-based authentication
- Secure access enforcement (no password login)

### 7. Scalability
- VM templates for rapid deployment
- Standardized configurations
- Expandable architecture

---

## 🧰 Tools Used
- Ubuntu Server
- VirtualBox / Proxmox
- SSH
- Ansible
- NFS / Samba
- Cron

---

## 📊 Outcome
- Enterprise-style virtual infrastructure
- Isolated multi-service environment
- Automation-enabled data center simulation
