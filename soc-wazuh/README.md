# 🛡 SOC Implementation using Wazuh SIEM

## 📌 Overview

This project demonstrates the implementation of a Security Information and Event Management (SIEM) solution using Wazuh in an enterprise environment. The system was designed to centralize log collection, monitor endpoint activity, and support real-time threat detection and analysis.

The implementation was carried out in both an academic environment and a real-world internship setting, with the latter providing practical exposure to enterprise-level monitoring and troubleshooting.

---

## 🎯 Objective

To design and deploy a centralized monitoring solution capable of collecting, analyzing, and correlating security events across multiple systems, supporting SOC operations and improving overall security visibility.

---

## 🛠 Environment

- Wazuh Manager deployed on Ubuntu Linux (Virtualized using VMware)
- Windows endpoints and servers
- Two monitored servers (including application and web services)
- Application and web activity monitoring
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

- **Wazuh Manager service became inactive**  
  → Investigated system logs and resolved configuration-related issues  

- **Agent connectivity issues**  
  → Identified misconfigurations and manually reconfigured affected agents  

- **Version compatibility issues**  
  → Adjusted configurations to ensure stable system performance  

---

## 🧠 Skills Demonstrated

- SIEM implementation and configuration  
- Log analysis and security monitoring  
- Threat detection and investigation  
- Endpoint and server monitoring  
- Troubleshooting and problem-solving in real environments  

---

## 📸 Screenshots

*(Sanitized screenshots of dashboards, alerts, and agent status will be added here)*

---

## 🚀 Future Improvements

- Implement automated alert response mechanisms  
- Enhance dashboard visualization for improved threat analysis  
- Expand monitoring coverage across additional systems and endpoints  

---

## 📄 Full Documentation

Detailed step-by-step implementation and configurations are available in a separate document (sanitized for security purposes).
