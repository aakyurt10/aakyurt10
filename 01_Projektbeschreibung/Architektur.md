# Ziel
Die Architektur soll klar, nachvollziehbar und für ein kleines Home-Lab angemessen sein.

# Voraussetzungen
- Definierter IP-Adressbereich (z. B. 192.168.100.0/24)
- Benennungskonzept für Server und Clients
- Dokumentierte Rollenverteilung

# Umsetzung
- `DC01` (Windows Server 2022): AD DS, DNS, DHCP
- `CLIENT01`, `CLIENT02` (Windows 10/11): Domänen-Clients
- Interner Hyper-V Switch für isoliertes Testnetz
- Beispielwerte:
  - Domäne: `lab.local`
  - DC-IP: `192.168.100.10`
  - DHCP-Range: `192.168.100.100-200`

# Test
- Ping zwischen allen Systemen möglich
- Clients lösen `dc01.lab.local` korrekt auf
- DHCP vergibt gültige Adresse, Gateway und DNS

# Troubleshooting
- IP-Konflikte durch saubere DHCP-Ausschlüsse vermieden
- Falsche DNS-Einträge am Client durch `ipconfig /flushdns` und `ipconfig /renew` korrigiert
- Kommunikationsprobleme durch Windows-Firewall-Regeln geprüft

# Fazit
Die Architektur ist bewusst einfach, aber vollständig genug, um Kernaufgaben einer Windows-Server-Umgebung realistisch zu demonstrieren.
