
# 🛡️ Wazuh SIEM Security Operations Lab

![SIEM](https://img.shields.io/badge/SIEM-Wazuh-blue)
![Deployment](https://img.shields.io/badge/Deployment-Docker-blue)
![Framework](https://img.shields.io/badge/MITRE-ATT%26CK-red)
![Focus](https://img.shields.io/badge/SOC-Blue%20Team-green)

---

## 👋 Project Overview

This project is a hands-on **Security Operations (SOC) simulation lab** built using **Wazuh SIEM deployed via Docker** in a virtualized environment.

The goal of this lab is to simulate real-world SOC operations by monitoring endpoints, detecting malicious activity, investigating security incidents, and mapping findings to the **MITRE ATT&CK framework**.

This project demonstrates practical experience in:

* Security monitoring and log analysis
* Threat detection and incident investigation
* Threat hunting across endpoint telemetry
* SOC workflow simulation using SIEM tools

---

## 🏗️ Lab Architecture

The environment was built using a multi-system SOC simulation setup:

* Wazuh Manager (Central SIEM Server)
* Wazuh Dashboard (Security Monitoring Interface)
* Wazuh Indexer (Log Storage & Search)
* Windows 11 Endpoint Agent
* Ubuntu Server Endpoint
* Docker & Docker Compose
* VirtualBox (Virtualized Environment)

---

## ⚔️ Attack Scenarios Simulated

To simulate real-world adversary behavior, the following attack scenarios were executed:

* SSH Brute Force Attack (Credential Access)
* Windows Authentication Failure Attempts
* Unauthorized File Modification Events
* Registry Modification (Persistence Attempt)
* Suspicious Endpoint Activity (Linux & Windows)

---

## 🔍 SOC Investigation Activities

Within this lab, I performed SOC-level security operations including:

* Real-time monitoring of security events in Wazuh Dashboard
* Log analysis across Windows and Linux endpoints
* Investigation of authentication anomalies and attack patterns
* Threat hunting using filters and log correlation techniques
* Incident timeline reconstruction based on event data
* Identification of compromised or suspicious behavior

---

## 🧠 MITRE ATT&CK Mapping

All detected security events were mapped to adversary techniques using the MITRE ATT&CK framework:

| Technique                       | ID    | Description                                      |
| ------------------------------- | ----- | ------------------------------------------------ |
| Brute Force                     | T1110 | Repeated authentication attempts against systems |
| Valid Accounts                  | T1078 | Use of legitimate credentials for access         |
| Command & Scripting Interpreter | T1059 | Execution of system-level commands               |
| Data Manipulation               | T1565 | Unauthorized modification of system files        |
| Defense Evasion                 | T1562 | Attempts to bypass security controls             |

---

## 🧾 Sample Incident Summary

### 🚨 Brute Force Attack Detection

* **Detection Source:** Wazuh Authentication Logs
* **Event Type:** Repeated SSH login failures
* **Behavior Observed:** Multiple failed login attempts within a short time window
* **Analysis:** Pattern consistent with brute force credential attack
* **MITRE Mapping:** T1110 – Brute Force
* **Outcome:** Attack behavior successfully identified through SIEM monitoring

---

## 📸 Evidence & Screenshots

Screenshots of alerts, dashboards, and investigations are included in the `/screenshots` directory.

They demonstrate:

* Wazuh alert detection dashboard
* Authentication failure events
* File integrity monitoring alerts
* Security event timelines

---

## 🧠 Key Skills Demonstrated

* SIEM deployment and configuration (Wazuh)
* Security event monitoring and alert analysis
* Threat detection and behavioral analysis
* MITRE ATT&CK-based mapping and classification
* Incident investigation and root cause analysis
* Threat hunting using log correlation

---

## 📊 Outcome of Project

This lab strengthened my ability to:

* Translate raw logs into actionable security insights
* Detect and investigate simulated cyberattacks
* Apply structured SOC investigation methodologies
* Operate within a MITRE ATT&CK-driven detection framework
* Simulate real-world SOC workflows in a controlled environment

---

## 🚀 Future Improvements

* Integration of active threat intelligence feeds
* Custom Wazuh detection rule creation
* SOAR automation for alert response workflows
* Expanded multi-agent attack simulation environment

---


## 👤 Author

**Olaide Jamal**
SOC Analyst | SIEM Engineer | Threat Hunter | Incident Response

---

## 📫 Connect With Me

* LinkedIn: [https://linkedin.com/in/olaide-jamal](https://linkedin.com/in/olaide-jamal)

---

