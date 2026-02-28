# 🔐 IAM Risk Assessment

## 📌 Scope
Microsoft Entra ID – Identity & Access Management

---

## 📊 Risk Table

| ID | Risk Description | Impact | Likelihood | Risk Level | Control Implemented | Residual Risk |
|----|-----------------|--------|------------|------------|---------------------|---------------|
| R1 | No MFA enabled | High | High | 🔴 High | Conditional Access (MFA) | 🟢 Low |
| R2 | Too many Global Admins | High | Medium | 🔴 High | PIM + Role Reduction | 🟢 Low |
| R3 | No access review | Medium | High | 🟠 Medium | Access Review (Quarterly) | 🟢 Low |
| R4 | Untrusted login locations | High | Medium | 🔴 High | Location-based CA | 🟢 Low |
| R5 | Unmanaged devices access | High | Medium | 🔴 High | Device Compliance Policy | 🟠 Medium |
| R6 | Permanent admin privileges | High | Medium | 🔴 High | PIM (Just-in-Time) | 🟢 Low |

---

## 📊 Risk Evaluation Criteria

| Level | Description |
|------|------------|
| 🔴 High | Immediate security threat |
| 🟠 Medium | Potential risk |
| 🟢 Low | Controlled risk |

---

## 🧪 Methodology

Risk was assessed based on:

- Impact (Business damage)
- Likelihood (Chance of occurrence)

Formula:

Risk Level = Impact × Likelihood

---

## 🏁 Conclusion

The implementation of IAM controls significantly reduced the risk exposure.

Key improvements:
- Strong authentication (MFA)
- Controlled admin access (PIM)
- Continuous monitoring (Access Review)
- Context-aware access (Conditional Access)

---
