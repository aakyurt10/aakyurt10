# Ziel
Typische DNS-Störungen strukturiert analysieren und beheben.

# Voraussetzungen
- Zugriff auf DC und betroffenen Client
- Tools: `nslookup`, `ipconfig`, Eventanzeige

# Umsetzung
- Prüfreihenfolge festgelegt: Netzwerk, DNS-Server, Zone, Client-Cache
- Soll-Ist-Vergleich der DNS-Servereinstellungen durchgeführt
- Fehlerbilder und Gegenmaßnahmen dokumentiert

# Test
- Vorher/Nachher-Vergleich mit `nslookup`
- Domänenanmeldung nach Korrektur erfolgreich
- Eventlogs zeigen keine neuen DNS-Fehler

# Troubleshooting
- NXDOMAIN: fehlenden A-Record angelegt
- Falscher DNS am Client: Adapter oder DHCP korrigiert
- Intermittierende Fehler: Dienstneustart und Log-Analyse durchgeführt

# Fazit
Mit einer festen Prüfreihenfolge lassen sich DNS-Probleme schnell und reproduzierbar eingrenzen.
