# Ziel
Einen sauberen DHCP-Scope planen, damit Adressvergabe stabil und konfliktfrei läuft.

# Voraussetzungen
- Netzwerkplan und reservierte statische Adressen
- Kenntnis der benötigten Client-Anzahl

# Umsetzung
- Beispiel-Scope: `192.168.100.100-192.168.100.200`
- Ausschlüsse für statische Systeme definiert (z. B. DC, Drucker)
- Reservierungen für spezielle Clients dokumentiert
- Lease-Dauer passend zur Lab-Nutzung gewählt

# Test
- Mehrere Clients erhalten unterschiedliche Adressen
- Keine Überschneidung mit statischen IPs
- Reservierte MAC erhält feste vorgesehene IP

# Troubleshooting
- Konflikte: Scope-Grenzen und statische IPs abgeglichen
- Falsche Reservierung: MAC-Adresse korrigiert
- Adresspool erschöpft: Scope erweitert oder Leasedauer angepasst

# Fazit
Ein strukturierter Scope verhindert Adressprobleme und macht das Netzwerk im Lab nachvollziehbar.
