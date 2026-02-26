# Identity Lifecycle Management (Joiner / Mover / Leaver)

## Ziel
Dieses Dokument beschreibt den Benutzerlebenszyklus in Microsoft Entra ID und wie Zugriffsrechte sicher verwaltet werden.

Identity Lifecycle Management stellt sicher, dass Benutzerkonten korrekt erstellt, angepasst und deaktiviert werden.

---

## 🔄 Überblick

Der Lebenszyklus besteht aus drei Phasen:

1. Joiner (Eintritt eines Mitarbeiters)
2. Mover (Positions- oder Abteilungswechsel)
3. Leaver (Austritt aus dem Unternehmen)

---

## 🟢 1. Joiner (Neuer Benutzer)

**Beschreibung:**  
Ein neuer Mitarbeiter wird erstellt und erhält initiale Berechtigungen.

**Umsetzung im Lab:**
- Benutzer erstellt (z.B. HR – John Peters)
- Zuweisung zur Gruppe: SG-HR
- Standardrechte vergeben

**Sicherheitskontrollen:**
- MFA aktiviert
- Conditional Access greift automatisch

**Risiko ohne Kontrolle:**
- Benutzer erhält falsche oder zu viele Rechte

---

## 🔄 2. Mover (Abteilungswechsel)

**Beschreibung:**  
Ein Benutzer wechselt Rolle oder Abteilung.

**Umsetzung im Lab:**
- Benutzer von SG-HR → SG-IT verschoben
- Alte Berechtigungen entfernt
- Neue Berechtigungen vergeben

**Wichtige Maßnahme:**
👉 **Remove old access BEFORE assigning new access**

**Risiko ohne Kontrolle:**
- Privilege Accumulation (zu viele Rechte über Zeit)

---

## 🔴 3. Leaver (Austritt)

**Beschreibung:**  
Ein Mitarbeiter verlässt das Unternehmen.

**Umsetzung im Lab:**
- Benutzerkonto deaktiviert
- Sessions beendet
- Zugriff vollständig entzogen

**Optional (Best Practice):**
- Passwort zurücksetzen
- Account nach X Tagen löschen

**Risiko ohne Kontrolle:**
- Ehemalige Mitarbeiter behalten Zugriff (!! Audit Finding)

---

## 🔐 Sicherheitsrelevanz

Identity Lifecycle ist kritisch für:

- Vermeidung von Insider Threats
- Schutz sensibler Daten
- Audit Compliance

---

## 📊 Framework Mapping

| Framework     | Kontrolle |
|--------------|----------|
| ISO 27001    | A.9.2.1, A.9.2.6 |
| NIST 800-53  | AC-2 |
| BSI IT-Grundschutz | ORP.4.A7 |

---

## 🧠 Audit Perspektive

Ein Auditor prüft:

- Werden Benutzer zeitnah deaktiviert?
- Werden alte Rechte entfernt?
- Gibt es dokumentierte Prozesse?
- Werden Logs geprüft?

---

## 📸 Evidence (Screenshots)

Die folgenden Nachweise wurden dokumentiert:

- Benutzererstellung (Joiner)
- Gruppenänderung (Mover)
- Konto-Deaktivierung (Leaver)

---

## ✅ Fazit

Ein korrekt implementierter Identity Lifecycle reduziert signifikant das Risiko von:

- Unautorisierten Zugriffen
- Datenverlust
- Compliance-Verstößen

Dieses Lab zeigt eine praxisnahe Umsetzung in Microsoft Entra ID.
