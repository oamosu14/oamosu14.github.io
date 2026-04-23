
---

# 🖥️ 2. HOME LAB MINI DATA CENTER (FULL VERSION)

📁 `projects/home-lab-data-center/README.md`

---

```markdown
# 🖥️ Home Lab Mini Data Center (Virtualized Infrastructure Platform)

## 📌 Overview

This project builds a scalable virtual infrastructure platform that simulates an enterprise data center environment using Linux virtualization.

It is designed to run continuously, host multiple services, and support automation and remote management.

---

## 🏗️ Architecture Design

Physical Host → Hypervisor → Multiple Linux VMs → Service Layer → Automation Layer

---

# 🚀 FULL IMPLEMENTATION

---

## 1. Hypervisor Setup

- Install VirtualBox or Proxmox
- Enable virtualization (VT-x/AMD-V)
- Configure networking:
  - Bridged network (external access)
  - Internal network (isolated services)

---

## 2. VM Deployment Strategy

Create multiple Linux VMs:

- Web Server Node
- Database Node
- Security Node
- Automation Node

---

## 3. Network Segmentation


✔ Isolates traffic  
✔ Improves security  
✔ Mimics enterprise architecture  

---

## 4. Central Services

- SSH remote management
- File sharing (NFS/Samba)
- DNS services (optional)

---

## 5. Automation Layer

- Ansible for configuration management
- Cron jobs for scheduled automation tasks

---

## 6. Remote Access Setup

- SSH key-based authentication
- Secure login only (no passwords)
- Optional VPN access for remote control

---

## 7. Scalability Design

- VM templates for fast deployment
- Standardized OS configuration
- Easy expansion without redesign

---

# 🧰 Tools Used

- Ubuntu Server
- VirtualBox / Proxmox
- SSH
- Ansible
- NFS / Samba
- Cron

---

# 📊 Outcome

- Built enterprise-style virtual infrastructure
- Implemented isolated multi-service environment
- Enabled automation and remote administration
- Designed scalable data center architecture



