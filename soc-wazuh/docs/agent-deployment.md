# Agent Deployment

## Overview

This document summarizes the deployment and configuration process for integrating Windows and Linux systems into the Wazuh SIEM environment.

The deployment focused on centralized agent management, automated installation methods, authentication configuration, and endpoint monitoring integration.

---

# Windows Endpoint Deployment

## Deployment Approach

Windows endpoint agents were deployed using Group Policy Object (GPO) deployment methods to support centralized and scalable installation across multiple systems.

The deployment process included:
- Preparing the Wazuh MSI installer
- Configuring deployment transforms using Orca
- Defining Wazuh Manager connection settings
- Applying deployment policies through Active Directory Group Policy

Reference Resources:
- [Windows SDK - Windows App Development](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/?utm_source=chatgpt.com)
- [Wazuh Packages List & Installation Guide](https://documentation.wazuh.com/current/installation-guide/index.html?utm_source=chatgpt.com)

---

## Deployment Configuration

The deployment configuration included:
- Wazuh Manager address configuration
- Authentication server configuration
- TCP communication protocol
- Password-based agent enrollment

The deployment package was customized using Microsoft Orca to automate installation settings and simplify large-scale deployment.

Additional Resources:
- [Microsoft Orca MSI Tool Documentation](https://learn.microsoft.com/en-us/windows/win32/msi/orca-exe?utm_source=chatgpt.com)

---

## Group Policy Object (GPO) Deployment

GPO deployment was configured to:
- Install Wazuh agents automatically
- Apply deployment transforms
- Start Wazuh services automatically
- Enforce policy updates during system startup

This approach enabled centralized endpoint onboarding and simplified operational management.

Additional Resources:
- [Microsoft Group Policy Documentation](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/manage/group-policy/group-policy-overview?utm_source=chatgpt.com)

---

# Windows Server Deployment

Windows Server systems were integrated using the same centralized deployment methodology.

Additional focus was placed on:
- Service reliability
- Startup policy enforcement
- Recovery configuration
- Consistent policy application

Recovery actions were configured to automatically restart Wazuh services during failures to improve operational stability.

---

# Linux Agent Deployment

## Integrated Linux Systems

Linux agents were deployed to:
- Application servers
- Web servers

These systems were integrated with the Wazuh Manager for centralized monitoring and log collection.

---

## Linux Monitoring Configuration

Linux agent configurations included:
- Application log monitoring
- Web server log monitoring
- File Integrity Monitoring (FIM)
- System activity monitoring

Important directories and log sources were configured for continuous monitoring and security analysis.

Reference Resources:
- [Wazuh Linux Agent Installation Guide](https://documentation.wazuh.com/current/installation-guide/wazuh-agent/wazuh-agent-package-linux.html?utm_source=chatgpt.com)

---

# File Share Server Integration

A dedicated File Share Server agent was configured to support:
- Real-time File Integrity Monitoring
- File change detection
- Monitoring of sensitive directories
- Security event reporting

This configuration improved visibility into unauthorized file changes and suspicious activity.

Reference Resources:
- [Wazuh File Integrity Monitoring Documentation](https://documentation.wazuh.com/current/user-manual/capabilities/file-integrity/index.html?utm_source=chatgpt.com)

---

# Security Considerations

Sensitive deployment information such as:
- IP addresses
- Credentials
- Domain names
- Organizational identifiers

has been removed or generalized for security and privacy purposes.

---

# Conclusion

The deployment process demonstrated practical experience with enterprise-scale endpoint onboarding, centralized monitoring integration, GPO-based deployment, Linux agent management, and File Integrity Monitoring using Wazuh SIEM.
