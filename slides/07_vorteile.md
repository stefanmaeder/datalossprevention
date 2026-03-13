# Vorteile

- Vertraulichkeit (Confidentiality)
    - TLS verschlüsselt Daten am Transportlayer, sodass Inhalte vor passiven Lauscher:innen („Eavesdropping“) geschützt sind.
- Integritätsschutz der Daten
    - TLS stellt sicher, dass während der Übertragung keine unbemerkten Veränderungen am Datenstrom stattfinden.
- Authentifizierung von Kommunikationspartnern
    - Der Austausch digitaler Zertifikate und Public-Key-Kryptographie ermöglicht die eindeutige Identifikation von Servern (und optional Clients).
- TLS ist der dominierende Sicherheitsstandard im Internet (HTTPS, Mail, APIs). Dies schafft hohe Kompatibilität und breite Akzeptanz.
- Neuere Versionen (z. B. TLS 1.3) setzen obligatorisch sichere Verfahren wie Perfect Forward Secrecy (PFS), was Rückschlüsse aus späteren Schlüsselkompromittierungen verhindert.
