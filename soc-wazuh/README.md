# 🛡 SOC Implementation using Wazuh SIEM

## 📌 Overview

This project demonstrates the implementation of a Security Information and Event Management (SIEM) solution using Wazuh in an enterprise-style environment. The system was designed to centralize log collection, monitor endpoint activity, and support real-time threat detection and analysis.

The implementation was carried out in both an academic environment and a practical internship environment, providing hands-on exposure to enterprise-level monitoring, troubleshooting, and security operations.

---

## 🎯 Objective

To design and deploy a centralized monitoring solution capable of collecting, analyzing, and correlating security events across multiple systems, supporting SOC operations and improving overall security visibility.

---

## 🛠 Environment

- Wazuh Manager deployed on Ubuntu Linux (Virtualized using VMware)
- Windows endpoints and servers
- Two monitored Linux servers (application and web services)
- Application and web activity monitoring
- Office 365 cloud activity monitoring
- Virtualized environment configured to support enterprise-level monitoring (approximately 20–40 endpoints)

---

## ⚙️ Implementation

- Installed and configured Wazuh Manager on a Linux server
- Deployed Wazuh agents across endpoints and servers
- Monitored multiple systems including endpoints, servers, applications, and web services
- Used Group Policy Objects (GPO) for centralized agent deployment
- Configured File Integrity Monitoring (FIM) to detect unauthorized file changes
- Integrated Microsoft Office 365 logs for centralized cloud monitoring
- Built dashboards to monitor system activity, alerts, and endpoint status

---

## 📊 Security Monitoring Dashboards

Custom dashboards were created to provide focused visibility across different areas of the environment. Each dashboard was designed to support monitoring, detection, and analysis of security events.

### 🔹 Endpoint Security Monitoring
- Monitors alerts, agent activity, and authentication events
- Identifies top affected endpoints and attacker IPs
- Tracks vulnerabilities and system status changes over time

### 🔹 File Integrity Monitoring (FIM)
- Tracks file modifications (added, modified, deleted)
- Identifies users performing file changes
- Highlights frequently modified file paths
- Detects unauthorized or suspicious file activity

### 🔹 Office 365 Security Monitoring
- Monitors user activity and security alerts in the cloud environment
- Identifies suspicious login behavior and failed operations
- Tracks user-based alert trends and geographical activity

### 🔹 Environment Overview Dashboard
- Provides high-level visibility of alerts and system health
- Displays alert severity distribution and agent status
- Highlights top alert-generating systems

### 🔹 Threat Detection & Response
- Focuses on high-severity alerts and active threats
- Maps detected activity to MITRE ATT&CK techniques
- Identifies common attack patterns and network-based threats

---

## ⚠️ Challenges & Solutions

### Wazuh Manager Service Issues
- Investigated inactive manager service issues through system log analysis
- Resolved configuration-related problems affecting service availability

### Agent Connectivity Issues
- Identified agent communication and enrollment problems
- Manually reconfigured affected agents and validated connectivity

---

## 🧠 Skills Demonstrated

- SIEM implementation and configuration
- Log analysis and security monitoring
- Threat detection and investigation
- Endpoint and server monitoring
- File Integrity Monitoring (FIM)
- Office 365 security monitoring
- Linux administration
- Troubleshooting and problem-solving in practical environments

---

## 📸 Screenshots

Due to the project being conducted within a practical enterprise-style environment, screenshots cannot be shared to protect sensitive information and system confidentiality.

---

## 🚀 Future Improvements

- Implement automated alert response mechanisms
- Enhance dashboard visualization for improved threat analysis
- Expand monitoring coverage across additional systems and endpoints
- Integrate additional threat intelligence and alert correlation capabilities

---

## 📄 Full Documentation

Detailed step-by-step implementation and configurations are available in the sanitized project documentation below:

📄 [View Full Documentation](soc-wazuh/docs/Wazuh.pdf)
