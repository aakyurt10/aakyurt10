# Ziel
Desktop- und Benutzerumgebung standardisieren, um Supportaufwand zu reduzieren.

# Voraussetzungen
- Vorbereitete OU-Struktur
- Testbenutzer und Testclient

# Umsetzung
- Neue GPO für Benutzer-OU erstellt
- Beispielrichtlinien gesetzt (z. B. Hintergrund, Systemsteuerung einschränken)
- GPO mit Ziel-OU verknüpft

# Test
- Benutzer meldet sich an und erhält gewünschte Desktop-Konfiguration
- Änderungen sind über `gpresult /h` nachweisbar
- Zweiter Client zeigt identisches Verhalten

# Troubleshooting
- Richtlinie fehlt: Sicherheitsfilterung/WMI-Filter geprüft
- Verzögerte Anwendung: Hintergrundaktualisierung abgewartet oder forciert
- Falscher Benutzerbereich: GPO-Link auf korrekte OU gesetzt

# Fazit
Desktop-Richtlinien verbessern Konsistenz und sind ein zentraler Baustein in der Client-Verwaltung.
