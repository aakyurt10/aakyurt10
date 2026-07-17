# Ziel
Windows-Clients in die Domäne aufnehmen und zentrale Anmeldung ermöglichen.

# Voraussetzungen
- Client mit Netzwerkzugriff zum DC
- DNS des Clients zeigt auf den Domain Controller
- Domänenkonto mit Join-Berechtigung

# Umsetzung
- Computername nach Schema gesetzt (`CLIENT01`, `CLIENT02`)
- Domäne `lab.local` in den Systemeinstellungen eingetragen
- Domänenanmeldedaten verwendet und Neustart durchgeführt

# Test
- Anmeldung mit Domänenbenutzer möglich
- Computerobjekt erscheint in AD
- `nltest /dsgetdc:lab.local` liefert Domain Controller

# Troubleshooting
- „Domain not found“: DNS-Serveradresse und Namensauflösung geprüft
- „Access denied“: Berechtigung/Konto geprüft
- Vertrauensstellung defekt: Computerkonto zurückgesetzt und erneut beigetreten

# Fazit
Der Domänenbeitritt funktioniert auf beiden Clients und ermöglicht zentrale Benutzerverwaltung und GPO-Anwendung.
