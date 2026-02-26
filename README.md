# BayHaus.de - Historisches Website-Archiv (Mirror)

Dieses Repository dient als **historisches Archiv** (Mirror-Kopie) der alten BAYHAUS Immobilien Website (`www.bayhaus.de`), bevor diese 2026 im Zuge der Modernisierung abgeschaltet und durch eine komplett neue Architektur (Firebase/React) ersetzt wurde.

Der Zweck dieses Archivs ist es, Code, Struktur, Inhalte und damalige Konfigurationen fÃ¼r die Zukunft aufzubewahren, falls jemals Fragen aufkommen, was genau auf der alten Seite stand, wie das Setup aussah oder wer involviert war.

## 1. Ãœbersicht & Technologie

*   **Zustand:** Statische Kopie der Live-Seite von Anfang 2026.
*   **Ehemaliges CMS:** TYPO3 CMS (circa 2017 eingerichtet/zuletzt grundlegend aktualisiert).
*   **SSL / Sicherheit:** âŒ Kein HTTPS. Die alte Seite lief ausschlieÃŸlich Ã¼ber eine unverschlÃ¼sselte HTTP-Verbindung.
*   **Tracking/Analytics:** Es war **kein** aktiver Tracking-Code implementiert (Google Analytics wurde zwar in der DatenschutzerklÃ¤rung erwÃ¤hnt, aber im Quellcode nie genutzt).
*   **3rd-Party Scripts:** Keine wesentlichen externen Skripte. Lediglich TYPO3-eigenes JavaScript (`jsfunc.validateform.js`) und ein damals schon veraltetes Flash-Slideshow-Plugin kamen zum Einsatz.

## 2. Historische Hosting- & Infrastruktur-Daten

Die Seite und die dazugehÃ¶rigen Dienste waren historisch (Ã¼ber viele Jahre) gewachsen und Ã¼ber verschiedene Dienstleister verteilt. Hier ist die Rekonstruktion der **inaktiven/alten** Umgebung:

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
*   **Inhaberschaft bis zur Ãœbergabe:** Die Domains und der dd24-Account lagen verwaltungstechnisch auf dem Account von Dr. Danica Krunic. Heiner Stadler (GeschÃ¤ftsfÃ¼hrer BAYHAUS) hatte bei dd24 lediglich eine Kundennummer (`00915750`) fÃ¼r Support-Korrespondenz, die Rechnungen und Zahlungen liefen jedoch vollstÃ¤ndig Ã¼ber Danica.

### E-Mail-Infrastruktur
*   **Mail-Server (MX):** `mail.bayhaus.de` (Routete auf die IP `185.33.180.158`).
*   **Hosting:** Wahrscheinlich ebenfalls direkt in den Paketen bei domaindiscount24 (dd24) gehostet (die IP gehÃ¶rte jedenfalls nicht zum JWEILAND-Netzwerk).
*   **Umfang:** Etwa 5â€“6 aktive PostfÃ¤cher (u.a. `heinrich.stadler@bayhaus.de`, `info@bayhaus.de`) mit insgesamt ca. 30 GB Speichervolumen.

## 3. Beteiligte Personen (Stand bis Anfang 2026)

*   **Heinrich ("Heiner") Stadler:** GeschÃ¤ftsfÃ¼hrer der BAYHAUS Immobilien GmbH und Inhaber des GeschÃ¤fts.
*   **Dr. Danica Krunic ("Dany"):** Bisherige IT-Betreuerin (Ã¼ber ca. 20 Jahre hinweg). Betreute Webhosting, TYPO3, Domains und E-Mails Ã¼ber ihre Firma *Kunst und Kultur.org*. Berechnete Hosting und Domains Ã¼ber eine jÃ¤hrliche Sammelrechnung an Heiner.
*   **Frederik Stadler:** Neffe von Heiner Stadler. Hat die IT-Betreuung und Neuentwicklung der Website Anfang 2026 komplett Ã¼bernommen. Hat den Domain-Transfer (via INWX) aus dem Altvertrag gelÃ¶st und die komplette E-Mail-Infrastruktur modernisiert sowie eine neue Firebase-basierte Website hochgezogen.

## 4. Wichtige Hinweise fÃ¼r die Zukunft

*   **Eingefrorener Stand:** Dies ist ein "Read-Only" Archiv. Die archivierten Dateien sind stark veraltet und werden nicht mehr gewartet.
*   **Datenschutz / Sicherheit:** Aufgrund fehlender Updates enthalten die alten TYPO3-Fragmente wahrscheinlich SicherheitslÃ¼cken. Sie dÃ¼rfen unter keinen UmstÃ¤nden wieder auf einem Ã¶ffentlichen Webserver produktiv geschaltet oder ausgefÃ¼hrt werden.
*   **Fehlende Datenbank:** Da es sich oft bei solchen Mirrors um AbzÃ¼ge (Scrape / Download der fertig gerenderten Frontend-Dateien) handelt, ist die zugrundeliegende TYPO3-MySQL-Datenbank hier nicht zwangslÃ¤ufig enthalten. Die reinen Ausgabe-HTML-Dateien, CSS und Bilder der Seite sind jedoch zur Ansicht und als Dokumentation vorhanden.

## 5. Website-Struktur & Ehemalige Inhalte

Die alte Website war strukturell sehr einfach gehalten und diente primär als digitale Visitenkarte und Portfolio-Showcase.

### Haupt-Navigation
1.  **Bayhaus** (Startseite mit Unternehmensprofil)
2.  **Wohnimmobilien** (Aktuelle Angebote & Projekte)
3.  **Gewerbeobjekte** (Gewerbliche Angebote)
4.  **Profil** (Über die Geschäftsführung, Historie)
5.  **Referenzen** (Erfolgreich vermittelte/begleitete Großprojekte)
6.  **Impressum & Datenschutz**

### Bekannte Bauprojekte & Listings (Wohnimmobilien)
Auf der Unterseite /wohnimmobilien waren unter anderem folgende dedizierte Landingpages bzw. Projekt-Exposés verlinkt:
*   Alter Hof
*   Klostergarten
*   Knöbelblock
*   Olympiawohnpark
*   ParkSide
*   Schellinghöfe
*   Stadtquartier Am Südpark
*   Welfenhöfe
*   (Zusätzlich gab es eine Sektion 'Virtueller Spaziergang durch München')

### Referenz-Projekte (Showcase)
Auf der Seite /referenzen wurden signifikante Münchner Bauprojekte und Immobilien als Referenzen des Unternehmens aufgeführt:

**Wohnimmobilien-Referenzen:**
*   Klostergarten St. Anna im Lehel
*   Alter Hof Kaiserresidenz
*   Knöbelblock im Lehel
*   Schellinghöfe in Schwabing
*   Winzerer Straße Schwabing
*   Wohnen am Olympiaberg
*   ParkSide Agnes Bernauer Straße in Laim
*   Am Blumenanger in Waldtrudering
*   MAX III in Haidhausen, Innere Wiener Straße
*   Karlshöfe in der Karlstraße Maxvorstadt
*   Theresienhöhe  Wohnen am Park
*   Stadtwohnungen im Grünen am Arnulfpark

**Gewerbeobjekte-Referenzen:**
*   Elisenhof Stachus
*   Weißer Riese Arabellapark
*   Europäisches Patentamt

---
*Dieses README wurde automatisiert auf Basis des Quellcodes und der Übergabe-Dokumentation im Februar 2026 generiert.*
