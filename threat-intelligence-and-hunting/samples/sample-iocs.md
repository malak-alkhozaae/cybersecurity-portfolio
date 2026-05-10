# Sample Indicators of Compromise (IOCs)

## Malicious IP Addresses

```text
192.168.56.101
192.168.56.120
```

---

## Suspicious Domains

```text
malicious-example[.]com
phishing-login[.]net
fake-update[.]org
```

---

## Malicious File Hashes

```text
44d88612fea8a8f36de82e1278abb02f
275a021bbfb6489e54d471899f7db9d1
```

---

## MITRE ATT&CK Techniques Referenced

| Technique ID | Description |
|---|---|
| T1046 | Network Service Scanning |
| T1078 | Valid Accounts |
| T1498 | Network Denial of Service |
| T1070.004 | File Deletion |
| T1548.003 | Abuse Elevation Control Mechanism |

---

## Detection Sources

- Wazuh SIEM
- Suricata IDS
- VirusTotal
- Sysmon
- File Integrity Monitoring (FIM)
- Threat Intelligence Feeds
