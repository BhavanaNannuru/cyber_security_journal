# 🛡️ Cybersecurity Daily — July 11, 2025

## 📌 Topic: Cloud Security Basics — Shared Responsibility Model

> “Cloud security is a team effort—both you and your provider play vital roles.”

---

## 🧠 What Is the Shared Responsibility Model?

When using cloud services (like AWS, Azure, Google Cloud), **security duties are shared**:

- **Cloud Provider** secures the infrastructure (data centers, physical servers, network).
- **You (Customer)** secure your data, applications, configurations, access controls.

> 🗝️ The model balances accountability—your provider protects the foundation, while you manage what’s built on top.

---

## 🔍 Responsibilities Breakdown

| Who               | Responsibilities                                     |
|-------------------|------------------------------------------------------|
| **Cloud Provider**| Physical security, host OS, virtualization, network |
| **Customer**      | Data encryption, user access, app security, configs |

---

## 🚨 Common Misconfigurations

- **Open S3 buckets / Storage**  
  Accidentally exposing files or databases to the internet.

- **Weak IAM Policies**  
  Granting excessive permissions—e.g. making every user an admin.

- **No Encryption**  
  Storing sensitive data without encryption at rest or in transit.

- **Outdated Software**  
  Running unpatched apps or services on cloud VMs.

---

## 🛠️ Real-World Case

**Capital One (2019)**  
- Misconfigured AWS WAF (firewall) allowed SSRF attack.  
- Attacker accessed over **100 million customer records**, revealing sensitive data.  
- Reminder: configuration matters just as much as infrastructure setup.

---

## ✅ Cloud Security Best Practices

1. **Enable Encryption**  
   - Data at rest (e.g., AWS KMS)  
   - Data in transit (TLS/HTTPS)

2. **Harden Identity Access Management (IAM)**  
   - Apply least-privilege principles  
   - Use role-based access control (RBAC)

3. **Audit & Monitor**  
   - Review logs (CloudTrail, Azure Monitor)  
   - Set alerts for unusual access

4. **Secure Configurations**  
   - Regularly scan with tools (e.g., AWS Config, Azure Security Center)  
   - Ensure storage buckets aren't public

5. **Keep Software Updated**  
   - Patch VMs, containers, serverless functions

6. **Backup & Recovery Plans**  
   - Regular data snapshots and testing of restore procedures

---

## 📌 Summary (1-liner)

> *“Effective cloud security depends on both your provider’s infrastructure and your own configurations and controls.”*

🔗 **Source**: [AWS Shared Responsibility Model documentation](https://aws.amazon.com/compliance/shared-responsibility-model/)
