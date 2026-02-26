# Identity & Access Management (IAM) Controls

## Ziel
Dieser Abschnitt beschreibt die implementierten IAM-Kontrollen innerhalb der Microsoft Entra ID Umgebung und deren Bedeutung im Kontext von IT-Sicherheit und Compliance.

IAM ist ein zentraler Bestandteil moderner Sicherheitsarchitekturen und stellt sicher, dass nur autorisierte Benutzer Zugriff auf Systeme und Daten erhalten.

---

## 🔐 Überblick der implementierten Kontrollen

Die folgenden IAM-Kontrollen wurden im Lab umgesetzt:

1. Multi-Faktor-Authentifizierung (MFA)
2. Least Privilege Prinzip
3. Conditional Access
4. Privileged Identity Management (PIM)
5. Access Reviews
6. Identity Lifecycle Management
7. Device Compliance (Zero Trust)

---

## 🔑 1. Multi-Faktor-Authentifizierung (MFA)

**Beschreibung:**  
MFA erhöht die Sicherheit, indem neben dem Passwort ein zusätzlicher Faktor erforderlich ist.

**Implementierung im Lab:**
- Aktivierung von MFA für Benutzer
- Nutzung von Microsoft Authenticator

**Risiko ohne MFA:**
- Kontoübernahme durch Phishing oder Passwort-Leaks

**Framework Mapping:**
- ISO 27001: A.9.4.2
- NIST: IA-2
- BSI: OPS.1.1.2

---

## 🔒 2. Least Privilege (Minimalprinzip)

**Beschreibung:**  
Benutzer erhalten nur die minimal notwendigen Berechtigungen.

**Implementierung im Lab:**
- Nutzung von Sicherheitsgruppen (z.B. SG-HR)
- Rollenzuweisung nur bei Bedarf

**Risiko ohne Kontrolle:**
- Unautorisierter Zugriff auf sensible Daten

**Framework Mapping:**
- ISO 27001: A.9.1.2
- NIST: AC-6
- BSI: ORP.4

---

## 🌍 3. Conditional Access

**Beschreibung:**  
Zugriff wird basierend auf Bedingungen gesteuert (z.B. Standort, Gerät, Risiko).

**Implementierung im Lab:**
- MFA erzwingen bei Login
- Zugriff nur von vertrauenswürdigen Geräten

**Risiko ohne Kontrolle:**
- Zugriff von unsicheren oder kompromittierten Geräten

**Framework Mapping:**
- ISO 27001: A.9.4.1
- NIST: AC-3
- BSI: OPS.1.1.4

---

## 👑 4. Privileged Identity Management (PIM)

**Beschreibung:**  
Verwaltung privilegierter Rollen mit Just-in-Time Zugriff.

**Implementierung im Lab:**
- Temporäre Adminrechte
- Genehmigungsprozesse

**Risiko ohne Kontrolle:**
- Dauerhafte Adminrechte = hohes Risiko

**Framework Mapping:**
- ISO 27001: A.9.2.3
- NIST: AC-5
- BSI: ORP.4.A2

---

## 🔍 5. Access Reviews

**Beschreibung:**  
Regelmäßige Überprüfung von Benutzerberechtigungen.

**Implementierung im Lab:**
- Review von Gruppenmitgliedschaften
- Zeitbasierte Reviews

**Risiko ohne Kontrolle:**
- „Zombie Accounts“ behalten Zugriff

**Framework Mapping:**
- ISO 27001: A.9.2.5
- NIST: AC-2
- BSI: ORP.4.A5

---

## 🔄 6. Identity Lifecycle Management

**Beschreibung:**  
Verwaltung von Benutzerkonten während ihres gesamten Lebenszyklus.

**Phasen:**
- Joiner (Neuer Benutzer)
- Mover (Abteilungswechsel)
- Leaver (Austritt)

**Implementierung im Lab:**
- HR User erstellt (Joiner)
- Gruppenänderung simuliert (Mover)
- Konto deaktiviert (Leaver)

**Risiko ohne Kontrolle:**
- Ehemalige Mitarbeiter behalten Zugriff

**Framework Mapping:**
- ISO 27001: A.9.2.1
- NIST: AC-2
- BSI: ORP.4.A7

---

## 💻 7. Device Compliance (Zero Trust)

**Beschreibung:**  
Zugriff nur von sicheren und verwalteten Geräten.

**Implementierung im Lab:**
- Conditional Access + Device Compliance

**Risiko ohne Kontrolle:**
- Zugriff von kompromittierten Geräten

**Framework Mapping:**
- ISO 27001: A.13.1
- NIST: CM-7
- BSI: OPS.1.1.5

---

## 🧠 Fazit

Die implementierten IAM-Kontrollen bilden die Grundlage einer Zero Trust Sicherheitsarchitektur und reduzieren signifikant das Risiko von Identitäts-basierten Angriffen.

Dieses Lab zeigt praxisnah, wie Unternehmen Identity Security umsetzen können.
