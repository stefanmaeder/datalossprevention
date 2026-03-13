# TLS Komponenten

- TLS Record Protocol
    - fragmentiert, optional komprimiert, authentifiziert (MAC) und verschlüsselt Anwendungsdaten, bevor sie gesendet werden
- TLS Handshake Protocol
- Change Cipher Spec Protocol
    - signalisiert den Wechsel vom unverschlüsselten in den verschlüsselten Zustand (bzw. zwischen Cipher‑Spezifikationen)
- Alert Protocol
    - Meldet Warnungen und Fehler (z. B. close_notify, bad_record_mac) an die Gegenstelle, damit diese die Verbindung korrekt beenden oder Fehler behandeln kann.
​
- Application Data Protocol
    - Trägt die eigentlichen Anwendungsdaten (z. B. HTTP, IMAP) als Payload im Record‑Layer, nachdem der Handshake abgeschlossen und die Cipher aktiviert ist.
