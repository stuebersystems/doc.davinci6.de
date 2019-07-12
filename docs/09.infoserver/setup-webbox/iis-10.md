# DAVINCI WEBBOX und IIS 10

Dieses Kapitel beschreibt die Installation und Konfiguration der DAVINCI WEBBOX auf Ihrem Apache HTTP Server.

Die DAVINCI WEBBOX setzt folgende Installationen voraus:

* DAVINCI SERVER
* DAVINCI INFOSERVER

## Installation der DAVINCI WEBBOX

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite [davinci-webbox.stueber.de] in Ihrem Web-Browser.

2. Klicken Sie in unter `Getting started` auf `Download zip archive`. Ihr Web-Browser lädt Ihnen nun ein Zip-Archiv herunter.

3. Enpacken Sie das Zip-Archiv und kopieren Sie alle Dateien in den Ordner Ihrer Webseite. Standardmäßig ist dies der Ordner `C:\inetpub\wwwroot`.

## Konfiguration des IIS-Web-Servers

### HTTP-Antwortheader

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Alle Apps > Windows-Verwaltungsprogramme > Internetinformationsdienste (IIS)-Manager`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DAVINCI WEBBOX installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `HTTP-Antwortheader`. Die Ansicht "HTTP-Antwortheader" öffnet sich.

4. Klicken Sie nun auf `Hinzufügen` auf der rechten Seite unter "Aktionen". Ein Dialogfenster öffnet sich.

5. Tragen Sie in diesem Dialogfenster unter "Name" den Wert `Access-Control-Allow-Origin` und unter "Wert" `*` ein. Bestätigen Sie mit `OK`.

![ "HTTP-Antwortheader hinzufügen"](../../images/webbox-http-header.png)

Nach dem gleichen Muster fügen Sie bitte auch die folgenden HTTP-Antwortheader hinzu:

Name|Wert
---|--
 X-XSS-Protection| 1; mode=block
 X-Content-Type-Options|nosniff
 X-Frame-Options| SAMEORIGIN

### MIME-Typen

Überprüfen Sie jetzt bitte noch, ob die MIME-Typen für `json`, `woff` und `svg` registriert sind:

1. Markieren Sie dafür wieder in der linken Navigation Ihre Webseite, in der Sie die DAVINCI WEBBOX installieren wollen.

2. Auf der rechten Seite doppelklicken Sie auf das Symbol `MIME-Typ`. Die Ansicht "MIME-Typ" öffnet sich.

3. Überprüfen Sie, ob Sie Einträge für `json`, `woff` und `svg` finden. 

Sollten Sie nicht alle drei Einträge finden, müssen Sie die jeweils fehlenden noch hinzufügen:

1. Klicken Sie dazu auf der rechten Seite unter "Aktionen" auf Hinzufügen. Ein Dialgofenster öffnet sich.

2. Für `json` tragen Sie unter Dateinamenerweiterung `json` und unter MIME-Typ `application/json` ein.
  
![ "MIME-Typ für json registrieren"](../../images/webbox-register-json.png)

3. Wiederholen Sie diese kation für die foglednen Dateinamenerweiterung. Für `svg` tragen Sie unter Dateinamenerweiterung `svg` und unter MIME-Typ `image/svg+xml` ein.
  
![ "MIME-Typ für svg registrieren"](../../images/webbox-register-svg.png)

4. Für `woff` tragen Sie unter Dateinamenerweiterung `woff` und unter MIME-Typ `font/x-woff` ein.
  
![ "MIME-Typ für woff registrieren"](../../images/webbox-register-woff.png)

## Die DAVINCI-WEBBOX testen

Um sicherzugehen, dass alles korrekt installiert und konfiguriert ist, empfiehlt sich ein kleiner Test mit der DAVINCI-WEBBOX:

Öffnen Sie Ihren Web-Browser auf demselben Computer, auf dem Sie gerade eben die DAVINCI-WEBBOX installiert haben und tippen Sie folgende URL ein:

```txt
http://localhost/davinci-timetable.html
```

Diese URL sollte Ihnen im Idealfall eine Stundenplanansicht zurückliefern, die in etwa so aussieht:

![ "Ein Stundenplan in der DAVINCI-WEBBOX"](../../images/webbox-timetable.png)

Ein weiterer Test:

```txt
http://localhost/davinci-substitutions.html
```

Diese URL sollte Ihnen im Idealfall eine Vertretungsplanansicht zurückliefern, die in etwa so aussieht:

![ "Eine Vertretungsplanliste in der DAVINCI-WEBBOX"](../../images/webbox-substitutions.png)

!!! info "Hinweis"

  Die DAVINCI-WEBBOX zeigt auch Inhalte aus erst in der Zukunft gültigen Plänen an. Zurückliegend werden die Daten der letzten beiden Wochen mit ausgegeben.

## Die DAVINCI-WEBBOX nutzen

Auf der Webseite [davinci-webbox.stueber.de] finden Sie eine Dokumentation aller Aufrufparameter sowie zahlreiche Beispiele für das Einbinden der DAVINCI-WEBBOX in Ihre Webseite.

[davinci-webbox.stueber.de]: http://davinci-webbox.stueber.de

## Die DAVINCI-WEBBOX aktualisieren

Die aktualisierten Dateien der DAVINCI WEBBOX stellen wir auf der Webseite [davinci-webbox.stueber.de](http://davinci-webbox.stueber.de/) zum Download zur Verfügung. Bitte laden Sie sich das hinterlegte Ziparchiv herunter und legen es auf dem Rechner ab, auf dem Ihr Webserver läuft. Entpacken Sie die Dateien und legen sie an der entsprechenden Stelle ab, standardmäßig wäre der Pfad `C:\inetpub\wwwroot`.
