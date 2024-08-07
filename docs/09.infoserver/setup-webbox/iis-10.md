# DaVinci WebBox und IIS 10

Dieses Kapitel beschreibt die Installation und Konfiguration der DaVinci WebBox auf Ihrem IIS-Web-Server.

Die DaVinci WebBox setzt folgende Installationen voraus:

* DaVinci Server
* DaVinci InfoServer

## Installation der DaVinci WebBox

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite [davinci-webbox.stueber.de] in Ihrem Web-Browser.

2. Klicken Sie in unter `Getting started` auf `Download zip archive`. Ihr Web-Browser lädt Ihnen nun ein Zip-Archiv herunter.

3. Enpacken Sie das Zip-Archiv und kopieren Sie alle Dateien in den Ordner Ihrer Webseite. Standardmäßig ist dies der Ordner `C:\inetpub\wwwroot`.

## Konfiguration des IIS-Web-Servers

### HTTP-Antwortheader

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Alle Apps > Windows-Verwaltungsprogramme > Internetinformationsdienste (IIS)-Manager`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DaVinci WebBox installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `HTTP-Antwortheader`. Die Ansicht "HTTP-Antwortheader" öffnet sich.

4. Klicken Sie nun auf `Hinzufügen` auf der rechten Seite unter "Aktionen". Ein Dialogfenster öffnet sich.

5. Tragen Sie in diesem Dialogfenster unter "Name" den Wert `Access-Control-Allow-Origin` und unter "Wert" `*` ein. Bestätigen Sie mit `OK`.

[!["HTTP-Antwortheader hinzufügen"][1]][1] 

Nach dem gleichen Muster fügen Sie bitte auch die folgenden HTTP-Antwortheader hinzu:

Name|Wert
---|--
 X-XSS-Protection| 1; mode=block
 X-Content-Type-Options|nosniff
 X-Frame-Options| SAMEORIGIN

### MIME-Typen

Überprüfen Sie jetzt bitte noch, ob die MIME-Typen für `json`, `woff` und `svg` registriert sind:

1. Markieren Sie dafür wieder in der linken Navigation Ihre Webseite, in der Sie die DaVinci WebBox installieren wollen.

2. Auf der rechten Seite doppelklicken Sie auf das Symbol `MIME-Typ`. Die Ansicht "MIME-Typ" öffnet sich.

3. Überprüfen Sie, ob Sie Einträge für `json`, `woff` und `svg` finden. 

Sollten Sie nicht alle drei Einträge finden, müssen Sie die jeweils fehlenden noch hinzufügen:

1. Klicken Sie dazu auf der rechten Seite unter "Aktionen" auf Hinzufügen. Ein Dialgofenster öffnet sich.

2. Für `json` tragen Sie unter Dateinamenerweiterung `json` und unter MIME-Typ `application/json` ein.

[![Beschriftung][2]][2] 

3. Wiederholen Sie diese kation für die foglednen Dateinamenerweiterung. Für `svg` tragen Sie unter Dateinamenerweiterung `svg` und unter MIME-Typ `image/svg+xml` ein.

[!["MIME-Typ für svg registrieren"][3]][3] 

4. Für `woff` tragen Sie unter Dateinamenerweiterung `woff` und unter MIME-Typ `font/x-woff` ein.

[![Beschriftung][4]][4] 


## Die DaVinci-WebBox testen

Um sicherzugehen, dass alles korrekt installiert und konfiguriert ist, empfiehlt sich ein kleiner Test mit der DaVinci-WebBox:

Öffnen Sie Ihren Web-Browser auf demselben Computer, auf dem Sie gerade eben die DaVinci-WebBox installiert haben und tippen Sie folgende URL ein:

```txt
http://localhost/davinci-timetable.html
```

Diese URL sollte Ihnen im Idealfall eine Stundenplanansicht zurückliefern, die in etwa so aussieht:

[![Beschriftung][5]][5] 

Ein weiterer Test:

```txt
http://localhost/davinci-substitutions.html
```

Diese URL sollte Ihnen im Idealfall eine Vertretungsplanansicht zurückliefern, die in etwa so aussieht:

![ "Eine Vertretungsplanliste in der DaVinci-WebBox"](/assets/images/webbox-substitutions.png)

!!! info "Hinweis"

  Die DaVinci-WebBox zeigt auch Inhalte aus erst in der Zukunft gültigen Plänen an. Zurückliegend werden die Daten der letzten beiden Wochen mit ausgegeben.

## Die DaVinci-WebBox nutzen

Auf der Webseite [davinci-webbox.stueber.de] finden Sie eine Dokumentation aller Aufrufparameter sowie zahlreiche Beispiele für das Einbinden der DaVinci-WebBox in Ihre Webseite.

[davinci-webbox.stueber.de]: http://davinci-webbox.stueber.de

## Die DaVinci-WebBox aktualisieren

Die aktualisierten Dateien der DaVinci WebBox stellen wir auf der Webseite [davinci-webbox.stueber.de](http://davinci-webbox.stueber.de/) zum Download zur Verfügung. Bitte laden Sie sich das hinterlegte Ziparchiv herunter und legen es auf dem Rechner ab, auf dem Ihr Webserver läuft. Entpacken Sie die Dateien und legen sie an der entsprechenden Stelle ab, standardmäßig wäre der Pfad `C:\inetpub\wwwroot`.

[1]:/assets/images/is/webbox-http-header.png
[2]:/assets/images/is/webbox-register-json.png
[3]:/assets/images/is/webbox-register-svg.png
[4]:/assets/images/is/webbox-register-woff.png
[5]:/assets/images/is/webbox-timetable.png