
# 🔐 IT Audit Report – Identity & Access Management (IAM)

## 📌 Project Information

- **Project Name:** Microsoft 365 IAM GRC Lab
- **Auditor:** Christian Chukwuka
- **Date:** 2026-02-XX
- **Scope:** Identity & Access Management (IAM)
- **Environment:** Microsoft Entra ID (Azure AD)

---

## 🎯 Audit Objective

The objective of this audit is to evaluate the effectiveness of Identity and Access Management controls, focusing on:

- User authentication security
- Access control mechanisms
- Privileged access management
- Compliance with security frameworks

---

## 📦 Scope of Review

The following controls were assessed:

| Control ID | Control Name |
|-----------|-------------|
| IAM-01 | Multi-Factor Authentication (MFA) |
| IAM-02 | Least Privilege |
| IAM-03 | Conditional Access |
| IAM-04 | Privileged Identity Management (PIM) |
| IAM-06 | Access Review |

---

## 🧪 Methodology

The audit was conducted using:

- Configuration review (Microsoft Entra Admin Center)
- Access reviews and role assignments analysis
- Conditional Access policy validation
- Screenshot-based evidence collection
- Mapping against:
  - ISO 27001 (Annex A)
  - NIST 800-53
  - CIS Controls v8

---

## 🔍 Audit Findings

---

### 🔴 Finding 1: Excessive Privileges (Global Administrator)

- **Control:** IAM-02 (Least Privilege)
- **Issue:** Multiple users assigned Global Administrator role
- **Risk Level:** HIGH

**Risk:**
- Full tenant compromise if account is breached

**Recommendation:**
- Reduce Global Admin accounts to minimum (1–2)
- Implement PIM for just-in-time access

**Status:**
✅ Remediated

---

### 🟡 Finding 2: MFA Not Fully Enforced Initially

- **Control:** IAM-01 (MFA)
- **Issue:** Users did not have registered authentication methods
- **Risk Level:** MEDIUM

**Risk:**
- Increased likelihood of account compromise

**Recommendation:**
- Enforce MFA via Conditional Access
- Require user registration

**Status:**
✅ Implemented

---

### 🟢 Finding 3: Conditional Access Policies Implemented

- **Control:** IAM-03
- **Status:** GOOD PRACTICE

**Implemented Controls:**
- Require MFA
- Location-based access restriction
- Risk-based access
- Device compliance enforcement

---

### 🟢 Finding 4: Privileged Identity Management (PIM)

- **Control:** IAM-04
- **Status:** STRONG

**Implemented Controls:**
- Eligible role assignments (not permanent)
- MFA required for activation
- Justification required
- Time-bound access

---

### 🟢 Finding 5: Access Review (Guest Users)

- **Control:** IAM-06
- **Status:** IMPLEMENTED

**Details:**
- Quarterly review configured
- Guest users monitored
- Auto-removal enabled

---

## 📊 Risk Summary

| Risk Level | Count |
|-----------|------|
| HIGH | 1 |
| MEDIUM | 1 |
| LOW | 3 |

---

## 📚 Compliance Mapping

| Framework | Control |
|----------|--------|
| ISO 27001 | A.9 Access Control |
| NIST 800-53 | AC-2, AC-6 |
| CIS Controls v8 | Control 5 & 6 |

---

## 📸 Evidence

Stored in:
