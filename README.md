# 🛡️ Wazuh SIEM Lab

![SIEM](https://img.shields.io/badge/SIEM-Wazuh-blue)
![Docker](https://img.shields.io/badge/Deployment-Docker-blue)
![MITRE](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red)
![SOC](https://img.shields.io/badge/Focus-SOC%20Analysis-green)

---

# 📌 Overview

This project documents my hands-on Wazuh SIEM lab built to simulate real-world SOC operations.

The lab focuses on:
- Threat detection
- Log analysis
- Threat hunting
- MITRE ATT&CK mapping
- Security monitoring

---

# 🎯 Objectives

- Deploy and configure Wazuh SIEM using Docker
- Ingest and analyze endpoint security logs
- Detect attack techniques
- Conduct threat hunting
- Improve SOC analyst skills

---

# 🏗️ Lab Architecture

```text
+----------------------+
|   Wazuh Manager      |
|     Ubuntu Server    |
+----------+-----------+
           |
           |
+----------v-----------+
|    Windows Agent     |
| Endpoint Monitoring  |
+----------------------+
```

---

# ⚙️ Technologies Used

- Wazuh SIEM
- Docker
- Ubuntu Linux
- Windows 11
- MITRE ATT&CK Framework
- VirtualBox

---

# 🚨 Detection Use Cases

## Registry Modification (Persistence)
Detected suspicious registry modifications linked to persistence techniques.

### MITRE ATT&CK
T1112 – Modify Registry

---

## File Deletion (Defense Evasion)
Monitored unauthorized file deletions and destructive behavior.

### MITRE ATT&CK
T1070 – Indicator Removal on Host

---

## Data Destruction (Impact)
Detected destructive actions affecting system integrity.

### MITRE ATT&CK
T1485 – Data Destruction

---

# 🔍 Threat Hunting

Conducted threat hunting using:
- Process monitoring
- Registry monitoring
- Service analysis
- Log correlation
- Alert investigation

---

# 📊 Key Skills Demonstrated

- SIEM Deployment
- Log Analysis
- Threat Detection
- Threat Hunting
- MITRE ATT&CK Mapping
- SOC Operations
- Security Monitoring

---

# 📸 Screenshots

## MITRE ATT&CK Dashboard
![MITRE](screenshots/mitre-dashboard.png)

## Threat Hunting Dashboard
![Threat Hunting](screenshots/threat-hunting.png)

## GDPR Monitoring
![GDPR](screenshots/gdpr-dashboard.png)

---

# 🧠 Lessons Learned

This project helped me:
- Understand real-world SOC workflows
- Improve SIEM analysis skills
- Develop threat hunting techniques
- Gain hands-on cybersecurity experience

---

# 🚀 Future Improvements

- Build custom Wazuh detection rules
- Add automated alerting
- Expand cloud monitoring
- Integrate threat intelligence feeds

---

# 👤 Author

Olaide Jamal

Aspiring SOC Analyst | Cybersecurity Enthusiast
