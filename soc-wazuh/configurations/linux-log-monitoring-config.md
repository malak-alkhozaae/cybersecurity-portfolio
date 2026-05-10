# Linux Log Monitoring Configuration

## Overview

This document summarizes example Linux log monitoring configurations implemented within the Wazuh SIEM environment.

The configuration focused on monitoring application logs, web server logs, and critical Linux system activity to improve centralized visibility and threat detection capabilities.

---

# Application Log Monitoring

The Linux Application Server was configured to collect application-specific logs for centralized analysis within Wazuh.

Example configuration:

```xml
<localfile>
  <log_format>syslog</log_format>
  <location>/var/log/application.log</location>
</localfile>
```

This configuration enabled:
- Application activity monitoring
- Log collection and analysis
- Security event visibility
- Centralized monitoring

---

# Web Server Log Monitoring

The Linux Web Server was configured to monitor web-related logs, including access and error events.

Example configuration:

```xml
<localfile>
  <log_format>syslog</log_format>
  <location>/var/wwwlogs/nginx_error.log</location>
</localfile>

<localfile>
  <log_format>syslog</log_format>
  <location>/var/wwwlogs/nginx_access.log</location>
</localfile>
```

This monitoring configuration improved visibility into:
- Web application activity
- Server errors
- Suspicious requests
- Web-related security events

---

# Centralized Monitoring Benefits

The Linux log monitoring implementation improved:
- Security visibility
- Threat detection capabilities
- Log correlation
- Incident investigation workflows
- Centralized event analysis

The integration also supported SOC operations by consolidating Linux server activity into a centralized SIEM environment.

---

# Security Considerations

Sensitive information including:
- Real server names
- Internal infrastructure paths
- Organizational information
- Production log details

has been removed or generalized for security and privacy purposes.

---

# References

- [Wazuh Log Data Collection Documentation](https://documentation.wazuh.com/current/user-manual/capabilities/log-data-collection/index.html?utm_source=chatgpt.com)
