# Day 1 – OWASP Top 10 Introduction
📅 Date: 7 June 2025

## 🔥 What I Learned Today
- OWASP Top 10 is a list of most critical web app security risks
- Focuses on real-world exploits like SQL Injection, XSS, etc.

## 🧠 Top Takeaways
| Risk | Description                         | Real-World Meaning                                | Prevention                                               | Example                                                  |
|------|-------------------------------------|--------------------------------------------------|-----------------------------------------------------------|----------------------------------------------------------|
| A01  | Broken Access Control               | Users can access unauthorized data               | Implement role-based access checks on every request       | A user views another user's account by changing ID in URL|
| A02  | Cryptographic Failures              | Sensitive data exposed due to weak encryption    | Use strong encryption (e.g., AES), HTTPS, and secure key storage | Passwords stored in plain text get leaked          |
| A03  | Injection                           | User input alters database queries (e.g., SQLi)  | Use prepared statements and input validation              | Attacker uses `' OR '1'='1` to bypass login             |
| A04  | Insecure Design                     | Poor app design leads to exploitable flaws       | Secure by design, threat modeling, use design patterns    | No rate limiting allows brute-force login attacks       |
| A05  | Security Misconfig                  | Poor server settings expose system               | Disable default accounts, close unused ports, set proper permissions | Admin panel left exposed without authentication |
| A06  | Vulnerable & Outdated Components    | Old libraries with known flaws used in app       | Regularly update components and monitor CVEs              | Using outdated jQuery with XSS vulnerability            |
| A07  | Identification & Auth Failures      | Weak login or session handling leads to takeover | Enforce MFA, session expiration, strong password policies | No timeout on session allows hijacking                  |
| A08  | Software/Data Integrity Failures    | Untrusted code updates allow tampering           | Use digital signatures, verify sources, secure CI/CD      | App downloads update from an unauthenticated source     |
| A09  | Security Logging & Monitoring Failures | Attacks go undetected due to missing logs     | Implement logging, monitoring, and alerting tools         | SQL injection not logged or alerted                     |
| A10  | Server-Side Request Forgery (SSRF)  | Server is tricked into accessing internal assets | Whitelist allowed domains, disable unnecessary protocols  | Attacker accesses internal metadata service via crafted URL |


## 🛠️ Next Up
- Install Kali tools (Wireshark, Nmap, Burp Suite)
- Try OWASP Juice Shop locally

