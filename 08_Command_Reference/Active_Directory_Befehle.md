# Ziel
AD-spezifische Diagnosebefehle für Betrieb und Fehlersuche verständlich dokumentieren.

# Voraussetzungen
- Domain Controller oder RSAT-Umgebung
- Administrative Berechtigungen

# Umsetzung
## net user
- **Zweck:** Benutzerkonten anzeigen oder verwalten.
- **Syntax:** `net user [Benutzername] [Passwort] [/add]`
- **Beispiel:** `net user test.user P@ssw0rd123 /add`
- **Beispielausgabe erklärt:** Bestätigt, dass das Konto erstellt wurde.

## net group
- **Zweck:** Gruppen anzeigen oder verwalten.
- **Syntax:** `net group [Gruppenname] [Benutzer] [/add] /domain`
- **Beispiel:** `net group GG_IT test.user /add /domain`
- **Beispielausgabe erklärt:** Zeigt erfolgreiche Aufnahme in die Domänengruppe.

## dcdiag
- **Zweck:** Domain Controller Gesundheitscheck.
- **Syntax:** `dcdiag [/test:DNS]`
- **Beispiel:** `dcdiag /test:DNS`
- **Beispielausgabe erklärt:** Tests für DNS/AD-Dienste; Fehler zeigen konkrete Problemfelder.

## repadmin
- **Zweck:** AD-Replikation prüfen.
- **Syntax:** `repadmin /replsummary`
- **Beispiel:** `repadmin /replsummary`
- **Beispielausgabe erklärt:** Zeigt Replikationsstatus, Fehlerraten und betroffene Partner.

# Test
- Befehle auf dem DC ausgeführt
- Ergebnisse mit Ereignisanzeige und AD-Konsole abgeglichen

# Troubleshooting
- Replikationsfehler: DNS und Zeitdienst prüfen
- Benutzer/Gruppenänderung nicht sichtbar: Replikation und OU prüfen
- Befehlsfehler: Domänenkontext und Rechte kontrollieren

# Fazit
Die AD-Befehle helfen, Probleme früh zu erkennen und zielgerichtet zu beheben.
