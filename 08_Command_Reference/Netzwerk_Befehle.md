# Ziel
Zentrale Netzwerkbefehle für Diagnose im Home-Lab dokumentieren.

# Voraussetzungen
- CMD oder PowerShell
- Netzwerkverbindung zwischen Lab-Systemen

# Umsetzung
## ipconfig
- **Zweck:** Zeigt IP-Konfiguration eines Hosts.
- **Syntax:** `ipconfig [/all]`
- **Beispiel:** `ipconfig /all`
- **Beispielausgabe erklärt:** Zeigt IP, Subnetz, DNS-Server, Lease-Infos.

## ping
- **Zweck:** Prüft Erreichbarkeit eines Ziels.
- **Syntax:** `ping <ziel>`
- **Beispiel:** `ping dc01.lab.local`
- **Beispielausgabe erklärt:** Antwortzeit und Paketverlust zeigen Verbindungsqualität.

## tracert
- **Zweck:** Zeigt Weg der Pakete bis zum Ziel.
- **Syntax:** `tracert <ziel>`
- **Beispiel:** `tracert dc01.lab.local`
- **Beispielausgabe erklärt:** Listet Hops; hilft bei Routing-Problemen.

## nslookup
- **Zweck:** Prüft DNS-Namensauflösung.
- **Syntax:** `nslookup <name>`
- **Beispiel:** `nslookup client01.lab.local`
- **Beispielausgabe erklärt:** Zeigt antwortenden DNS-Server und aufgelöste IP.

# Test
- Befehle auf beiden Clients ausgeführt
- Ergebnisse mit Soll-Netzkonfiguration verglichen

# Troubleshooting
- Ping ohne Antwort: Firewall, DNS und IP-Routing prüfen
- Falsche DNS-Antwort: DNS-Cache leeren und Zone prüfen
- APIPA-Adresse: DHCP-Erreichbarkeit testen

# Fazit
Diese Befehle sind die Basis für schnelle Erstdiagnosen in Windows-Netzwerken.
