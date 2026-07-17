# Ziel
Wichtige Windows-Server-Befehle kompakt dokumentieren, um Administration und Analyse zu beschleunigen.

# Voraussetzungen
- Eingabeaufforderung oder PowerShell mit passenden Rechten
- Zugriff auf Server oder Client im Lab

# Umsetzung
## hostname
- **Zweck:** Zeigt den lokalen Computernamen.
- **Syntax:** `hostname`
- **Beispiel:** `hostname`
- **Beispielausgabe erklärt:** Gibt z. B. `DC01` zurück. So prüfst du schnell, auf welchem System du arbeitest.

## whoami
- **Zweck:** Zeigt den aktuell angemeldeten Benutzer.
- **Syntax:** `whoami`
- **Beispiel:** `whoami`
- **Beispielausgabe erklärt:** `lab\administrator` zeigt, dass die Anmeldung in der Domäne erfolgt.

## gpupdate
- **Zweck:** Erzwingt sofortige Aktualisierung von Gruppenrichtlinien.
- **Syntax:** `gpupdate [/force]`
- **Beispiel:** `gpupdate /force`
- **Beispielausgabe erklärt:** Meldet, ob Benutzer- und Computerrichtlinien erfolgreich aktualisiert wurden.

## gpresult
- **Zweck:** Zeigt angewendete Gruppenrichtlinien.
- **Syntax:** `gpresult /r` oder `gpresult /h report.html`
- **Beispiel:** `gpresult /r`
- **Beispielausgabe erklärt:** Listet aktive GPOs und hilft bei Richtlinienanalyse.

## netdom
- **Zweck:** Domänen- und Computerbeziehungen verwalten.
- **Syntax:** `netdom <operation> [optionen]`
- **Beispiel:** `netdom query computer`
- **Beispielausgabe erklärt:** Zeigt bekannte Computerkonten in der Domäne.

# Test
- Befehle auf DC und Client ausgeführt
- Ausgaben mit erwarteter Domänenkonfiguration abgeglichen

# Troubleshooting
- „Access denied“: Konsole als Administrator starten
- Unerwartete GP-Ergebnisse: `gpupdate /force` und Neustart durchführen
- `netdom` nicht gefunden: RSAT/AD-Tools prüfen

# Fazit
Diese Befehle decken zentrale Daily-Tasks in einer Windows-Domänenumgebung ab.
