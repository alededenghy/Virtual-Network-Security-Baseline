# Virtual-Network-Security-Baseline

## Overview
This project documents the design, deployment, troubleshooting, and security assessment of a virtualized internal network built as part of an IT and cybersecurity career simulation. The objective was to implement core infrastructure services within a constrained environment, resolve connectivity issues, and establish a baseline security assessment using industry-standard tools.

The project emphasizes practical IT operations, network troubleshooting, and foundational cybersecurity analysis.

---

## Environment & Architecture
The network was deployed as an isolated internal environment using Oracle VirtualBox, with no external internet access.

**Systems included:**
- Firewall / Router (pfSense)
- DNS Server (Linux)
- Web Server (Linux)
- CEO Workstation (Ubuntu 24.04)
- Kali Linux (Trusted and Untrusted)

All systems communicated through an internal virtual network to simulate a private enterprise environment.

---

## Project Objectives
- Deploy a cost-effective virtual network without adding physical hardware
- Troubleshoot routing and DNS resolution issues
- Document system configurations and network settings
- Establish a baseline of exposed services using port scanning
- Analyze insecure protocols and recommend mitigations

---

## Tools & Technologies
- **Oracle VirtualBox**
- **Linux (Ubuntu & Debian-based systems)**
- **pfSense**
- **Nmap**
- **Wireshark**
- **FTP**
- Standard Linux networking utilities

---

## Key Tasks Completed
- Diagnosed and resolved DNS and routing issues on an Ubuntu workstation
- Documented IP addressing, gateways, and DNS configurations across systems
- Transferred files using FTP to verify connectivity and authentication
- Performed internal port scanning to identify exposed services
- Captured and analyzed clear-text FTP credentials using Wireshark
- Established a security baseline for DNS and Web servers
- Developed practical security recommendations based on findings

---

## Security Baseline Summary
- **DNS Server:** Exposed only required DNS services, following least-privilege principles
- **Web Server:** Exposed multiple services, creating a large attack surface
- **FTP Traffic:** Credentials transmitted in clear text and visible via packet capture

These findings represent a baseline snapshot of the environment’s normal behavior and highlight potential security risks.

---

## Recommendations
- Replace FTP with encrypted alternatives such as **SFTP or FTPS**
- Disable or restrict unnecessary services to reduce attack surface
- Enforce encrypted remote administration protocols
- Perform regular port scans to monitor for unauthorized changes
- Apply least-privilege principles to server roles and services

---

## Screenshots & Evidence
Supporting screenshots documenting configuration, scanning results, and traffic analysis are available in the `screenshots/` directory.

---

## Disclaimer
This project was completed in a controlled lab environment for educational and portfolio purposes only. No real production systems or sensitive data were involved.

---
