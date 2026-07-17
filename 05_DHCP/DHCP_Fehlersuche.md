# Ziel
Typische DHCP-Probleme schnell erkennen und systematisch beheben.

# Voraussetzungen
- Zugriff auf DHCP-Konsole und betroffene Clients
- Befehle: `ipconfig`, Ereignisanzeige

# Umsetzung
- Prüfreihenfolge definiert: Dienst, Autorisierung, Scope, Optionen, Client
- Fehlerfälle dokumentiert (APIPA, falscher DNS, keine Lease)
- Gegenmaßnahmen pro Fehlerfall festgehalten

# Test
- Nach Korrektur gültige Lease am Client bestätigt
- Netzwerk- und Domänenzugriff wiederhergestellt
- DHCP-Logs zeigen erfolgreiche Vergaben

# Troubleshooting
- APIPA (`169.254.x.x`): DHCP-Erreichbarkeit geprüft
- Kein Offer: DHCP-Dienst neugestartet und Scope geprüft
- Falsche DNS-Option: Scope-Option 006 korrigiert

# Fazit
Mit klaren Prüfketten lassen sich DHCP-Fehler zuverlässig eingrenzen und beheben.
