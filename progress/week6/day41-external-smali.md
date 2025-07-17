# 📝 Day 41 – External Devices, Smali, and Android Security  
📅 Date: 17 July 2025  

---

## 🔌 External Device Compromise  
- Studied how **external devices** (USBs, keyboards, mice, chargers) can be compromised.  
- **Threats include**:  
  - *BadUSB attacks* – modified firmware on USB devices acting as HID (keyboard/mouse).  
  - Data exfiltration via infected devices.  
  - Rogue peripherals acting as attack vectors.  
- Importance of **Device Control Policies** and endpoint protection software to mitigate such risks.  

---

## 📱 Android App Architectures  
- **Native Apps**: Built specifically for a platform (Android/iOS), uses platform SDKs and APIs.  
- **Hybrid Apps**: Web apps wrapped in a native container using frameworks like Cordova or React Native.  
- Security concerns:  
  - Hybrid apps may expose extra attack surface if improperly sandboxed.  
  - Native apps rely on stricter OS-level security enforcement.  

---

## 🛠️ Smali and Register Usage  
- **Smali**: Assembly-like language for Android’s Dalvik bytecode.  
- Learned **register types**:  
  - `vX`: Local registers used in the method (variables).  
  - `pX`: Parameter registers passed into the method (method arguments).  
- Understanding this is crucial for Android reverse engineering and APK analysis.  

---

## 🚨 CVE-2024-40889 (Google Chrome – V8 Engine Use-After-Free)  
- **Vulnerability** in Chrome’s V8 JavaScript engine (Use-after-free in array handling).  
- Allowed arbitrary code execution via malicious web content.  
- Potential for full browser and system compromise.  
- Fixed in **Chrome 118.x Security Release (July 16, 2024)**.  



