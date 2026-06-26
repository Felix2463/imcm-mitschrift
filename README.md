# Imcm-Mitschrift

Das ist das README.mad File unseres Repositories. Die Dateiendung .md für Markdown - eine heute sehr weit verbreitete [Auszeichnungssprache] (https://de.wikipedia.org/wiki/Auszeichnungssprache). Weitere bekannte Auszeichnungssprachen sind:
Learning\* heißen.

- Hypertext Markup Language (HTML)
- Extensible Markup Language (XML)
- Yet Another Markup Language (YAML, YML)

> **Achtung!**
> Die Abkürzung ML steht nicht immer für _Markup Language_, sie kann auch \*Machinechlag noch funktioniert (Kontext des kalten Krieges)

## Playlist zur Funktionsweise des Internets

![TCP-IP-Modell](/assets/https___miro.medium.com_v2_resize_fit_720_format_webp_1_g1GzSjM5-J3aN2wjVz6qKA.png)

### Teil 1 - What is the Internet?

- das Internet wurde in den 1970er-Jahren entwickelt
- Motivation: Schaffung eines dezentrales Netzwerks, das auch nach einem Atomans
- Funktionsweise: Paketvermittlung (_Packet Switching_) - Nachrichten bzw. Dateien werden in kleine Pakete aufgeteilt und unabhängig voneinander über das Netzwerk verschickt
- Internet: das Netz der Netze - besteht aus vielen kleineren Netzen unterschiedlicher Internetanbieter (_Internet Service Provider - ISP_, z.B.: Salzburg AG, Magenta, A1, ...)

### Teil 2 - The Internet: Wires, Cables and WiFi

Informationen werden im Internet als Bits übertragen. Bits zwei Werte: 0 und 1. 8 Bits zusammengefasst ergebebn 1 Byte. Mit einem Byte kann man 256 verschiedene Werte speichern (2^8).

Bits können über verschiedene Übertragungsmedien zwischen Computern versendet werden. Die Anzahl der übertragenen Bits pro Sekunde wird als **Bandbreite** bezeichnet. Bei einer Bandbreite von 300MBit/s können beispielsweise 300 Millionen Bit pro Sekunde über die Leitung laufen. Übertragungsmedien können sein:

**1. Elektrizität / Kupferdraht (Ethernet)**

- billig
- einfach in der Verarbeitung
- weit verbreitet
- hohe Verluste über mittlere und lange Distanzen (hunderte Meter)

**2. Licht / Glasfaserkabel**

- extrem schnell
- verlustfrei
- geeignet für Ozeankabel
- teuer und schwierig in der Verarbeitung

**3. Funk / Radiowellen**

- hoher Komfort, Internet überall

### Teil 3 - The Internet: IP-Adresses & DNS

- Protokolle sind die Tegeln der Kommunikation
- eines der wichtigsten Protokolle im Internet ist das Internet Protokoll (IP)
- jedes Gerät im Internet hat zumindest eine (eindeutige) IP-Adresse, viele Geräte haben eine externe IP (ähnlich wie die Hausnummer) und eine interne IP (ähnlich wie die Raumnummer)
- das _Domain Name System_ (DNS) übersetzt menschenlesbare Domainnamen (z.B.:wwww.google.com) in IP-Adressen
- DNS-Server führen Tabellen mit Domainnamen und en entsprechenden Ip-Adressen

### Teil 4 - The Internet: Packets, Routing & Reliability

- über das Internet versendete Daten in Pakete aufgeteilt
- einzelne Pakete haben eine Größe von ca. 1,5kB. D.h., ein Foto mit einer Größe von 10MB wird in ca. 6700 Pakete aufgeteilt, bevor es über das Internet versendet wird
- Pakete können unterschiedliche Routen durch das Internet nehmen. Die Route wird je nach Auslastung, Störungen etc. durch spezielle Computer - die Router - dynamisch bestimmt.
- jedes Paket enthält dei Quell- und Ziel-IP-Adresse sowie eine eindeutige Paketnummer
- das _Transmission Control Protocol_ (TCP) prüft am Ziel, ob alle Pakete einer Übertragung angekommen sind. Falls Pakete fehlen, fordert es diese erneut vom Absender an.
- TCP und IP bilden gemeinsam das Rückrad des Internets. Man spricht daher auch vom TCP/IP-Modell bzw. _TCP/IP-Stack_.

### Teil 5 - The Internet: HTTP & HTML

- http steht für _Hypertext Transport Protocol_. HTTP arbeitet nach dem Client-Server-Prinzip:

  - ein Web-Client (Browser) sendet eine Anfrage (_request_) an einen Web-Server
  - der Web-Server verarbeitet die Anfrage und sendet eine Antwort (_response_) zurück. Die Antwort u.a. einen sogenannten [HTTP-Statuscode](https://de.wikipedia.org/wiki/HTTP-Statuscode), der Auskunft über die Verarbeitung der Anfrage gibt.

  > #### HTTP-Statuscode
  >
  > - **1xx** - die Anfrage dauert noch an
  > - **2xx** - die Anfrage war erfolgreich
  > - **3xx** - Um- oder Weiterleitung
  > - **4xx** - Clientfehler (z.B. 404 - _Page not found_)
  > - **5xx** - Serverfehler 💀

- HTTP-Anfragen werden immer mit einer **HTTP-Methode** übertragen
- Daten (HTML-Seiten, Bilder, Videos, ...) werden mit GET-Anfragen angefordert
- Benutzereingaben (Z.B. aus Formularfeldern - z.B. Passwort, Datein-Uploads, ...) werden mit POST-Anfragen verschlüsselt versendet
- es gibt auch andere HTTP-Methoden. Diese lernen wir aber erst später.
- HTTP*Anfragen und -Antworten können auch **Cookies** enthalten. Cookies sind kleine Textdateien, die aus Schlüssel-Wert-Paaren (*\_key-value-Pairs*) bestehen. Sie werden bei jeder Anfrage vom Client mitgesendet und ermöglichen so u.a. die Indentifikation einzelner Nutzer.

### Teil 8 - The Internet: How Search Works

- Suchmaschinen-Bots (_Crawler_) durchstreifen ständig das WWW und katalogisieren Websites. Der so entstehende Katalog wird auch **Index** genannt
- wenn wir einen Suchbegriff bei Google (oder einer anderen _Search Engine_) eingeben, wird NICHT das WWW durchsucht, sondern lediglich der zuvor erstellte Index
- Suchergebnisse werden auf Basis eines (geheimen) Algorithmus geranked - Ergebnisse, die weiter oben stehen, werden öfter angeklickt
- Einfluss auf das Ranking haben u.a.:
  - im Text vorkommende Suchbegriffe (_Keywords_)
  - Links die auf meine Seite zeigen (_Backlinks_)
- die Suchergebnisse werden an die Benutzer\*innen angepasst! D.h., nicht jede/r sieht die gleichen Informationen, selbst wenn sie idente Suchanfragen durchführen!
- [Startpage](https://www.starpage.com/) ist eine Datensparsame Suchmaschine, die ihren Benutzer\*innen die Verwendung von Google ohne Tracking oder Personalisierung erlaubt

---

### Ergänzung: Überblick über das TCP/IP-Modell

Im TCP/IP-Modell übernimmt jede Schicht eine eigene Aufgabe (merke: *divide and conquer*), hat einen eigenen Namen für die versendeten Dateneinheiten und einen eigenen Adressierungsmechanismus:

| Schicht | Protokoll | Dateneinheit | Adressen | 
| --- | --- | --- | --- |
| Internet | IP | Paket | Ip-Adressen |
| Transport | TCP | Segment | Ports |
| Link | Ethernet | Frame | MAC-Adressen |

Die Daten Anwendungsschicht werden auf der Transportschicht in ein Segment verpackt. Dieses wird in der Internetschicht in ein Paket verpackt; und dieses schlussendlich in der Link-Schicht in ein Frame.

![Datenkapselung im TCP/IP-Modell](/assets/segment-packet-frame.jpg)

---

## Webtechnologie: HTML, CSS und JS

![HTML_CSS_JS](/assets/html-css-js.png)

### HTML - *Hypertext Markup Language*

HTML gibt eine Struktur für die Webpageinhalte vor.
Die `index.html` ist in der Regel der zentrale Eiinstiegspunkt für jede Website - alle weiteren Inhalte (Bilder, Videos, CSS-Stylesheet, JS-Files, usw.) werden über diese verknüpft.

Die zentralen Bausteine von HTML sind die sogenannten **Tags**. Tags können mit Hilfe von **Attributen** erweitert werden. Attribute bestehen aus Schlüssel-Wert-Paaren (*key-value-pairs*). Der  HTML-Quelltext einer Webpage wird vom Browser und von verschiedenen Bots (Suchmaschienen-Bots - *Crawler*, KI-Bots, ...) gelesen und interpretiert.

![Aufbau eines HTML-Tags](/assets/html-tag)