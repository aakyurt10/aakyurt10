# Windows Server AD Projekt (Home Lab)

## Projektübersicht
Dieses Repository dokumentiert mein praktisches Home-Lab-Projekt im Rahmen meiner Umschulung zum Fachinformatiker für Systemintegration (FISI).  
Ich baue eine kleine, realistische Windows-Server-Umgebung auf und dokumentiere alle Schritte verständlich und praxisnah.

## Verwendete Technologien
- Hyper-V
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Group Policy (GPO)
- Windows 10/11 Clients
- PowerShell und klassische Admin-Tools

## Lab-Architektur
Kleines Home-Lab ohne fiktive Enterprise-Komplexität:
- 1x Hyper-V Host
- 1x Windows Server 2022 (Domain Controller)
- AD DS, DNS und DHCP auf dem Server
- 2x Windows Clients für Domänenbeitritt und Tests

## Lernziele
- Sichere Grundkonfiguration eines Domain Controllers
- Strukturierte Benutzer- und Gruppenverwaltung
- DNS- und DHCP-Basisbetrieb in einer AD-Umgebung
- Einsatz und Test von Gruppenrichtlinien
- Systematisches Troubleshooting bei typischen Fehlern
- Professionelle technische Dokumentation

## Gezeigte Skills
- Installation und Konfiguration von Serverrollen
- Planung einer OU-Struktur
- Erstellung von Benutzern, Gruppen und Richtlinien
- Domänenbeitritt von Clients
- Analyse mit Standardbefehlen (z. B. dcdiag, nslookup, gpresult)
- Fehleranalyse mit klaren Testschritten

## Repository-Struktur
- `01_Projektbeschreibung/` Projektziele, Lab-Übersicht, Architektur
- `02_HyperV/` Hyper-V Installation, VM-Erstellung, virtuelle Switches
- `03_ActiveDirectory/` AD-Installation, OU-Struktur, Benutzer/Gruppen, Domänenbeitritt
- `04_DNS/` DNS Grundlagen, Konfiguration, Fehlersuche
- `05_DHCP/` DHCP Konfiguration, Scope-Planung, Fehlersuche
- `06_GPO/` Passwort- und Desktop-Richtlinien, GPO-Tests
- `07_Troubleshooting/` typische Probleme bei Domain Join, DNS und Netzwerk
- `08_Command_Reference/` wichtige Admin-Befehle mit Beispielen
- `09_Lernnotizen/` Erkenntnisse und Lessons Learned

## Screenshots
Geplant/ergänzt in den jeweiligen Fachdokumenten:
- Hyper-V VM-Übersicht
- AD-Benutzer und OU-Struktur
- DNS- und DHCP-Konfiguration
- GPO-Ergebnisse auf Client
- Beispiel-Fehlerbilder bei Troubleshooting

## Zukünftige Verbesserungen
- Zusätzlicher Member Server für Rollen-Trennung
- Grundlegende Backup-Strategie (System State)
- WSUS-/Patch-Management-Dokumentation
- Erweiterte GPO-Szenarien (z. B. Laufwerkszuordnung)
