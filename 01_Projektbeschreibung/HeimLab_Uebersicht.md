# Ziel
Das Home-Lab soll eine kleine, realistische Windows-Domäne abbilden, um typische FISI-Aufgaben praktisch zu üben.

# Voraussetzungen
- PC/Laptop mit aktivierter Virtualisierung
- Windows 10/11 Pro oder höher für Hyper-V
- ISO für Windows Server 2022 und Windows Client
- Grundkenntnisse TCP/IP

# Umsetzung
- Hyper-V als Virtualisierungsplattform eingerichtet
- 1 Domain Controller mit AD DS, DNS und DHCP aufgebaut
- 2 Clients als Testsysteme erstellt
- Alle Systeme in einem internen Testnetz segmentiert

# Test
- Alle VMs starten fehlerfrei
- Clients erhalten IP per DHCP
- DNS-Namensauflösung zum Domain Controller funktioniert
- Anmeldung mit Domänenkonto auf beiden Clients möglich

# Troubleshooting
- VM ohne Netzwerk: virtuellen Switch und Adapterbindung geprüft
- Kein DHCP-Lease: DHCP-Dienststatus und Scope-Aktivierung geprüft
- Domain Join Fehler: Uhrzeit, DNS-Server-Eintrag und Erreichbarkeit geprüft

# Fazit
Das Lab bildet typische Aufgaben aus der Systemadministration praxisnah ab und ist als Lern- und Portfolio-Umgebung geeignet.
