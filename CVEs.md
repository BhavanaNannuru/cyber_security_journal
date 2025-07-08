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


### June 30 – CVE Study  
**CVE-2016-4657 (Trident Exploit Chain – WebKit Vulnerability)**  
Vulnerability in Apple’s WebKit (Memory Corruption in Safari)  
Used in Trident exploit chain by Pegasus spyware (NSO Group)  
Allowed attackers to compromise iPhones via a single malicious link  
Enabled remote code execution, full surveillance, and access to mic/camera  
Patched by Apple in iOS 9.3.5 (August 2016)


### July 1 – CVE Study  
**CVE-2014-6271 (Shellshock – Bash Vulnerability)**  
Vulnerability in GNU Bash shell (Improper function parsing)  
Allowed attackers to execute commands by injecting code into environment variables  
Exploited in web servers, IoT devices, DHCP clients — massive internet-wide risk  
Impact included remote code execution with minimal access  
Patched by GNU in Bash updates released September 2014


### July 2 – CVE Study  
**CVE-2018-11776 (Apache Struts OGNL Injection – Jakarta Plugin)**  
Vulnerability in Apache Struts 2 (Improper namespace handling in OGNL expressions)  
Allowed attackers to inject and execute remote code via crafted URLs  
Affected web apps using vulnerable Struts configurations (e.g., REST plugin)  
Notable past Struts bug led to the Equifax data breach (2017)  
Patched in Apache Struts 2.3.35 and 2.5.17 (August 2018)


### July 3 – CVE Study  
**CVE-2019-0708 (BlueKeep – RDP Vulnerability)**  
Vulnerability in Microsoft Remote Desktop Protocol (RDP) service  
Allowed attackers to execute remote code on unpatched Windows systems (Wormable)  
Could spread without user interaction, similar to WannaCry-style attacks  
Millions of Windows 7, Server 2008 systems were initially exposed  
Patched by Microsoft in May 2019, including an emergency patch for Windows XP

### July 4 – CVE Study  
**CVE-2017-5638 (Apache Struts2 – Jakarta Multipart RCE)**  
Vulnerability in Apache Struts2 (Improper input validation in file upload parser)  
Allowed attackers to execute arbitrary code via crafted Content-Type headers  
Famously exploited in the 2017 **Equifax data breach** (148M records stolen)  
Targeted web apps using the Jakarta Multipart parser in default configs  
Patched by Apache in Struts 2.3.32 and 2.5.10.1 (March 2017)


### July 5 – CVE Study  
**CVE-2021-34527 (PrintNightmare – Windows Print Spooler Vulnerability)**  
Vulnerability in Windows Print Spooler service (Improper privilege validation)  
Allowed attackers to execute remote code and gain SYSTEM-level privileges  
Exploited for lateral movement and deploying ransomware in networks  
Impacted all supported Windows versions, including domain controllers  
Patched by Microsoft in July 2021 (Emergency out-of-band update)


### July 6 – CVE Study  
**CVE-2023-34362 (MOVEit Transfer – SQL Injection Vulnerability)**  
Vulnerability in Progress MOVEit Transfer (Improper input sanitization in SQL queries)  
Allowed attackers to execute arbitrary SQL commands and exfiltrate sensitive data  
Exploited by the CL0P ransomware group in a massive global supply chain attack  
Affected organizations worldwide, including banks and government agencies  
Patched by Progress Software in May 2023 (Security Advisory issued)

### July 7 – CVE Study  
**CVE-2023-23397 (Outlook NTLM Leak – Microsoft Outlook Vulnerability)**  
Vulnerability in Microsoft Outlook (Improper handling of calendar reminders)  
Allowed attackers to steal NTLM hashes by sending crafted calendar invites  
Exploited for credential theft without user interaction (zero-click)  
Impacted Outlook for Windows clients across enterprise environments  
Patched by Microsoft in March 2023 (Patch Tuesday release)

### July 8 – CVE Study  
**CVE-2022-30190 (Follina – Microsoft MSDT Vulnerability)**  
Vulnerability in Microsoft Support Diagnostic Tool (MSDT) via Office documents  
Allowed attackers to execute arbitrary code when a user opened or previewed a malicious file  
Exploited through specially crafted Word documents delivered via phishing emails  
Impacted all supported Windows versions with Office installed  
Patched by Microsoft in June 2022 (Security Update KB5014697)

