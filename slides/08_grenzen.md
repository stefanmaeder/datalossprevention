# Grenzen

- Abhängigkeit von korrekt implementierten Kryptosystemen
    - TLS ist nur sicher, wenn die Implementierung und Konfiguration korrekt sind (z. B. sichere Cipher Suites, Zertifikatsvalidierung). Fehlkonfigurationen führen zu Schwachstellen.

- Komplexität des Managements
    - Zertifikatsausstellung, -erneuerung und -revokation erfordern organisatorischen Aufwand und spezielle Infrastruktur (PKI).

- Performance-Overhead
    - Kryptografische Operationen (Handshake, Verschlüsselung/Entschlüsselung) verursachen Rechenleistung und können Latenzen steigern, besonders bei vielen Verbindungen oder ressourcenbeschränkten Systemen.

- Keine vollständige Ende-zu-Ende-Sicherheit über Zwischenpunkte
    - TLS schützt nur den Transportweg zwischen Client und Server. Falls ein Proxy, Load Balancer oder ein MITM für legitime Kontrolle eingesetzt wird, wird Sicherheit des End-to-End-Kanals unterbrochen.

- Erschwerte Netzwerküberwachung / DLP
    - Durch starke Verschlüsselung werden Inhalte und Metadaten weitgehend verborgen, was klassische Deep Packet Inspection (DPI) oder DLP-Tools auf Netzwerkebene stark einschränkt.

- MDPI
    - Risiko durch Protokoll-Downgrades oder veraltete Versionen
    - Ältere TLS-Versionen (z. B. 1.0, 1.1) und schwache Cipher Suites sind angreifbar, wenn nicht entsprechend konfiguriert oder deaktiviert.
