# Dashboard Design

## Overview

This document summarizes the design and purpose of the custom dashboards created within the Wazuh SIEM environment.

The dashboards were designed to improve security visibility, simplify threat monitoring, support SOC workflows, and enhance security event analysis across monitored systems.

---

# Dashboard Objectives

The dashboard environment was designed to:
- Centralize security visibility
- Improve threat detection monitoring
- Support SOC-style workflows
- Monitor endpoint health and activity
- Visualize security trends
- Track suspicious activity
- Improve incident investigation efficiency

---

# Endpoint Security Monitoring Dashboard

The Endpoint Security Monitoring Dashboard focused on endpoint-related security events and agent visibility.

Configured monitoring areas included:
- Top alert types
- Top affected agents
- Failed authentication attempts
- Vulnerability trends
- Agent health monitoring
- Compliance-related events

This dashboard improved visibility into endpoint security posture and operational monitoring.

---

# File Integrity Monitoring Dashboard

The File Integrity Monitoring Dashboard focused on:
- File modifications
- File additions and deletions
- Frequently modified paths
- User activity related to file changes
- Real-time integrity monitoring

This dashboard improved visibility into unauthorized changes and suspicious file activity.

---

# Office 365 Security Monitoring Dashboard

The Office 365 Dashboard focused on:
- Authentication activity
- Office 365 alerts
- Exchange activity
- SharePoint activity
- DLP-related events
- Geographical alert distribution
- Suspicious mailbox activity

This improved cloud security visibility and centralized monitoring capabilities.

---

# Overview Dashboard

The Overview Dashboard provided high-level visibility into:
- Alert severity distribution
- Agent connection status
- Alert trends
- Top alerting agents
- MITRE ATT&CK tactics

The goal of this dashboard was to provide a quick operational overview of the security environment.

---

# Threat Detection & Response Dashboard

The Threat Detection & Response Dashboard focused on:
- High-severity alerts
- MITRE ATT&CK techniques
- Network attack visibility
- Threat prioritization
- Critical alert monitoring
- Suspicious activity investigation

This dashboard supported SOC analysts by improving visibility into active threats and attack behaviors.

---

# Dashboard Design Benefits

The custom dashboard approach improved:
- Security event visibility
- Threat analysis workflows
- SOC operational awareness
- Security monitoring efficiency
- Incident investigation capabilities
- Alert prioritization

The dashboards also simplified the analysis of large volumes of security events collected across endpoints, servers, and cloud services.

---

# Security Considerations

Sensitive information including:
- Internal hostnames
- Real IP addresses
- Usernames
- Organizational identifiers
- Operational alert data

has been removed or generalized for security and privacy purposes.

---

# Conclusion

The custom dashboard implementations enhanced the Wazuh SIEM environment by improving centralized visibility, supporting security monitoring operations, and enabling more effective threat detection and response workflows.
