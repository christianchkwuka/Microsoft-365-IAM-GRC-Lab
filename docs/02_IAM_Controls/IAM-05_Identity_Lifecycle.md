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

<img width="1882" height="885" alt="User_creation" src="https://github.com/user-attachments/assets/c2110fa3-e669-40cc-a2b5-30965aeaa4ce" />

<img width="1902" height="950" alt="User_John" src="https://github.com/user-attachments/assets/0a4b49ba-9fa1-40ca-ad56-a53d6ef79e9f" />

<img width="1912" height="895" alt="User_in_group" src="https://github.com/user-attachments/assets/99ee1ef6-4a5a-4c1e-ab05-779bc618c0d9" />


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

<img width="1905" height="857" alt="Mover_John" src="https://github.com/user-attachments/assets/2b07e965-9c08-4b23-86e5-2a15598efd8a" />

<img width="1913" height="852" alt="Move_John_2" src="https://github.com/user-attachments/assets/0ca44e94-862b-42f2-b5ed-65042713b708" />

<img width="1891" height="873" alt="Moved_John_3" src="https://github.com/user-attachments/assets/24b758fe-52c2-4b46-9902-d2ecaae75052" />

<img width="1892" height="878" alt="John_moved_sales" src="https://github.com/user-attachments/assets/799bfa0b-48fa-4141-b277-9d77c61f9644" />


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

- <img width="1887" height="892" alt="Leaver_enabled" src="https://github.com/user-attachments/assets/3876d5ec-7783-43d7-a41d-b7f7536e1ca2" />

<img width="1891" height="876" alt="Leaver_disable_setting" src="https://github.com/user-attachments/assets/4b18d3ae-8eb4-4c1f-8283-6a12b5ad83b2" />

<img width="1905" height="896" alt="Leaver_disable Session_revoke" src="https://github.com/user-attachments/assets/78caea75-15d2-48b1-a303-ca6621defc17" />




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
