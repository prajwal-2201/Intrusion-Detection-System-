# 🚨 Network Intrusion Detection System using Suricata (DVWA Lab)

## 📌 Overview
This project demonstrates the design and implementation of a Host-based Intrusion Detection System (IDS) using **Suricata** to detect real-world web application attacks.

A vulnerable application (**DVWA – Damn Vulnerable Web App**) was deployed locally, and multiple attacks were simulated to test detection capabilities.

The IDS successfully detected:
- Port scanning
- SYN scanning
- Brute force login attempts
- SQL Injection
- Command Injection

---

## 🎯 Objectives
- Understand IDS/IPS fundamentals
- Write custom Suricata rules
- Simulate real cyber attacks safely
- Monitor logs and alerts
- Perform attack detection & analysis

---

## 🛠️ Tools & Technologies
- Kali Linux
- Suricata IDS
- DVWA (Vulnerable Web App)
- Apache + MySQL
- Nmap
- Browser-based attack simulation

---

## 🏗️ Architecture

Attacker (Kali tools / Browser)
        ↓
DVWA Web Server (localhost)
        ↓
Suricata IDS (traffic monitoring)
        ↓
Alerts → fast.log / eve.json

---

## ⚙️ Implementation Steps

### Phase 1 – Environment Setup
- Installed Suricata
- Configured rule paths
- Enabled fast.log alerts
- Started Apache & DVWA

### Phase 2 – IDS Monitoring
- Captured live traffic using Suricata
- Verified ICMP detection using ping
- Verified TCP detection using Nmap

### Phase 3 – Custom Rule Creation
Created detection rules for:
- SYN packets
- Port scans
- Brute force attempts
- SQL injection payloads
- Command injection patterns

### Phase 4 – Attack Simulation
Simulated:
- Nmap scans
- DVWA brute force login
- SQL injection attacks
- Command injection attacks

### Phase 5 – Alert Analysis
- Observed alerts in `/var/log/suricata/fast.log`
- Verified rule triggering
- Validated detection accuracy

---

## 🚨 Detected Attacks

| Attack Type | Tool Used | Detection Result |
|-----------|-----------|----------------|
| Port Scan | Nmap | ✅ Detected |
| SYN Scan | Nmap -sS | ✅ Detected |
| Brute Force | DVWA login | ✅ Detected |
| SQL Injection | DVWA SQLi | ✅ Detected |
| Command Injection | DVWA Command Exec | ✅ Detected |

---

## 📸 Screenshots
Screenshots of alerts are available in the `/screenshots` folder.

---

## 🧠 Skills Gained
- IDS rule writing
- Network traffic analysis
- Log analysis
- Threat detection engineering
- Security testing
- Linux system administration

---

## 🚀 Key Learnings
- How Suricata processes packets
- Signature-based detection
- Writing efficient detection rules
- Detecting real attack behavior
- SOC-style monitoring workflow

---

## 📌 Resume Description
Built a Network Intrusion Detection System using Suricata to detect port scanning, brute force, SQL injection, and command injection attacks by writing custom rules and analyzing live traffic from a DVWA lab environment.

---

## 👤 Author
**Prajwal V**
Cybersecurity Enthusiast | Network Security | IDS/Threat Detection
