# 🛡️ Day 43 – Fortinet CVE & USB Security Mechanisms  
📅 Date: 19 July 2025  

---

## 🚨 CVE-2025-25257 (Fortinet FortiWeb – SQL Injection RCE)  
- **Vulnerability Summary**  
  - Critical **SQL Injection** in Fortinet FortiWeb’s Web Application Firewall (WAF).  
  - Caused by improper sanitization of user-supplied input in HTTP(S) requests.  

- **Attack Details**  
  - Allowed **unauthenticated remote attackers** to:  
    - Execute arbitrary SQL queries on backend databases.  
    - Escalate to full **Remote Code Execution (RCE)** as `root`.  
    - Deploy persistent malware such as **web shells** for long-term access.  
  - Exploited hours after a public proof-of-concept (PoC) was released.  
  - Real-world impact: Dozens of production FortiWeb instances were compromised.  

- **Affected Versions**  
  - FortiWeb prior to:  
    - 7.6.4  
    - 7.4.8  
    - 7.2.11  
    - 7.0.11  

- **Mitigation & Lessons**  
  - Apply patches immediately.  
  - Enforce **input validation and sanitization** in WAF rule sets.  
  - Monitor for unexpected outbound connections from WAF systems.  

---

## 💾 USB/Pendrive Security Mechanisms  
- **Risks with USB Devices**  
  - **Malware Propagation**: AutoRun worms, infected executables.  
  - **BadUSB Attacks**: Malicious firmware reprogramming of USB devices.  
  - **Data Exfiltration**: Insider threat using removable media to copy sensitive data.  

- **Protection Techniques**  
  - 🔒 **USB Port Control**: Disable unused ports in BIOS/UEFI or through OS group policies.  
  - 🛡️ **Endpoint Protection**: Use tools to block unauthorized devices (e.g., USBGuard).  
  - 🛑 **AutoRun Blocking**: Disable AutoRun/AutoPlay to stop automatic execution of malicious payloads.  
  - 🔐 **Hardware Encryption**: Enforce encrypted USB drives with password/PIN protection.  
  - 🧪 **Content Scanning**: Force all USB devices to pass antivirus scans before mounting.  

- **Enterprise Best Practices**  
  - Implement **Device Control Policies** (allow only whitelisted USB devices).  
  - Train employees about **USB baiting attacks** (e.g., attackers leaving infected USBs in parking lots).  

