# BayHaus.de - Historisches Website-Archiv (Mirror)

Dieses Repository dient als **historisches Archiv** (Mirror-Kopie) der alten BAYHAUS Immobilien Website (`www.bayhaus.de`), bevor diese 2026 im Zuge der Modernisierung abgeschaltet und durch eine komplett neue Architektur (Firebase/React) ersetzt wurde.

Der Zweck dieses Archivs ist es, Code, Struktur, Inhalte und damalige Konfigurationen für die Zukunft aufzubewahren, falls jemals Fragen aufkommen, was genau auf der alten Seite stand, wie das Setup aussah oder wer involviert war.

## 1. Übersicht & Technologie

*   **Zustand:** Statische Kopie der Live-Seite von Anfang 2026.
*   **Ehemaliges CMS:** TYPO3 CMS (circa 2017 eingerichtet/zuletzt grundlegend aktualisiert).
*   **SSL / Sicherheit:** ❌ Kein HTTPS. Die alte Seite lief ausschließlich über eine unverschlüsselte HTTP-Verbindung.
*   **Tracking/Analytics:** Es war **kein** aktiver Tracking-Code implementiert (Google Analytics wurde zwar in der Datenschutzerklärung erwähnt, aber im Quellcode nie genutzt).
*   **3rd-Party Scripts:** Keine wesentlichen externen Skripte. Lediglich TYPO3-eigenes JavaScript (`jsfunc.validateform.js`) und ein damals schon veraltetes Flash-Slideshow-Plugin kamen zum Einsatz.

## 2. Historische Hosting- & Infrastruktur-Daten

Die Seite und die dazugehörigen Dienste waren historisch (über viele Jahre) gewachsen und über verschiedene Dienstleister verteilt. Hier ist die Rekonstruktion der **inaktiven/alten** Umgebung:

### Webhosting (TYPO3)
*   **Hoster:** JWEILAND (spezialisiertes TYPO3-Hosting). 
*   **Infrastruktur:** Die physischen Server lagen im Rechenzentrum von *domainfactory* (bzw. Host Europe).
*   **Webserver:** nginx
*   **Historische IP-Adresse:** `134.119.225.135`
*   **Hostname:** `mc21466.ispgateway.de`

### Domains & DNS
Die Domains (`bayhaus.de` und `bayhaus.com`) wurden nicht beim Webhoster direkt verwaltet, sondern waren logisch getrennt.
*   **Registrar / Technischer Verwalter:** domaindiscount24 (dd24).
*   **DNS (Nameserver):** `ns1/ns2/ns3.domaindiscount24.net`
*   **Inhaberschaft bis zur Übergabe:** Die Domains und der dd24-Account lagen verwaltungstechnisch auf dem Account von Dr. Danica Krunic. Heiner Stadler (Geschäftsführer BAYHAUS) hatte bei dd24 lediglich eine Kundennummer (`00915750`) für Support-Korrespondenz, die Rechnungen und Zahlungen liefen jedoch vollständig über Danica.

### E-Mail-Infrastruktur
*   **Mail-Server (MX):** `mail.bayhaus.de` (Routete auf die IP `185.33.180.158`).
*   **Hosting:** Wahrscheinlich ebenfalls direkt in den Paketen bei domaindiscount24 (dd24) gehostet (die IP gehörte jedenfalls nicht zum JWEILAND-Netzwerk).
*   **Umfang:** Etwa 5–6 aktive Postfächer (u.a. `heinrich.stadler@bayhaus.de`, `info@bayhaus.de`) mit insgesamt ca. 30 GB Speichervolumen.

## 3. Beteiligte Personen (Stand bis Anfang 2026)

*   **Heinrich ("Heiner") Stadler:** Geschäftsführer der BAYHAUS Immobilien GmbH und Inhaber des Geschäfts.
*   **Dr. Danica Krunic ("Dany"):** Bisherige IT-Betreuerin (über ca. 20 Jahre hinweg). Betreute Webhosting, TYPO3, Domains und E-Mails über ihre Firma *Kunst und Kultur.org*. Berechnete Hosting und Domains über eine jährliche Sammelrechnung an Heiner.
*   **Frederik Stadler:** Neffe von Heiner Stadler. Hat die IT-Betreuung und Neuentwicklung der Website Anfang 2026 komplett übernommen. Hat den Domain-Transfer (via INWX) aus dem Altvertrag gelöst und die komplette E-Mail-Infrastruktur modernisiert sowie eine neue Firebase-basierte Website hochgezogen.

## 4. Wichtige Hinweise für die Zukunft

*   **Eingefrorener Stand:** Dies ist ein "Read-Only" Archiv. Die archivierten Dateien sind stark veraltet und werden nicht mehr gewartet.
*   **Datenschutz / Sicherheit:** Aufgrund fehlender Updates enthalten die alten TYPO3-Fragmente wahrscheinlich Sicherheitslücken. Sie dürfen unter keinen Umständen wieder auf einem öffentlichen Webserver produktiv geschaltet oder ausgeführt werden.
*   **Fehlende Datenbank:** Da es sich oft bei solchen Mirrors um Abzüge (Scrape / Download der fertig gerenderten Frontend-Dateien) handelt, ist die zugrundeliegende TYPO3-MySQL-Datenbank hier nicht zwangsläufig enthalten. Die reinen Ausgabe-HTML-Dateien, CSS und Bilder der Seite sind jedoch zur Ansicht und als Dokumentation vorhanden.
