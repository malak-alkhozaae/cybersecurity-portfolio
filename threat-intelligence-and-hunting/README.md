# 🛡 Threat Intelligence & Threat Hunting Platform

Threat Intelligence | Threat Hunting | Wazuh SIEM | MISP | Suricata | MITRE ATT&CK | Incident Response

---

## 📌 Overview

This project demonstrates the design and implementation of a threat intelligence and threat hunting platform using Wazuh SIEM as the main monitoring and analysis solution. The platform was developed to support proactive threat detection, security event correlation, IOC analysis, and incident investigation within a controlled cybersecurity lab environment.

The project integrates multiple security components, including threat intelligence sources, network intrusion detection, vulnerability detection, file integrity monitoring, and attack simulation. It focuses on improving visibility across monitored systems and supporting SOC-style investigation workflows.

---

## 🎯 Objective

To build a centralized security monitoring and threat hunting environment capable of detecting, analyzing, and investigating suspicious activities using SIEM logs, threat intelligence indicators, and security event correlation.

---

## 🛠 Tools & Technologies

- Wazuh SIEM
- MISP Threat Intelligence Platform
- VirusTotal
- Suricata IDS/IPS
- MITRE ATT&CK Framework
- Linux
- Windows
- Nmap
- hping3
- Virtualized lab environment

---

## ⚙️ Implementation

### SIEM Deployment & Monitoring
- Deployed Wazuh SIEM for centralized log collection and security monitoring
- Configured monitored endpoints to forward security events to the SIEM
- Analyzed alerts, logs, and system activity through the Wazuh dashboard

### Threat Intelligence Integration
- Integrated threat intelligence concepts using MISP and VirusTotal
- Investigated Indicators of Compromise (IOCs)
- Used threat intelligence data to support alert enrichment and analysis

### Network Threat Detection
- Integrated Suricata IDS/IPS for network-based threat detection
- Monitored suspicious traffic patterns and network-based alerts
- Analyzed attack behavior generated through controlled simulations

### Threat Hunting
- Performed proactive threat hunting using logs and security alerts
- Investigated suspicious activities and abnormal behavior
- Mapped relevant attack techniques to MITRE ATT&CK

### Vulnerability & File Monitoring
- Used vulnerability detection to identify weaknesses in monitored systems
- Configured File Integrity Monitoring to detect unauthorized file changes
- Reviewed generated alerts to support investigation workflows

### Incident Response & Playbooks
- Documented SOC-style investigation steps
- Created basic response workflows for detected threats
- Supported analysis using alert correlation and threat context

---

## 📸 Screenshots

Screenshots and diagrams will be added here after the project documentation is finalized.

---

## 🚀 Future Improvements

- Add more threat intelligence feeds
- Create custom detection rules
- Expand MITRE ATT&CK mapping
- Build threat hunting dashboards
- Improve automated response workflows
- Add more attack simulation scenarios
