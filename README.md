# 🔐 Enterprise SOC Incident Investigation Lab  
### End-to-End Attack Detection & Root Cause Analysis

## Badge 

![SIEM](https://img.shields.io/badge/SIEM-Wazuh-blue)
![Platform](https://img.shields.io/badge/Platform-Windows%2011-lightgrey)
![Attack-Simulation](https://img.shields.io/badge/Attack-Simulation-red)
![SOC](https://img.shields.io/badge/SOC-Incident%20Response-green)

## 📌 Project Overview

This project simulates a real-world enterprise security incident involving a multi-stage attack chain.  
The objective is to detect, investigate, and perform root cause analysis using SIEM log correlation and Windows event monitoring.

The lab replicates a realistic SOC (Security Operations Center) investigation workflow at L2 level.

---

## 🖥️ Lab Architecture

| Machine | Role | Purpose |
|----------|--------|----------|
| Kali Linux | Attacker | Simulate brute force attacks |
| Windows 11 | Victim | Target system (Sysmon enabled) |
| Wazuh SIEM | Log Monitoring | Detection, correlation & alerting |

All systems are configured in an isolated internal network to simulate an enterprise SOC environment.

---

## 🚨 Attack Simulation Stages

### 1️⃣ Initial Access – Brute Force (MITRE T1110)

- Simulated repeated authentication failures
- Analyzed Windows Event ID 4625 (Failed Logon)
- Identified successful login (Event ID 4624)
- Detected abnormal login patterns in Wazuh

---

### 2️⃣ Privilege Escalation (MITRE T1068)

- Modified local administrator group membership
- Investigated Event ID 4732 (User added to Admin group)
- Validated unauthorized privilege assignment

---

### 3️⃣ Persistence Mechanism (MITRE T1053)

- Created scheduled task for persistence
- Added registry Run key
- Monitored Sysmon logs for system modification events

---

## 🔎 Investigation & Log Correlation

The investigation included:

- Authentication log analysis
- Privilege change monitoring
- Scheduled task creation tracking
- Registry modification detection
- Timeline reconstruction
- Indicator of Compromise (IOC) extraction
- MITRE ATT&CK mapping

Attack Flow Identified:

Brute Force → Successful Login → Privilege Escalation → Persistence Established

---

## 📊 Detection Sources

- Windows Security Event Logs
- Sysmon Logs
- Wazuh Alerts
- Authentication & Group Policy Logs

---

## 📄 Incident Response Report

A professional L2-level incident report was created including:

- Executive Summary
- Detailed Timeline
- MITRE ATT&CK Mapping
- Indicators of Compromise
- Root Cause Analysis
- Remediation Recommendations

---

## 🛠️ Tools & Technologies Used

- Wazuh SIEM
- Sysmon
- Windows Event Viewer
- Kali Linux
- Hydra (for brute force simulation)
- VirtualBox Lab Environment

---

## 🎯 Skills Demonstrated

- SIEM Monitoring & Alert Analysis
- Windows Log Investigation
- Log Correlation Techniques
- Threat Detection & Attack Chain Analysis
- Incident Documentation (L2 Level)
- MITRE ATT&CK Framework Mapping

---

## 📌 Key Takeaways

This lab demonstrates the ability to:

- Detect multi-stage attacks in an enterprise environment
- Correlate logs across different event sources
- Perform structured incident investigations
- Produce professional SOC-level documentation

---

## 🚀 Author

Cybersecurity Enthusiast | SOC Analyst Aspirant  
Focused on Blue Teaming, Threat Detection, and Incident Response
