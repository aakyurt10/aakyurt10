# Ziel
Häufige Domain-Join-Probleme im Home-Lab reproduzierbar lösen.

# Voraussetzungen
- Zugriff auf Client und Domain Controller
- Tools: `ping`, `nslookup`, `netdom`, Ereignisanzeige

# Umsetzung
- Ursachenliste erstellt: DNS, Zeit, Rechte, Netzwerk
- Standard-Checkliste für Join-Fehler dokumentiert
- Wiederbeitritt-Prozess (Remove/Join) beschrieben

# Test
- Fehlerfall nachgestellt (falscher DNS am Client)
- Problem behoben und erfolgreicher Join erneut durchgeführt
- Anmeldung mit Domänenkonto bestätigt

# Troubleshooting
- „Domäne nicht gefunden“: DNS-Einstellung korrigiert
- „Zugriff verweigert“: Join-Berechtigung geprüft
- Vertrauensproblem: Computerkonto zurückgesetzt und neu beigetreten

# Fazit
Mit fester Checkliste lassen sich Join-Fehler schnell analysieren und ohne Trial-and-Error lösen.
