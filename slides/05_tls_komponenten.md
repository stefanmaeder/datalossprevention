# TLS Komponenten

- RFC 5246 erklärt, dass TLS aus zwei Schichten besteht: dem TLS Record Protocol und dem TLS Handshake Protocol, wobei das Record‑Protokoll auf einem zuverlässigen Transport (z. B. TCP) aufsetzt.
- Das Record‑Protokoll fragmentiert, optional komprimiert, authentifiziert (MAC) und verschlüsselt Anwendungsdaten, bevor sie gesendet werden; die Struktur TLSPlaintext mit ContentType, ProtocolVersion und length ist in Abschnitt 6 von RFC 2246 (TLS 1.0) erläutert.
- Change Cipher Spec Protocol: Signalisiert den Wechsel vom unverschlüsselten in den verschlüsselten Zustand (bzw. zwischen Cipher‑Spezifikationen), historisch als eigenes Mini‑Protokoll definiert.
​- Alert Protocol: Meldet Warnungen und Fehler (z. B. close_notify, bad_record_mac) an die Gegenstelle, damit diese die Verbindung korrekt beenden oder Fehler behandeln kann.
​- Application Data Protocol: Trägt die eigentlichen Anwendungsdaten (z. B. HTTP, IMAP) als Payload im Record‑Layer, nachdem der Handshake abgeschlossen und die Cipher aktiviert ist.
