# File Integrity Monitoring (FIM) Configuration

## Overview

This document summarizes example File Integrity Monitoring (FIM) configurations used within the Wazuh SIEM environment.

The configurations were designed to monitor sensitive directories, detect unauthorized modifications, and improve visibility into critical file activity.

---

# Windows File Share Monitoring

The File Share Server agent was configured to monitor sensitive directories in real time using the Wazuh syscheck module.

Example configuration:

```xml
<directories check_all="yes" report_changes="yes" realtime="yes">
F:\
</directories>
```

This configuration enabled:
- Real-time monitoring
- File modification detection
- Change reporting
- Recursive directory monitoring

---

# Linux Application Directory Monitoring

The Linux Application Server was configured to monitor important application directories.

Example configuration:

```xml
<directories whodata="yes">/opt/application</directories>
```

This configuration improved visibility into:
- Application file modifications
- Unauthorized changes
- User-related file activity

---

# Linux Web Directory Monitoring

The Linux Web Server was configured to monitor the web root directory hosting web applications and websites.

Example configuration:

```xml
<directories whodata="yes">/www/wwwroot</directories>
```

This configuration supported:
- Web file integrity monitoring
- Website modification detection
- Suspicious web activity monitoring

---

# Monitoring Benefits

The FIM configurations improved:
- Security visibility
- Threat detection capabilities
- Incident investigation support
- Compliance-related monitoring
- Detection of unauthorized modifications

The monitoring also supported SOC operations by correlating file activity with other security events collected by Wazuh.

---

# Security Considerations

Sensitive information including:
- Real directory structures
- Internal server details
- Organizational identifiers
- Infrastructure information

has been removed or generalized for security and privacy purposes.

---

# References

- [Wazuh File Integrity Monitoring Documentation](https://documentation.wazuh.com/current/user-manual/capabilities/file-integrity/index.html?utm_source=chatgpt.com)
