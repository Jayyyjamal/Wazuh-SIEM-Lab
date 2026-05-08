# 🚨 SOC Incident Report: Privileged Group Membership Changes Detected

## 📌 Incident Overview

| Field | Value |
|---|---|
| Incident ID | SOC-2026-003 |
| Detection Platform | Wazuh SIEM |
| Severity Level | High |
| Category | Privilege Escalation / Account Manipulation |
| Detection Date | April 19, 2026 |
| Analyst | Olaide Jamal |
| Status | Investigated |

---

# 🧾 Executive Summary

During routine monitoring within the Wazuh SIEM environment, multiple Windows Security Event IDs associated with privileged group membership changes were detected from a monitored Windows endpoint.

The alerts indicated that a user account was added to privileged local groups including:

- Administrators
- Users

This activity is significant because unauthorized modification of privileged groups can enable attackers to escalate privileges, maintain persistence, and gain broader system access.

The events were identified, analyzed, and correlated using Wazuh log monitoring and Windows Security Event logs.

---

# 🖥️ Affected System

| Asset | Value |
|---|---|
| Hostname | DESKTOP-BI8QLCH |
| Agent Name | Windows |
| Agent ID | 001 |
| IP Address | 192.168.56.1 |
| Monitoring Tool | Wazuh Agent |

---

# 🚨 Detection Details

## Event IDs Observed

| Event ID | Description |
|---|---|
| 4728 | Member added to a security-enabled global group |
| 4732 | Member added to a security-enabled local group |
| 4733 | Member removed from a security-enabled local group |

---

# 🔍 Investigation Timeline

| Time (UTC) | Activity |
|---|---|
| 20:12:59 | Event ID 4732 detected |
| 20:13:03 | Event ID 4728 detected |
| 20:13:03 | Event ID 4733 detected |
| 20:15:00 | Alert triage initiated |
| 20:20:00 | Event correlation completed |

---

# 📸 Evidence Collected

## Event ID 4732 — User Added to Local Group

![Event ID 4732](../screenshots/eventid4732.png)

### Observations
- Wazuh detected Event ID 4732
- A user account was added to a local security-enabled group
- Target username identified:
```text
Administrators
