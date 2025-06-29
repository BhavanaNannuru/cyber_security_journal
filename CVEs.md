## 📅 June 28 – CVE Study

### CVE-2017-0144 (WannaCry Vulnerability – EternalBlue)
- Vulnerability in Microsoft SMBv1 (Remote Code Execution)
- Exploited by WannaCry ransomware in 2017
- Used EternalBlue exploit (NSA-leaked)
- Caused major damages, incl. UK's NHS
- Patched by Microsoft in March 2017 (MS17-010)

---

## June 29 – CVE Study  

### CVE-2021-44228 (Log4Shell Vulnerability – Apache Log4j)
- Vulnerability in Apache Log4j (Remote Code Execution via JNDI Lookup)  
- Exploited widely across internet-facing Java applications in 2021  
- Attackers used malicious `${jndi:ldap://...}` strings to trigger code execution  
- Initial impact seen on Minecraft servers; later affected enterprise, cloud systems  
- Patched in Log4j v2.15.0 (Dec 2021); hardened further in v2.16.0+
