# 📝 Day 42 – Keystroke Dynamics & CVE Study  
📅 Date: 18 July 2025  

---

## ⌨️ Keystroke Dynamics for Password Analysis  
- **What is Keystroke Dynamics?**  
  - A **biometric behavioral analysis** method that captures *how* a user types rather than *what* they type.  
  - Features include typing speed, dwell time (how long a key is pressed), and flight time (time between key presses).  

- **Applications in Security**  
  - **Authentication**: Adds a layer of security by verifying user typing patterns alongside passwords.  
  - **Forensics**: Helps identify or profile an attacker based on typing behavior in logs.  
  - **Attack Scenario**: Can be abused to reconstruct passwords by analyzing typing cadence through hardware keyloggers or malware.  

- **Key Points**  
  - Algorithms: SVMs, Random Forests, and Neural Networks are used to classify typing patterns.  
  - Vulnerabilities: Timing attacks can exploit keystroke dynamics to predict passwords.  
  - Defenses: Input obfuscation, randomized delay injection, and using secure password managers.  

---

## 🚨 CVE-2025-13168 (Critical)  
- **Vulnerability Summary**  
  - A **Buffer Overflow vulnerability** in a widely used OpenSSH implementation.  
  - Could allow unauthenticated remote attackers to execute arbitrary code.  
  - Exploited via specially crafted SSH requests to overwrite memory and gain system access.  

- **Impact**  
  - Affects OpenSSH versions < 9.8.  
  - Successful exploitation can lead to full server compromise.  
  - Weaponized in automated SSH worm attacks.  

- **Mitigation**  
  - Patch applied in OpenSSH 9.8 release (May 2025).  
  - Recommended actions: Immediate update and disable password-based SSH logins in favor of key-based authentication.  

---
