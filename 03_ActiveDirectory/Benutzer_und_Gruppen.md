# Ziel
Benutzer- und Gruppenverwaltung praxisnah aufbauen, um Berechtigungen sauber steuern zu können.

# Voraussetzungen
- Funktionierende AD-Domäne
- Geplante Rollen (z. B. Azubi, Admin, Standarduser)

# Umsetzung
- Testbenutzer (z. B. `max.mustermann`) erstellt
- Sicherheitsgruppen (z. B. `GG_IT`, `GG_Azubis`) angelegt
- Benutzer den passenden Gruppen zugewiesen
- Namenskonvention für Konten dokumentiert

# Test
- Anmeldung mit Testbenutzer auf Client möglich
- Gruppenmitgliedschaften mit `whoami /groups` geprüft
- Rechte greifen entsprechend Gruppenmodell

# Troubleshooting
- Anmeldung nicht möglich: Konto deaktiviert/Passwort abgelaufen geprüft
- Rechte fehlen: Gruppenmitgliedschaft und Token-Aktualisierung geprüft
- Falsche OU: Objekt verschoben und Vererbung kontrolliert

# Fazit
Durch Gruppen statt Einzelberechtigungen ist die Verwaltung übersichtlich, skalierbar und fehlerärmer.
