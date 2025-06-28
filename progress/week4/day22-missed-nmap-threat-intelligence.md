# 🛡️ Day 22 – Threat Intel & Nmap Mastery  
📅 **Date:** Real 28 June 2025

---

## ✅ Completed Tasks

### 📌 TryHackMe Rooms
- **🔍 Nmap**  
  - Understood port scanning and reconnaissance fundamentals
  - Scanned with TCP Connect, SYN, UDP, NULL, FIN, Xmas methods
  - Covered firewalls, filtered ports, stealth scans
  - Explored Nmap Script Engine (NSE) & evasion techniques  
  - ⏳ *Pending:* Few hands-on tasks due to attack box timeout

- **📡 Intro to Cyber Threat Intelligence**
  - Types of CTI: Strategic, Tactical, Technical, Operational
  - Lifecycle: Direction → Collection → Processing → Analysis → Dissemination → Feedback
  - MITRE ATT&CK, STIX, TAXII protocols
  - Cyber Kill Chain & Diamond Model

### 🧪 SIEM Hands-On
- Worked on sample SIEM dashboard:
  - Mapped threat intel concepts to real dashboards
  - Understood how CTI helps SOC teams correlate attacks


## 🧠 Quick Summary Notes

### 🔗 Nmap Scan Types
 - TCP Connect (-sT): Full 3-way handshake
 - SYN (-sS): Half-open, stealthier
 - UDP (-sU): Slow, hard to verify open ports
 - NULL (-sN), FIN (-sF), Xmas (-sX): Obscure, evade basic IDS

### 🌐 Port Behavior
- **Open** → `SYN/ACK`
- **Closed** → `RST`
- **Filtered** → No response (likely firewalled)

---

### 📊 NSE Script Usage
```bash
nmap --script=<category>                # safe, vuln, auth, brute, etc.
nmap --script=<script> --script-args=<args>  # run specific script
```

## 🧠 Threat Intelligence Overview

### 💡 Threat Intel Types
- **Strategic**: Business impact
- **Tactical**: TTPs (Tactics, Techniques, Procedures)
- **Technical**: Indicators (IPs, hashes)
- **Operational**: Adversary motive & campaign data

---

### 🔄 Threat Intel Lifecycle
Direction → Collection → Processing → Analysis → Dissemination → Feedback




---

### 📚 Key Frameworks
- **MITRE ATT&CK**: Tactics & techniques framework
- **STIX/TAXII**: Structured intel exchange protocols
- **Cyber Kill Chain**: 7-phase attack lifecycle
- **Diamond Model**: 4-point correlation of:
  - Adversary
  - Victim
  - Infrastructure
  - Capabilities

---


### 🐍 Python Program Completed
**Script:** `port_multi_scanner.py`  
**Purpose:** Scans common ports on a given target, reports open/closed using multithreading 
**Status:** ✅ Uploaded to GitHub Python repo  
**Learning:** Socket programming, recon logic



### 💡 Reflections
> "Every byte explored, every packet decoded, is a step closer to mastering the unseen battlefield. Progress isn't loud—it's persistent."  
