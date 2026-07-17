# Ziel
Typische DNS-Störungen im AD-Lab schnell eingrenzen und beheben.

# Voraussetzungen
- Zugriff auf DNS-Manager und Clients
- Befehle: `nslookup`, `ipconfig`, `dcdiag`

# Umsetzung
- Prüfablauf erstellt: Client-Konfig, Serverdienst, Zonen, Records
- Häufige Fehlerbilder mit konkreten Korrekturen dokumentiert
- Fokus auf AD-relevante DNS-Funktion gelegt

# Test
- Vorher/Nachher mit `nslookup` verglichen
- AD-Anmeldung und Namensauflösung erneut getestet
- `dcdiag /test:dns` ohne kritische Fehler

# Troubleshooting
- Falscher DNS-Server am Client korrigiert
- Fehlender Hostrecord manuell ergänzt
- DNS-Cache auf Client und Server geleert

# Fazit
DNS-Probleme sind meist schnell lösbar, wenn die Analyse strukturiert und AD-fokussiert erfolgt.
