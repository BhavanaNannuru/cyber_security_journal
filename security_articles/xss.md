# 🛡️ Cybersecurity Daily — Day 13

## 📌 Topic: Cross-Site Scripting (XSS)

> “XSS lets attackers inject malicious scripts into trusted websites, targeting users instead of servers.”

---

### 🧠 What is Cross-Site Scripting (XSS)?

**XSS** is a **web vulnerability** that allows attackers to inject **malicious scripts** into web pages viewed by other users.  

When victims visit the infected page:  
- The browser executes the attacker’s script.  
- This can **steal cookies**, session tokens, or redirect users to malicious sites.  

> 🧠 Think of it as someone sneaking fake instructions into a recipe you’re following.

---

### 🚨 Types of XSS

- **Stored XSS (Persistent)**  
  Malicious script is saved on the server and sent to every user.  

- **Reflected XSS (Non-Persistent)**  
  Script is in a URL or form input and runs only when the link is clicked.  

- **DOM-Based XSS**  
  Happens entirely in the browser when JavaScript dynamically changes the page.

---

### 🧠 Real-World Case

- **eBay XSS (2014)**  
  Attackers injected JavaScript in product listings.  
  When users clicked items, they were redirected to phishing pages.  

---

### ✅ Defense Against XSS

- 🚫 **Never trust user input**: Sanitize and validate all inputs.  
- 🛡️ **Use Output Encoding**: Prevent browsers from interpreting data as code.  
- 🔒 **Enable Content Security Policy (CSP)**: Blocks unauthorized scripts.  
- 🧪 Regularly test with XSS scanners (e.g., OWASP ZAP).  

---

### 📌 Summary (1-liner)

> *“XSS attacks target users by injecting malicious scripts into trusted websites — sanitize inputs to stop them.”*

🔗 **Source**: [OWASP – Cross-Site Scripting (XSS)](https://owasp.org/www-community/attacks/xss/)
