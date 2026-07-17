# Ziel
Grundlagen von DNS im AD-Kontext verstehen und korrekt einordnen.

# Voraussetzungen
- Laufender Domain Controller
- Basiswissen zu Hostnamen und IP-Adressen

# Umsetzung
- Rolle von DNS für AD erklärt (SRV-Records, Namensauflösung)
- Forward-Lookup-Zone für `lab.local` genutzt
- A- und PTR-Einträge als Kernobjekte dokumentiert

# Test
- `nslookup dc01.lab.local` liefert korrekte IP
- Reverse Lookup funktioniert für Client und Server
- Domänenanmeldung ohne Namensfehler möglich

# Troubleshooting
- Falsche Antworten: doppelte/alte DNS-Einträge bereinigt
- Zeitüberschreitung: DNS-Dienst und Firewall geprüft
- Kein Reverse Lookup: PTR-Zone ergänzt

# Fazit
DNS ist der zentrale Dienst für eine stabile AD-Umgebung und wurde im Lab nachvollziehbar aufgebaut.
