# 🔐 IAM-02: Conditional Access (Zero Trust Enforcement)

## 📌 Objective
The objective of this control is to enforce secure access to cloud resources by applying policy-based conditions such as user identity, device compliance, and authentication requirements.

Conditional Access is a core component of the Zero Trust security model:
> "Never trust, always verify"

---

## 🧠 Description
Conditional Access in Microsoft Entra ID allows organizations to control access to applications based on predefined policies.

These policies evaluate:
- User identity
- Device compliance
- Location (IP / Country)
- Risk level
- Authentication method

---

## ⚙️ Configuration Steps

### 🔹 Step 1: Navigate to Conditional Access
- Microsoft Entra Admin Center
- Go to: **Security → Conditional Access**

---

### 🔹 Step 2: Create New Policy
- Click: **New policy**

**Policy Name:**




---

### 🔹 Step 3: Assign Users
- Include: **All users**
- Exclude: **Break-glass / Admin account (to avoid lockout)**

---

### 🔹 Step 4: Target Resources
- Select: **All cloud apps**

---

### 🔹 Step 5: Configure Conditions (Optional)
- No conditions applied in this baseline configuration

---

### 🔹 Step 6: Grant Controls
- Select: **Grant access**
- Enable:
  - ✅ Require multi-factor authentication (MFA)

---

### 🔹 Step 7: Enable Policy
- Set policy status to: **On**
- Click: **Create**

---

## 📸 Evidence (Screenshots)

Stored in:
