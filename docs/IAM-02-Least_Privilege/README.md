# IAM-07: Least Privilege Principle

## Objective
Ensure users have only the minimum access required to perform their tasks.

---

## Implementation

- Role-based access control (RBAC)
- No permanent admin roles
- Use of PIM for privileged access
- Separation of duties between departments

---

## Example

- HR user:
  - Access: HR systems
  - No access to IT admin roles

- IT admin:
  - Access: Infrastructure
  - No access to finance systems

---

## Risk

- Excessive permissions
- Data leakage
- Unauthorized access

---

## Control Mapping

- ISO 27001: A.9.1, A.9.2
- NIST: AC-6
- CIS: Control 6

---

## Conclusion

Least privilege reduces attack surface and limits potential damage from compromised accounts.
