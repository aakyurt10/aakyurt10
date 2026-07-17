# Ziel
Hyper-V auf dem Host aktivieren, um Server- und Client-VMs stabil betreiben zu können.

# Voraussetzungen
- Windows Pro/Enterprise als Host
- BIOS/UEFI Virtualisierung aktiviert
- Genügend RAM und Speicherplatz

# Umsetzung
- Hyper-V-Rolle über Windows-Features aktiviert
- Neustart des Hosts durchgeführt
- Hyper-V-Manager für Verwaltung genutzt
- Standardpfade für VMs und VHDX geprüft

# Test
- Hyper-V-Manager startet ohne Fehler
- Neue Test-VM kann erstellt und gestartet werden
- Host-Ressourcen werden korrekt angezeigt

# Troubleshooting
- Hyper-V fehlt in Features: Host-Edition geprüft
- VM startet nicht: VT-x/AMD-V im BIOS kontrolliert
- Performance schwach: RAM-Zuweisung und dynamischen Speicher geprüft

# Fazit
Die Hyper-V-Installation ist die technische Basis für das gesamte Projekt und wurde stabil eingerichtet.
