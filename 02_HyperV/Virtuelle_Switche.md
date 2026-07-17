# Ziel
Ein stabiles virtuelles Netzwerk für Kommunikation zwischen Server und Clients bereitstellen.

# Voraussetzungen
- Hyper-V-Manager Zugriff
- Geplantes Netzsegment für das Lab

# Umsetzung
- Interner virtueller Switch `vSwitch-LAB` erstellt
- Alle VMs mit diesem Switch verbunden
- Statische IP für DC gesetzt, Clients per DHCP

# Test
- Ping zwischen DC und Clients erfolgreich
- DNS-Anfragen der Clients erreichen den DC
- Keine ungewollte Verbindung in Produktivnetz

# Troubleshooting
- Kein Netzwerk: falschen Switch an VM korrigiert
- Paketverlust: Netzwerkkartentreiber/Offloading geprüft
- Falsche IP: DHCP-Lease erneuert

# Fazit
Die Switch-Konfiguration stellt ein isoliertes, kontrollierbares Testnetz für alle Lab-Schritte bereit.
