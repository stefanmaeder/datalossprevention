# Dienste mit TLS

- generisch für beliebige Client/Server‑Anwendungen über einem zuverlässigen Transport:
  - Web‑Dienste (HTTP)
  - E‑Mail‑Dienste (IMAP, POP3, SMTP)
  - Echtzeit‑Dienste (Messaging, VoIP)
  - VPN‑artige und Anwendungs‑VPN‑Szenarien

- RFC 2246 führt im Glossar „application protocol“ als jedes Protokoll auf, das typischerweise direkt über dem Transportlayer läuft, und nennt beispielhaft Protokolle wie Telnet, FTP, HTTP und SMTP, die durch TLS abgesichert werden können.
​
- RFC 5246 betont, dass der TLS Record Layer beliebige höhere Protokolle kapselt; konkret werden in der Praxis u. a. Datenbank‑Verbindungen (z. B. TLS für PostgreSQL/MySQL), Verzeichnisdienste (LDAP‑over‑TLS) und Management‑Protokolle (z. B. HTTPS‑basierte APIs) über TLS abgesichert.
