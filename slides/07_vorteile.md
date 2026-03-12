# Vorteile

Vertraulichkeit (Confidentiality)
TLS verschlüsselt Daten am Transportlayer, sodass Inhalte vor passiven Lauscher*innen („Eavesdropping“) geschützt sind.
Beleg: RFC 8446 (Abstract) beschreibt explizit das Ziel, „eavesdropping“ zu verhindern. 
datatracker.ietf.org
Integritätsschutz der Daten
TLS stellt sicher, dass während der Übertragung keine unbemerkten Veränderungen am Datenstrom stattfinden.
Beleg: Die Sicherheitsziele von TLS umfassen Datenintegrität über Hash-basierte Mechanismen (HMAC). 
ncsc.nl
Authentifizierung von Kommunikationspartnern
Der Austausch digitaler Zertifikate und Public-Key-Kryptographie ermöglicht die eindeutige Identifikation von Servern (und optional Clients).
Beleg: TLS-Security-Guidelines erläutern Zertifikats-basierte Authentifikation im Handshake. 
ncsc.nl
Weit verbreitet und interoperabel
TLS ist der dominierende Sicherheitsstandard im Internet (HTTPS, Mail, APIs). Dies schafft hohe Kompatibilität und breite Akzeptanz.
Beleg: TLS gilt als „most widely used secure transmission protocol“ in der Forschungsliteratur zur verschlüsselten Traffic-Analyse. 
MDPI
Starker Schutz durch moderne Kryptografie
Neuere Versionen (z. B. TLS 1.3) setzen obligatorisch sichere Verfahren wie Perfect Forward Secrecy (PFS), was Rückschlüsse aus späteren Schlüsselkompromittierungen verhindert.
Beleg: TLS 1.3 erhebt PFS in den Stand der Pflicht und reduziert Angriffsflächen. 
MDPI
Schutz vor aktiven Angriffen
Durch Authentifikation, Verschlüsselung und Integritätsschutz ist TLS robust gegenüber klassischen aktiven Angriffen wie Datenmanipulation.
Beleg: NCSC/TLS-Security-Guidelines erläutern den Schutz des verschlüsselten Kanals.
