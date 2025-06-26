# Day 3 – OWASP Top 10 (Part 1) – Theory + Burp Suite Setup
📅 Date: 9 June 2025

## ✅ TryHackMe Room
[OWASP Top 10 - 2021 Edition](https://tryhackme.com/room/owasptop102021)

---

## 🧠 Topics Covered

### 🛡️ A01: Broken Access Control
- Studied examples of insecure access:
  - IDOR (Insecure Direct Object Reference)
  - Forced browsing by modifying resource IDs in URLs
- Key Insight: DOR (Direct Object Reference) is not a vulnerability on its own — **IDOR** occurs when there's no proper access check
- Learned about horizontal and vertical privilege escalation techniques

---

### 🔐 A02: Cryptographic Failures
- Reviewed insecure practices like:
  - Using weak cryptographic algorithms (e.g., MD5, SHA-1)
  - Transmitting sensitive data without HTTPS
  - Missing secure flags on cookies
- Will perform hands-on attack tomorrow due to environment constraints

---

### 💉 A03: Injection Attacks
- Understood how SQL and Command Injection work
- Studied payload examples like `' OR 1=1 --` and `; ls`
- Observed the risk of executing arbitrary queries or commands via unsanitized inputs
- Hands-on execution deferred to Day 4

---

## 🛠️ Tools Used

- **TryHackMe** platform for theory + guided labs
- ✅ **Burp Suite** – Defaulty Installed; configured, and launched inside Kali Linux
- Kali Linux environment fully operational

---

## ⚙️ Environment Setup Completed Today
- Opened and tested **Burp Suite Community Edition**
- Verified functionality inside Kali VM

---

## 🔁 Deferred to Day 4
- Practical exploitation for A02 and A03 vulnerabilities
- Capturing Burp Suite intercepts and screenshots
- Writing walkthrough for hands-on phase

---

## 🧠 Reflections
> Today I strengthened my theoretical foundation on core OWASP vulnerabilities and prepared my environment for hands-on exploitation. Burp Suite is now ready, and tomorrow I’ll put this knowledge into practice by intercepting and manipulating live HTTP traffic.

---

