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
