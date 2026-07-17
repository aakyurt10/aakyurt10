# Ziel
Eine klare OU-Struktur schaffen, um Benutzer, Computer und Richtlinien logisch zu organisieren.

# Voraussetzungen
- Domäne ist betriebsbereit
- Strukturplan (z. B. Users, Clients, Servers, Admins)

# Umsetzung
- OUs für Benutzer, Clients und Administration angelegt
- Objekte in passende OUs verschoben
- GPO-Verknüpfung auf OU-Ebene vorbereitet

# Test
- Neue Benutzer landen in geplanter OU
- GPO-Verknüpfung wirkt nur auf Ziel-OU
- Delegation kann OU-bezogen getestet werden

# Troubleshooting
- GPO greift nicht: falsche OU oder Sicherheitsfilter geprüft
- Objekt nicht sichtbar: ADUC-Ansicht und Replikation geprüft
- Versehentliche Verschiebung: Schutz vor Löschung aktiviert

# Fazit
Die OU-Struktur verbessert Ordnung, Delegation und gezielte Richtliniensteuerung im Lab.
