# Office 365 Module Configuration

## Overview

This document summarizes the Wazuh Office 365 module configuration approach used to integrate Microsoft Office 365 audit monitoring into the SIEM environment.

The configuration enabled centralized collection and monitoring of cloud-related audit events and security activity.

---

# Office 365 Monitoring Objectives

The configuration was designed to:
- Collect Office 365 audit logs
- Monitor authentication activity
- Improve cloud security visibility
- Detect suspicious Office 365 events
- Support SOC monitoring workflows
- Centralize cloud-related security events

---

# Example Office 365 Module Configuration

The Office 365 module was configured within the Wazuh Manager ossec.conf file.

Example configuration structure:

```xml
<office365>
  <enabled>yes</enabled>
  <interval>5m</interval>

  <tenant_id>REDACTED</tenant_id>
  <client_id>REDACTED</client_id>
  <client_secret>REDACTED</client_secret>

  <api_type>commercial</api_type>

  <subscriptions>
    <subscription>Audit.AzureActiveDirectory</subscription>
    <subscription>Audit.Exchange</subscription>
    <subscription>Audit.SharePoint</subscription>
    <subscription>Audit.General</subscription>
    <subscription>DLP.All</subscription>
  </subscriptions>
</office365>
```

---

# Configured Monitoring Areas

The integration included monitoring for:
- Azure Active Directory activity
- Exchange audit events
- SharePoint activity
- General Office 365 audit events
- Data Loss Prevention (DLP) events

This enabled centralized monitoring of cloud-related activity alongside endpoint and server security events.

---

# Monitoring Benefits

The Office 365 integration improved:
- Hybrid environment visibility
- Authentication monitoring
- Audit log collection
- Threat investigation capabilities
- Centralized SOC monitoring

The integration also enhanced visibility into cloud-based user activity and administrative operations.

---

# Security Considerations

Sensitive information including:
- Tenant identifiers
- Client IDs
- Client secrets
- Organizational information

has been removed or redacted for security and privacy purposes.

---

# References

- [Wazuh Office 365 Monitoring Documentation](https://documentation.wazuh.com/current/cloud-security/office365/index.html?utm_source=chatgpt.com)
- [Office 365 Management Activity API Documentation](https://learn.microsoft.com/en-us/office/office-365-management-api/office-365-management-activity-api-reference?utm_source=chatgpt.com)
