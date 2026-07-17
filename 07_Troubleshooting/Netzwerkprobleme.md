# Ziel
Netzwerkprobleme zwischen VMs systematisch erkennen und lösen.

# Voraussetzungen
- Zugriff auf Hyper-V-Host und alle VMs
- Befehle: `ipconfig`, `ping`, `tracert`

# Umsetzung
- Prüfkette für Layer 1-3 im Lab definiert
- Hyper-V-Switch, IP-Konfig und Firewall als Hauptpunkte dokumentiert
- Wiederkehrende Fehler und Lösungen festgehalten

# Test
- Erreichbarkeit aller Systeme per Ping validiert
- Traceroute zeigt erwarteten Pfad im Lab-Netz
- Dienste (DNS/DHCP/AD) nach Netzfix wieder verfügbar

# Troubleshooting
- Kein Link: virtuellen Adapter/zugewiesenen Switch geprüft
- Falsches Subnetz: IP-Konfiguration korrigiert
- Blockierte ICMP-Pakete: Firewall-Regeln geprüft

# Fazit
Die Kombination aus Hyper-V- und IP-Prüfung deckt die meisten Netzwerkprobleme im Home-Lab zuverlässig ab.
