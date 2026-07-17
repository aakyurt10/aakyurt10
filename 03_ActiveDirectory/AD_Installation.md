# Ziel
Active Directory Domain Services auf Windows Server 2022 installieren und neue Domäne bereitstellen.

# Voraussetzungen
- Server mit statischer IP
- Korrekte Zeitzone/Uhrzeit
- Lokale Administratorrechte

# Umsetzung
- AD DS-Rolle und Management-Tools installiert
- Server zum Domain Controller heraufgestuft
- Neue Gesamtstruktur `lab.local` erstellt
- Neustart und Anmeldung als Domänenadministrator durchgeführt

# Test
- `Active Directory-Benutzer und -Computer` öffnet ohne Fehler
- `dcdiag` zeigt keine kritischen Fehler
- SYSVOL/NETLOGON Freigaben vorhanden

# Troubleshooting
- Promotion-Fehler: DNS-Voraussetzungen geprüft
- Replikationswarnungen: Eventlog und Dienste geprüft
- Anmeldung schlägt fehl: Domänenname und Zeitabweichung kontrolliert

# Fazit
Die AD-Installation wurde erfolgreich abgeschlossen und bildet die zentrale Identitätsplattform des Labs.
