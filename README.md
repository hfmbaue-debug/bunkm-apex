# bunkm-apex

Nur ein Zweck: `bunkm.com` (ohne www) soll über HTTPS erreichbar sein und auf
`https://www.bunkm.com/` führen.

Warum nicht bei STRATO: das Domainpaket hat keinen Webspace, und die
Umleitung dort wird ohne Zertifikat ausgeliefert — `https://bunkm.com`
scheitert beim TLS-Handshake. STRATOs eigenes SSL kostet 30 €/Monat plus
100 € Einrichtung.

Warum nicht Cloudflare: dafür müssten die Nameserver zu Cloudflare, und
STRATO schaltet dann seine Mailfunktionen für die Domain ab —
kontakt@bunkm.com haengt daran.

GitHub Pages stellt das Zertifikat für den Apex aus. Nameserver, MX und das
Postfach bleiben unberuehrt; geaendert werden nur A- und AAAA-Records.
