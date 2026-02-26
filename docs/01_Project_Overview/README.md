# Microsoft 365 / Entra ID – IAM GRC Lab

## Ziel des Projekts
Dieses Projekt demonstriert die Implementierung von Identity & Access Management (IAM) Kontrollen in Microsoft Entra ID (Azure AD) unter Berücksichtigung relevanter Sicherheitsstandards und Compliance-Anforderungen.

Das Ziel ist es, eine realitätsnahe Unternehmensumgebung abzubilden und typische IAM-Prozesse aus der Praxis darzustellen.

---

## Projektumfang (Scope)

Im Rahmen dieses Labs wurden folgende IAM-Bereiche umgesetzt:

- Identity Lifecycle Management (Joiner, Mover, Leaver)
- Multi-Faktor-Authentifizierung (MFA)
- Conditional Access Richtlinien
- Least Privilege Prinzip
- Privileged Identity Management (PIM)
- Access Reviews (Zugriffsüberprüfungen)
- Geräte-Compliance (Device Compliance)
- Single Sign-On (SSO)
- Federation (B2B / B2C)
- Protokollierung & Monitoring (inkl. SIEM mit Wazuh)

---

## Verwendete Technologien

- Microsoft Entra ID (Azure Active Directory)
- Microsoft 365
- Wazuh SIEM
- VirtualBox (Lab-Umgebung)
- Windows Server / Linux Systeme

---

## Architekturüberblick

Die Umgebung simuliert eine typische Unternehmensstruktur mit:

- Benutzer- und Gruppenverwaltung (RBAC)
- Sicherheitsgruppen nach Abteilungen (HR, IT, etc.)
- Durchsetzung von Sicherheitsrichtlinien über Conditional Access
- Überwachung von Anmeldeereignissen (Sign-in Logs)
- Integration in ein SIEM-System zur Angriffserkennung

---

## Compliance & Framework Mapping

Dieses Projekt orientiert sich an folgenden Standards:

- ISO/IEC 27001 (Annex A)
- NIST 800-53
- BSI IT-Grundschutz
- DSGVO (Datenschutz-Grundverordnung)

---

## Autor

Christian Chukwuka  
Cybersecurity | GRC | IAM  
Deutschland
