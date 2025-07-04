# Day 27 – RDP and VPN Insights  
📅 Date: 3 July 2025  

🛡️ **BlueKeep (CVE-2019-0708)**  
- Critical vulnerability in Microsoft’s RDP service (affects older Windows systems).  
- Allows **unauthenticated remote code execution** – attacker sends specially crafted RDP requests.  
- Wormable: Can self-propagate without user interaction (like WannaCry).  
- Attack chain: Scan → Exploit RDP → Deploy payload (e.g., ransomware).  
- Mitigations: Disable RDP if not needed, enable Network Level Authentication (NLA), apply patches.  

🌐 **VPN Fundamentals**  
- Creates a **secure, encrypted tunnel** over public/untrusted networks.  
- Two common types:  
  - **SSL VPN**: Operates at application layer (browser-based access).  
  - **IPSec VPN**: Works at network layer, secures all traffic.  
- Key features: Confidentiality, integrity, authentication.  
- Enterprise Use: Enables secure remote work and site-to-site connections.  

📊 **Quick Notes:**  
- 🔥 **BlueKeep = RDP + No Auth + Wormable** → Critical risk.  
- 🛡️ **VPN = Encrypted Tunnel** → Protects data in transit.  
- 🏢 Combine VPNs + strong patching to harden enterprise networks.  

💡 **Key Takeaway**: Exposed RDP and weak VPN setups are prime targets for attackers. Secure them proactively.  
