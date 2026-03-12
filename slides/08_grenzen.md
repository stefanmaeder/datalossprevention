# Grenzen

Abhängigkeit von korrekt implementierten Kryptosystemen
TLS ist nur sicher, wenn die Implementierung und Konfiguration korrekt sind (z. B. sichere Cipher Suites, Zertifikatsvalidierung). Fehlkonfigurationen führen zu Schwachstellen.
Beleg: Verschiedene Studien und Standards zur sicheren Nutzung weisen auf Risiken durch Implementierungsfehler hin. 
rfc-editor.org
Komplexität des Managements
Zertifikatsausstellung, -erneuerung und -revokation erfordern organisatorischen Aufwand und spezielle Infrastruktur (PKI).
Beleg: TLS/DTLS Best Practice RFC verzeichnet allgemeine Risiken und Herausforderungen bei Zertifikatsverwaltung. 
rfc-editor.org
Performance-Overhead
Kryptografische Operationen (Handshake, Verschlüsselung/Entschlüsselung) verursachen Rechenleistung und können Latenzen steigern, besonders bei vielen Verbindungen oder ressourcenbeschränkten Systemen.
Beleg: Verschlüsselungsverfahren und zusätzliche Handshakes erzeugen Kosten im Betrieb, wie in verschiedenen Praxis-Analysen beschrieben. 
rfc-editor.org
Keine vollständige Ende-zu-Ende-Sicherheit über Zwischenpunkte
TLS schützt nur den Transportweg zwischen Client und Server. Falls ein Proxy, Load Balancer oder ein MITM für legitime Kontrolle eingesetzt wird, wird Sicherheit des End-to-End-Kanals unterbrochen.
Beleg aus verwandter Forschung: Studien zu TLS-Interception zeigen, dass klassische Überwachungstechniken die TLS-Ende-zu-Ende-Sicherheit aufbrechen müssen, um Inhalte sichtbar zu machen. 
arxiv.org
Erschwerte Netzwerküberwachung / DLP
Durch starke Verschlüsselung werden Inhalte und Metadaten weitgehend verborgen, was klassische Deep Packet Inspection (DPI) oder DLP-Tools auf Netzwerkebene stark einschränkt.
Beleg: Surveys zur Analyse von TLS-verschlüsseltem Traffic verdeutlichen, dass moderne TLS-Versionen traditionelle Inspektionstechniken „ineffective“ machen. 
MDPI
Risiko durch Protokoll-Downgrades oder veraltete Versionen
Ältere TLS-Versionen (z. B. 1.0, 1.1) und schwache Cipher Suites sind angreifbar, wenn nicht entsprechend konfiguriert oder deaktiviert.
Beleg: Empfehlungen und Standards zur sicheren Nutzung von TLS betonen, wie veraltete Konfigurationen Sicherheitslücken darstellen.
