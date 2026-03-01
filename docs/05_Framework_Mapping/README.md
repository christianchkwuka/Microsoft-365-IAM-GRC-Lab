# 🔐 IAM Framework Mapping

## 📌 Objective

This document maps implemented IAM controls to international security frameworks:

- ISO/IEC 27001:2022
- BSI IT-Grundschutz
- NIST SP 800-53
- CIS Controls v8
- GDPR (DSGVO)

---

## 📊 Control Mapping Table

| IAM Control | Description | ISO 27001 | BSI | NIST | CIS | GDPR |
|------------|------------|----------|-----|------|-----|------|
| MFA | Multi-factor authentication | A.5.17 | ORP.4 | IA-2 | Control 6 | Art. 32 |
| Conditional Access | Context-based access control | A.5.15 | APP.4.3 | AC-3 | Control 6 | Art. 32 |
| Least Privilege | Minimum access rights | A.5.18 | ORP.4 | AC-6 | Control 6 | Art. 5 |
| PIM | Just-in-time admin access | A.5.18 | ORP.4 | AC-2 | Control 5 | Art. 32 |
| Access Review | Periodic access validation | A.5.18 | ORP.4 | AC-2 | Control 5 | Art. 5 |
| Identity Lifecycle | Joiner-Mover-Leaver process | A.5.16 | ORP.4 | AC-2 | Control 5 | Art. 5 |
| Logging & Monitoring | Activity tracking | A.8.15 | DET.2 | AU-2 | Control 8 | Art. 32 |

---

## 🧠 Explanation of Frameworks

### ISO 27001
Focuses on:
- Access control
- Authentication
- Risk management

---

### BSI IT-Grundschutz
German standard emphasizing:
- Identity management (ORP.4)
- Access control (APP.4.3)
- Monitoring (DET.2)

---

### NIST SP 800-53
US framework covering:
- AC (Access Control)
- IA (Identification & Authentication)
- AU (Audit Logs)

---

### CIS Controls v8
Practical security controls:
- Control 5: Account Management
- Control 6: Access Control
- Control 8: Audit Logs

---

### GDPR (DSGVO)
Legal requirements:
- Article 5: Data minimization
- Article 32: Security of processing

---

## 📊 Summary

The implemented IAM controls align with multiple international security frameworks, ensuring:

- Strong authentication (MFA)
- Controlled access (Least Privilege)
- Secure administration (PIM)
- Continuous monitoring (Logs & SIEM)

---

## 🏁 Conclusion

The IAM implementation demonstrates compliance with industry standards and reflects real-world enterprise security architecture.
