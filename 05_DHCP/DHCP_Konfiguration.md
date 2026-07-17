# Ziel
DHCP auf dem Domain Controller konfigurieren, damit Clients automatisch gültige Netzwerkeinstellungen erhalten.

# Voraussetzungen
- Installierte DHCP-Serverrolle
- Autorisierung des DHCP-Servers in AD
- Geplanter IP-Bereich

# Umsetzung
- DHCP-Rolle installiert und in AD autorisiert
- Bereich (Scope) für Client-IPs erstellt
- Optionen gesetzt: DNS-Server, Domänenname, ggf. Gateway
- Leasedauer praxisnah konfiguriert

# Test
- Client erhält per `ipconfig /renew` eine gültige Lease
- Lease ist in der DHCP-Konsole sichtbar
- DNS-Serveroption wird korrekt verteilt

# Troubleshooting
- Keine Lease: Scope aktiv und verfügbarer Bereich geprüft
- Server nicht autorisiert: AD-Autorisierung nachgeholt
- Falsche Optionen: Scope-Optionen angepasst und Lease erneuert

# Fazit
Die DHCP-Konfiguration reduziert manuelle Fehler und beschleunigt die Client-Bereitstellung.
