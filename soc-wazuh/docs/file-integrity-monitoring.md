# File Integrity Monitoring (FIM)

## Overview

This document summarizes the implementation of File Integrity Monitoring (FIM) within the Wazuh SIEM environment.

The implementation focused on monitoring sensitive directories, detecting unauthorized file modifications, and improving visibility into potential security incidents across monitored systems.

---

# Implementation Objectives

The File Integrity Monitoring configuration was implemented to:
- Detect unauthorized file modifications
- Monitor sensitive directories
- Improve visibility into system changes
- Support threat detection and incident investigation
- Identify suspicious file activity
- Enhance compliance and security monitoring

---

# File Share Server Monitoring

A dedicated File Share Server agent was configured to monitor sensitive directories and file activity in real time.

The monitoring configuration included:
- Real-time monitoring
- File modification detection
- File addition and deletion tracking
- Detailed change reporting

The monitored directories were configured within the Wazuh agent ossec.conf file using the syscheck module.

Example monitoring capabilities included:
- File creation monitoring
- File deletion monitoring
- File modification detection
- User activity visibility

Reference Resources:
- [Wazuh File Integrity Monitoring Documentation](https://documentation.wazuh.com/current/user-manual/capabilities/file-integrity/index.html?utm_source=chatgpt.com)

---

# Linux Server File Monitoring

Linux application and web servers were configured to monitor:
- Application directories
- Web root directories
- Critical system paths
- Important configuration files

The monitoring configuration improved visibility into unauthorized changes affecting applications and hosted websites.

---

# Real-Time Monitoring Configuration

The Wazuh syscheck module was configured to support:
- Real-time file monitoring
- Change reporting
- Integrity validation
- Recursive directory monitoring

This enabled immediate visibility into suspicious file activity and unauthorized modifications.

---

# Security Monitoring Benefits

The FIM implementation improved:
- Detection of unauthorized file changes
- Threat visibility
- Incident investigation support
- Monitoring of critical systems
- Compliance-related monitoring
- Security auditing capabilities

The integration also supported SOC workflows by correlating file changes with other security events collected by Wazuh.

---

# Security Considerations

Sensitive information such as:
- Internal file paths
- Organizational directory structures
- Server identifiers
- Internal infrastructure information

has been removed or generalized for security and privacy purposes.

---

# Conclusion

The File Integrity Monitoring implementation enhanced the overall security monitoring capabilities of the Wazuh environment by improving visibility into critical file activity, suspicious modifications, and system integrity changes across monitored servers and endpoints.
