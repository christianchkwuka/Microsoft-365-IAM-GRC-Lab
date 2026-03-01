# 🔍 Logging and Monitoring (IAM)

## 📌 Objective

To monitor and detect:
- Unauthorized access
- Privileged misuse
- Suspicious login behavior
- Policy violations

---

## 🔧 Tools Used

- Microsoft Entra ID (Azure AD)
- Sign-in Logs
- Audit Logs
- Microsoft Defender for Cloud Apps (optional)

---

## 🧭 Step 1: Access Logs

Go to:

Entra Admin Center → Monitoring → Sign-in logs

---

## 🔐 Step 2: Sign-in Logs Analysis

Check for:

- Failed login attempts
- Unknown locations
- Risky sign-ins
- MFA status (success/failure)

Example:

User: admin@company.com  
Location: Unknown country  
Status: Failed login  

---

## 🧾 Step 3: Audit Logs

Go to:

Entra Admin Center → Monitoring → Audit logs

Track:

- Role assignments (PIM)
- User creation/deletion
- Policy changes (Conditional Access)
- Group membership changes

---

## 🚨 Step 4: Detect Suspicious Activity

Examples:

- Multiple failed logins → Possible brute force
- Admin role assigned suddenly → Privilege escalation
- Login from new country → Risk-based alert

---

## 🔗 Step 5: Integration with Conditional Access

Use logs to improve policies:

- Block risky sign-ins
- Require MFA for suspicious users
- Restrict access by location

---

## 📊 Step 6: SIEM Integration (Advanced)

Tool: Wazuh / Microsoft Sentinel

Purpose:

- Centralized log monitoring
- Real-time alerts
- Correlation of events

---

## 🛡️ Security Benefits

- Early detection of attacks
- Compliance (ISO 27001, NIST)
- Audit evidence
- Incident response readiness

---

## 📚 Framework Mapping

ISO 27001:
- A.12.4 Logging and Monitoring

NIST:
- AU-2 Event Logging
- AU-6 Audit Review

BSI:
- Logging & Monitoring Controls

GDPR:
- Article 32 (Security of processing)

---

## 📸 Evidence (Screenshots)

- Sign-in logs dashboard
- Audit logs (role assignment)
- Risky sign-in example

---

## ✅ Conclusion

Logging and monitoring ensure visibility into identity activities and help detect and respond to security threats in real time.
