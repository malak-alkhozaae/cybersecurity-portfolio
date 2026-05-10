# Sample Security Alerts

## ICMP Flood Detection Alert

```json
{
  "rule": {
    "id": "100101",
    "level": 10,
    "description": "Suricata detected possible ICMP flood activity"
  },
  "agent": {
    "name": "Bodhi-Agent"
  },
  "srcip": "192.168.56.101",
  "event_type": "alert"
}
```

---

## TCP SYN Flood Detection Alert

```json
{
  "rule": {
    "id": "100102",
    "level": 10,
    "description": "Suricata detected possible TCP SYN flood activity"
  },
  "agent": {
    "name": "Bodhi-Agent"
  },
  "srcip": "192.168.56.101",
  "event_type": "alert"
}
```

---

## Nmap SYN Scan Detection Alert

```json
{
  "rule": {
    "id": "100103",
    "level": 8,
    "description": "Suricata detected possible Nmap SYN scan activity"
  },
  "agent": {
    "name": "Bodhi-Agent"
  },
  "srcip": "192.168.56.101",
  "event_type": "alert"
}
```

---

## Brute-Force SSH Detection Alert

```json
{
  "rule": {
    "level": 12,
    "description": "Multiple failed SSH login attempts detected"
  },
  "agent": {
    "name": "Ubuntu-Agent"
  },
  "srcip": "192.168.56.120",
  "decoder": {
    "name": "sshd"
  }
}
```
