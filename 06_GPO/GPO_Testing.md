# Ziel
GPO-Änderungen kontrolliert testen, bevor sie breit eingesetzt werden.

# Voraussetzungen
- Test-OU mit Pilot-Benutzern/Clients
- Zugriff auf GPMC und Clients

# Umsetzung
- Test-GPO zunächst nur auf Pilot-OU verknüpft
- Erwartetes Verhalten pro Richtlinie dokumentiert
- Rollback-Plan (GPO deaktivieren/entfernen) vorbereitet

# Test
- `gpupdate /force` ausgeführt
- `gpresult /r` und Ereignisanzeige ausgewertet
- Soll-Ist-Vergleich pro Richtlinie dokumentiert

# Troubleshooting
- Keine Wirkung: falsche OU oder ACL auf GPO geprüft
- Teilweise Wirkung: Benutzer-/Computerkontext getrennt geprüft
- Instabilität: zuletzt geänderte Einstellung isoliert getestet

# Fazit
Strukturiertes GPO-Testing vermeidet Fehlkonfigurationen und erhöht die Betriebssicherheit.
