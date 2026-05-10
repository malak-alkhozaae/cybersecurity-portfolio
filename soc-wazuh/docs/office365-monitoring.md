# Office 365 Monitoring

## Overview

This document summarizes the integration of Microsoft Office 365 audit monitoring into the Wazuh SIEM environment.

The implementation focused on collecting and monitoring Office 365 security events, audit logs, authentication activity, and cloud-related security events to improve centralized visibility and threat detection capabilities.

---

# Integration Objectives

The Office 365 integration was implemented to:
- Centralize cloud audit monitoring
- Improve visibility into authentication activity
- Monitor administrative actions
- Detect suspicious Office 365 activity
- Support security investigations and threat detection
- Enhance SOC monitoring capabilities

---

# Azure AD Application Registration

A dedicated Azure AD application was registered to allow Wazuh to securely collect Office 365 audit logs through Microsoft APIs.

The implementation included:
- Azure AD application registration
- Tenant integration
- Client secret generation
- API permission assignment
- Secure authentication configuration

Integrated monitoring components included:
- Azure Active Directory events
- Exchange activity logs
- SharePoint activity logs
- General Office 365 audit activity
- Data Loss Prevention (DLP) related events

---

# API Permissions Configuration

The integration required specific Office 365 Management API permissions to allow centralized audit log collection.

The following monitoring areas were configured:
- ActivityFeed.Read
- ActivityFeed.ReadDlp

These permissions enabled visibility into organizational activity and DLP-related events across the Office 365 environment.

Reference Resources:
- [Microsoft Entra ID Documentation](https://learn.microsoft.com/en-us/entra/fundamentals/whatis?utm_source=chatgpt.com)
- [Office 365 Management Activity API Documentation](https://learn.microsoft.com/en-us/office/office-365-management-api/office-365-management-activity-api-reference?utm_source=chatgpt.com)

---

# Wazuh Office 365 Configuration

The Wazuh Manager was configured to collect Office 365 audit events using the Office 365 module configuration inside the ossec.conf file.

Configured subscription types included:
- Audit.AzureActiveDirectory
- Audit.Exchange
- Audit.SharePoint
- Audit.General
- DLP.All

This configuration enabled centralized collection and monitoring of cloud-related security events.

Reference Resources:
- [Wazuh Office 365 Monitoring Documentation](https://documentation.wazuh.com/current/cloud-security/office365/index.html?utm_source=chatgpt.com)

---

# Security Monitoring Benefits

The integration improved:
- Cloud visibility
- Authentication monitoring
- Suspicious activity detection
- Audit log analysis
- Centralized security monitoring
- Threat investigation workflows

This allowed Office 365 events to be monitored alongside endpoint and server security events within a single SIEM platform.

---

# Security Considerations

Sensitive information including:
- Tenant identifiers
- Client secrets
- Organizational information
- Authentication credentials

has been removed or generalized for security and privacy purposes.

---

# Conclusion

The Office 365 integration enhanced the Wazuh SIEM environment by extending security monitoring capabilities into cloud services, improving centralized visibility, audit monitoring, and threat detection across hybrid environments.
