# Cybersecurity Lab & Projects Repository

## Overview

This repository contains a collection of hands-on cybersecurity projects and laboratory exercises focused on penetration testing, security operations (SOC), and DevSecOps practices. The work demonstrates practical skills in network reconnaissance, vulnerability assessment, log analysis, and secure software development workflows using real-world tools in controlled environments.

The projects are designed for educational and portfolio purposes using isolated virtual lab environments.

---

## 1. Penetration Testing Lab (Primary Project)

### Objective
To identify and analyze security vulnerabilities within a controlled network environment consisting of intentionally vulnerable systems.

### Lab Environment
- Kali Linux (Attacker)
- Metasploitable2 (Vulnerable Linux system)
- Axigen Mail Server (Mail/Web application server)

### Network Range
- 192.168.56.0/24 (Host-only virtual network)

### Tools Used
- Nmap (network scanning)
- Netcat (banner grabbing and manual interaction)
- Wget (web content extraction)
- enum4linux (SMB enumeration)
- Nessus Essentials (vulnerability scanning)
- Curl (HTTPS inspection)

### Key Activities
- Network discovery and port scanning
- Service enumeration (FTP, SSH, HTTP, SMB)
- Web application analysis
- Mail server interface inspection
- Vulnerability identification and CVE research

### Key Findings
- Metasploitable2 exposed multiple outdated and vulnerable services (FTP, Telnet, HTTP, SMB)
- SMB null session access enabled unauthenticated enumeration
- Axigen mail server exposed an administrative web interface over HTTPS
- Multiple critical vulnerabilities identified via Nessus scanning

### Outcome
The project demonstrated how misconfigured and outdated services significantly increase attack surfaces and highlighted the importance of patch management, service hardening, and access control enforcement.

---

## 2. Security Operations Center (SOC) Project

### Objective
To simulate a SOC environment focused on monitoring, detecting, and analyzing security events using log data and alerting mechanisms.

### Focus Areas
- Log aggregation and analysis
- Intrusion detection
- Threat identification
- Incident triage and response

### Tools & Technologies
- Splunk / ELK Stack (Elasticsearch, Logstash, Kibana)
- Wireshark (packet analysis)
- Suricata / Snort (IDS/IPS simulation)
- Windows Event Logs
- Linux Syslog

### Key Activities
- Collection of system and network logs
- Detection of suspicious activities (brute force attempts, port scans)
- Creation of dashboards for security monitoring
- Incident classification and reporting

### Outcome
Developed practical understanding of SOC workflows, including alert investigation, log correlation, and incident response procedures.

---

## 3. DevSecOps Project

### Objective
To integrate security practices into the software development lifecycle (SDLC) by automating security checks in CI/CD pipelines.

### Focus Areas
- Secure coding practices
- Automated vulnerability scanning
- CI/CD security integration
- Infrastructure as Code (IaC) security

### Tools & Technologies
- GitHub Actions / GitLab CI
- Docker
- Trivy (container vulnerability scanning)
- SonarQube (static code analysis)
- Terraform (infrastructure provisioning)
- OWASP Dependency Check

### Key Activities
- Integration of security scanning into CI/CD pipelines
- Container image vulnerability scanning
- Static application security testing (SAST)
- Dependency vulnerability analysis

### Outcome
Demonstrated how security can be embedded into development workflows to detect vulnerabilities early and reduce deployment risks.

---

## Skills Demonstrated

### Penetration Testing
- Network reconnaissance
- Service enumeration
- Vulnerability assessment
- Exploitation awareness
- CVE research

### SOC Operations
- Log analysis
- Intrusion detection
- Incident response fundamentals
- Security monitoring

### DevSecOps
- CI/CD security integration
- Secure development lifecycle
- Container security
- Automated vulnerability scanning

---

## Key Cybersecurity Concepts Covered

- Attack surface analysis
- Enumeration techniques
- Vulnerability management
- CVE and threat intelligence research
- Defense-in-depth strategies
- Security automation principles

---

## Disclaimer

All activities in this repository were performed in isolated virtual environments for educational purposes only. No real-world systems were targeted.

---

## Future Improvements

- Integration of SIEM dashboards (Splunk/ELK)
- Advanced exploitation labs (Metasploit framework)
- Cloud security labs (AWS/Azure)
- Kubernetes security hardening projects
- Threat hunting simulations

---

## Author

Cybersecurity Student / Analyst (Lab Portfolio Project)
