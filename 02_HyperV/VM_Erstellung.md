# Ziel
Virtuelle Maschinen für Domain Controller und zwei Clients strukturiert anlegen.

# Voraussetzungen
- Vorhandene Hyper-V-Installation
- ISOs für Windows Server 2022 und Clients
- Geplantes Ressourcenprofil je VM

# Umsetzung
- `DC01` als Gen2-VM erstellt (z. B. 4 GB RAM, 2 vCPU)
- `CLIENT01` und `CLIENT02` als Gen2-VMs erstellt
- VHDX-Dateien pro VM getrennt angelegt
- Boot-Reihenfolge und ISO-Mount korrekt gesetzt

# Test
- Alle VMs booten in das Setup
- Installation abgeschlossen und lokale Anmeldung möglich
- Host bleibt unter Last stabil

# Troubleshooting
- Boot-Fehler: Secure-Boot-Vorlage geprüft
- ISO wird nicht erkannt: Datenträger neu eingebunden
- RAM-Engpass: dynamischen Speicher sinnvoll konfiguriert

# Fazit
Die VM-Struktur ist übersichtlich und unterstützt reproduzierbare Tests in allen weiteren Kapiteln.
