# DaVinci WebBox und Apache

Dieses Kapitel beschreibt die Installation und Konfiguration der DaVinci WebBox auf Ihrem Apache HTTP Server.

Die DaVinci WebBox setzt folgende Installationen voraus:

* DaVinci Server
* DaVinci InfoServer

## Installation

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite [davinci-webbox.stueber.de] in Ihrem Web-Browser.

2. Klicken Sie in unter `Getting started` auf `Download zip archive`. Ihr Web-Browser lädt Ihnen nun ein Zip-Archiv herunter.

3. Enpacken Sie das Zip-Archiv und kopieren Sie alle Dateien in den Ordner Ihrer Webseite. Standardmäßig ist dies der Ordner `c:\xampp\htdocs`. Im Zweifelsfall schauen Sie in der Apache-Konfigurationsdatei `httpd.conf` unter `DocumentRoot` nach.

## Konfiguration des Apache HTTP Servers {# Konfiguration des Apache HTTP Servers}

Standardmäßig müssen Sie unter Apache keine weitere Konfiguration für die DaVinci WebBox durchführen.

Im Gegensatz zum IIS sind die MIME-Typen für `json`, `woff`  und `svg` bereits registriert. Möchten Sie dies dennoch überprüfen, müssen Sie die folgende Datei in einem Texteditor öffnen:

```txt
c:\xampp\apache\conf\mime.types
```

## Testen

Um sicherzugehen, dass alles korrekt installiert und konfiguriert ist, empfiehlt sich ein kleiner Test mit der DaVinci-WebBox:

Öffnen Sie Ihren Web-Browser auf demselben Computer, auf dem Sie gerade eben die DaVinci-WebBox installiert haben und tippen Sie folgende URL ein:

```txt
http://localhost/davinci-timetable.html
```

Diese URL sollte Ihnen im Idealfall eine Stundenplanansicht zurückliefern, die in etwa so aussieht:

[!["Ein Stundenplan in der DaVinci-WebBox"][1]][1]

Ein weiterer Test:

```txt
http://localhost/davinci-substitutions.html
```

Diese URL sollte Ihnen im Idealfall eine Vertretungsplanansicht zurückliefern, die in etwa so aussieht:

[![ "Eine Vertretungsplanliste in der DaVinci-WebBox"][2]][2]


!!! info "Hinweis"

    Die DaVinci-WebBox zeigt auch Inhalte aus erst in der Zukunft gültigen Plänen an. Zurückliegend werden die Daten der letzten beiden Wochen mit ausgegeben.

## Die DaVinci-WebBox nutzen

Auf der Webseite [davinci-webbox.stueber.de] finden Sie eine Dokumentation aller Aufrufparameter sowie zahlreiche Beispiele für das Einbinden der DaVinci-WebBox in Ihre Webseite.

[davinci-webbox.stueber.de]: http://davinci-webbox.stueber.de

[1]:/assets/images/is/webbox-timetable.png
[2]:/assets/images/is/webbox-substitutions.png