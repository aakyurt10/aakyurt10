# Ziel
Eine sichere Passwort-Richtlinie für Domänenbenutzer anwenden.

# Voraussetzungen
- Funktionierende AD-Domäne
- Zugriff auf Gruppenrichtlinienverwaltung (GPMC)

# Umsetzung
- Default Domain Policy für Passwortregeln angepasst
- Mindestlänge, Komplexität und Ablaufzeit definiert
- Kontosperrrichtlinie ergänzt (Fehlversuche/Lockout)

# Test
- Neues Passwort wird gegen Richtlinie geprüft
- Zu schwache Passwörter werden abgelehnt
- `gpresult /r` zeigt angewendete Richtlinie

# Troubleshooting
- Richtlinie greift nicht: Replikation und GPO-Verknüpfung geprüft
- Alte Werte aktiv: `gpupdate /force` und Neustart durchgeführt
- Konflikte: Priorität und Enforced-Status geprüft

# Fazit
Die Passwort-Richtlinie erhöht die Basissicherheit und zeigt praxisnah den Einsatz zentraler Policies.
