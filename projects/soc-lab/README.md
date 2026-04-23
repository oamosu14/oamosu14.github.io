# 🛡️ SOC-Ready Virtual Machine (Security Operations Center Lab)

## 📌 Overview

This project builds a hardened Linux-based SOC environment designed for security monitoring, incident detection, threat intelligence, and response operations.

It aligns with industry frameworks:
- NIST Cybersecurity Framework
- ISO 27001
- CIS Controls

---

## 🎯 Objectives

- Deploy secure SOC VM
- Enable log collection and monitoring
- Implement SIEM tools
- Support incident response lifecycle
- Integrate threat intelligence feeds

---

# 🚀 FULL IMPLEMENTATION

---

## 1. VM Deployment

- Create Ubuntu Server VM in VirtualBox
- Assign isolated network (host-only)
- Allocate secure system resources

---

## 2. System Hardening

```bash
sudo ufw enable
sudo ufw allow ssh
sudo apt install fail2ban -y

---

## 3. Secure SSH Configuration

sudo nano /etc/ssh/sshd_config

Set:
PermitRootLogin no
PasswordAuthentication no


Restart service:

sudo systemctl restart ssh

4. Log Management

Enable system logging:

sudo systemctl enable rsyslog


Monitor logs:

cat /var/log/auth.log
