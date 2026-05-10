# 🛡 Threat Intelligence & Threat Hunting Platform

Threat Intelligence and Threat Hunting platform developed using Wazuh SIEM, Suricata IDS, MISP, VirusTotal, MITRE ATT&CK, and SOAR automation technologies.

This project demonstrates real-world Security Operations Center (SOC) operations including threat detection, intrusion monitoring, threat intelligence integration, cyber attack simulation, incident response, active response automation, and security event correlation across Windows and Linux environments.

Developed as part of an academic cybersecurity project focused on SOC operations, threat intelligence integration, threat hunting, and incident response automation.

---

## 🔍 Key Features

- Centralized SIEM monitoring using Wazuh
- Threat hunting and log analysis
- Suricata IDS integration
- MITRE ATT&CK event mapping
- MISP threat intelligence integration
- VirusTotal malware analysis integration
- File Integrity Monitoring (FIM)
- Vulnerability Detection
- Active Response automation
- SOAR workflow automation using Shuffle
- Simulated cyber attack scenarios
- Incident response playbooks

---

## 🏗 SOC Architecture

The project follows a centralized Security Operations Center (SOC) architecture using Wazuh SIEM, Suricata IDS, threat intelligence integrations, and SOAR automation workflows for threat detection and response.

![SOC Architecture](images/architecture/soc-architecture-diagram.png)

---

## 📊 Security Monitoring Dashboards

### MITRE ATT&CK Dashboard
![MITRE Dashboard](images/dashboards/mitre-attack-dashboard.png)

### Vulnerability Detection Dashboard
![Vulnerability Dashboard](images/dashboards/vulnerability-dashboard.png)

### File Integrity Monitoring Dashboard
![FIM Dashboard](images/dashboards/fim-dashboard.png)

### Threat Hunting Dashboard
![Threat Hunting Dashboard](images/dashboards/threat-hunting-dashboard.png)

---

## ⚔ Attack Simulations & Detection

### Hydra SSH Brute-Force Attack
![Hydra Attack](images/attacks/hydra-bruteforce.png)

### Nmap SYN Scan
![Nmap Scan](images/attacks/nmap-scan.png)

### TCP SYN Flood Attack
![SYN Flood](images/attacks/syn-flood-attack.png)

### ICMP Flood Attack
![ICMP Flood](images/attacks/icmp-flood-attack.png)

---

## 🚨 Threat Detection & Alerts

### TCP SYN Flood Detection
![SYN Flood Alert](images/alerts/syn-flood-alert.png)

### Nmap Scan Detection
![Nmap Alert](images/alerts/nmap-alert.png)

### ICMP Flood Detection
![ICMP Alert](images/alerts/icmp-flood-alert.png)

### Firewall-Drop Active Response
![Firewall Drop](images/alerts/firewall-drop-alert.png)

---

## 🔗 Threat Intelligence & Integrations

### Suricata Custom Rules
![Suricata Rules](images/integrations/suricata-custom-rules.png)

### MISP Integration
![MISP Integration](images/integrations/misp-integration.png)

### VirusTotal Integration
![VirusTotal Integration](images/integrations/virustotal-wazuh-config.png)

---

## 🤖 SOAR Automation with Shuffle

### Shuffle Workflow
![Shuffle Workflow](images/automation/shuffle-workflow.png)

### Shuffle Webhook Integration
![Shuffle Webhook](images/automation/shuffle-webhook.png)

### Automated SSH Alert Handling
![Shuffle SSH Alert](images/automation/shuffle-ssh-alert.png)

---

## ⚙ Technologies Used

### SIEM & Monitoring
- Wazuh SIEM
- Suricata IDS

### Threat Intelligence
- MISP
- VirusTotal
- MITRE ATT&CK

### SOAR & Automation
- Shuffle SOAR
- Wazuh Active Response

### Operating Systems
- Windows
- Ubuntu Linux
- Bodhi Linux
- Kali Linux

### Security Tools
- Sysmon
- Nmap
- Hydra
- hping3

---

## 📘 Incident Response Playbooks

This repository includes incident response playbooks for handling different cybersecurity incidents, including:

- Phishing Attack Response
- Malware Infection Response
- Brute-Force Attack Response

---

## 📂 Repository Structure

```text
threat-intelligence-and-hunting/
│
├── docs/
├── images/
├── playbooks/
├── rules/
├── samples/
└── README.md
```

---

## 🚀 Future Improvements

- Expand SOAR automation workflows
- Integrate additional threat intelligence feeds
- Enhance dashboard visualizations
- Add Sigma rule support
- Implement automated IOC enrichment
- Deploy containerized SOC lab environment
