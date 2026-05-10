# Password-Based Agent Enrollment Configuration

## Overview

This document summarizes the configuration approach used to enable password-based Wazuh agent enrollment.

The configuration was implemented to simplify secure agent onboarding and centralized enrollment management.

---

# Authentication Configuration

The Wazuh Manager authentication settings were modified within the ossec.conf configuration file to enable password-based authentication.

Example configuration:

```xml
<auth>
  <use_password>yes</use_password>
</auth>
```

This configuration enabled agents to authenticate during enrollment using a predefined shared password.

---

# Authentication Password File

A dedicated authentication password file was configured on the Wazuh Manager to store the enrollment password used during agent registration.

Example configuration approach:

```bash
echo <REDACTED_PASSWORD> > /var/ossec/etc/authd.pass
```

---

# File Permissions & Security

Appropriate permissions and ownership configurations were applied to restrict unauthorized access to the authentication password file.

Example commands:

```bash
chmod 640 /var/ossec/etc/authd.pass
chown root:wazuh /var/ossec/etc/authd.pass
```

---

# Service Restart

After configuration updates, the Wazuh Manager service was restarted to apply the new authentication settings.

Example command:

```bash
systemctl restart wazuh-manager
```

---

# Security Considerations

Sensitive information including:
- Real passwords
- IP addresses
- Internal infrastructure details
- Organizational identifiers

has been removed or redacted for security and privacy purposes.

---

# References

- [Wazuh Password Authentication Documentation](https://documentation.wazuh.com/current/user-manual/agent/agent-enrollment/security-options/using-password-authentication.html?utm_source=chatgpt.com)
