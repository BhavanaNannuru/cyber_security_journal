# 🛡️ Day 26 – Layers Matter  
📅 Date: 2 July 2025

Today’s journey was about **fortifying identity** and **uncovering weakness in design**.

## 🔐 2FA – Two-Factor Authentication
Two-Factor Authentication adds an additional layer of security beyond the password. It ensures that even if one factor (typically the password) is compromised, the attacker still needs the second to gain access.

### ✅ Why 2FA Matters
- Reduces risk from password reuse, phishing, and credential stuffing.
- Makes it significantly harder for attackers to gain unauthorized access.
- Widely adopted by platforms (Google, GitHub, AWS, etc.).

### 🔄 Types of 2FA
- **Something you know**: Password, PIN.
- **Something you have**: OTP app (Google Authenticator), SMS code, hardware token.
- **Something you are**: Biometrics (fingerprint, face recognition).

### 🛡️ Common 2FA Methods
| Method               | Example                     | Strength   |
|----------------------|-----------------------------|------------|
| SMS-based OTP        | Code via SMS                | Low        |
| TOTP apps            | Google Authenticator        | Medium     |
| Push Notification    | Authy, Duo                  | High       |
| Hardware Token       | Yubikey                     | Very High  |
| Biometrics           | Fingerprint/Face Unlock     | Medium     |

---

## 🐛 CVE-2018-11776 – Apache Struts Namespace Misconfiguration

### 🧠 Summary:
- Vulnerability in **Apache Struts 2** when using **namespace-based URL configuration**.
- Allows **Remote Code Execution (RCE)** if the app does not properly validate namespace values.
- Identified in versions **Struts 2.3 to 2.5.16**.

### 💥 Root Cause:
- Unvalidated user input passed into namespace in the URL.
- Malicious input evaluated in OGNL (Object-Graph Navigation Language), leading to RCE.

### 🔍 Mitigation:
- Upgrade Apache Struts to version 2.3.35 or 2.5.17+.
- Avoid dynamic namespace evaluation.
- Apply input validation & disable OGNL where possible.

---

## 🧠 Final Thoughts

> Security is not just patching flaws — it's understanding why they existed in the first place.

Learning about **2FA** shows the importance of **layered defenses**, while **CVE-2018-11776** teaches how design missteps can break those defenses entirely.

Both are reminders that in cybersecurity, simplicity doesn’t mean weakness — but **misconfiguration always does**.