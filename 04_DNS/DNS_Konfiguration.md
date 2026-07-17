# Ziel
DNS-Server so konfigurieren, dass interne Namensauflösung für die Domäne zuverlässig funktioniert.

# Voraussetzungen
- Installierte DNS-Serverrolle
- Statische IP auf dem DC

# Umsetzung
- Zone `lab.local` geprüft/verwaltet
- Dynamische Updates für AD-integrierte Zone aktiviert
- Forwarder für externe Auflösung gesetzt (optional)
- Wichtige Hosteinträge dokumentiert

# Test
- Clients lösen interne Hostnamen auf
- `nslookup` gegen DC als DNS-Server erfolgreich
- AD-bezogene SRV-Records vorhanden

# Troubleshooting
- Externe Auflösung fehlerhaft: Forwarder und Root-Hints geprüft
- Client nutzt falschen DNS: DHCP-Option 006 geprüft
- Alte Cache-Einträge: DNS- und Client-Cache geleert

# Fazit
Die DNS-Konfiguration unterstützt sowohl AD-Funktion als auch stabile Namensauflösung im Lab.
