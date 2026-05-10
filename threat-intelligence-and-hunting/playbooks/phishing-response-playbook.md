# Phishing Attack Response Playbook

## Objective
Identify, investigate, contain, and respond to phishing emails targeting users within the organization.

## Scope
This playbook applies to suspected or confirmed phishing incidents, including credential harvesting emails, malicious links, malicious attachments, and business email compromise attempts.

## Incident Categories
- Credential harvesting emails
- Malicious links or attachments
- Business Email Compromise (BEC)
- User-reported suspicious emails

## Detection Sources
- Email security gateway alerts
- User-reported suspicious emails
- Wazuh SIEM alerts
- Threat intelligence indicators
- Suspicious URL or domain reputation results

## Response Procedure

### 1. Detection
- Review reported phishing email or generated SIEM alert.
- Identify sender address, subject, URLs, attachments, and affected users.
- Check whether the email was delivered to multiple users.

### 2. Analysis
- Inspect email headers.
- Analyze URLs and domains using threat intelligence sources.
- Check attachments using malware analysis tools where applicable.
- Search SIEM logs for related activity, such as suspicious login attempts or endpoint alerts.

### 3. Containment
- Remove the phishing email from affected mailboxes.
- Block malicious sender addresses, domains, or URLs.
- Disable compromised accounts if credentials were entered.
- Isolate affected endpoints if malware execution is suspected.

### 4. Eradication
- Remove malicious files or artifacts from affected systems.
- Revoke active sessions and reset passwords for compromised users.
- Apply additional email filtering rules if needed.

### 5. Recovery
- Restore affected accounts after password reset and verification.
- Re-enable access after confirming no further suspicious activity.
- Monitor affected users and systems for follow-up indicators.

### 6. Post-Incident Review
- Document the phishing attempt, affected users, indicators, and response actions.
- Update detection rules and awareness materials.
- Review email security controls and improve filtering where needed.

## Roles and Responsibilities
- SOC Analyst: Initial triage, alert review, and escalation.
- IT Administrator: Account remediation and mailbox cleanup.
- Security Engineer: Blocking, rule tuning, and technical investigation.
- Incident Response Lead: Coordination, communication, and final review.

## Validation
- Conduct phishing simulation exercises periodically.
- Review and update the playbook after real incidents or major control changes.
