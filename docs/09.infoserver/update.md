# DAVINCI INFOSERVER und DAVINCI WEBBOX aktualisieren

Wenn Sie in Ihrem Schulnetzwerk die DAVINCI-Module aktualisieren möchten, sind folgende Module zu aktualisieren.

!!! info "Hinweis"

    Das Aktualisieren von DAVINCI und DAVINCI LOOK wird nur zur Vollständigkeit aufgezählt und wird hier nicht weiter beschrieben.

Auf welchen Rechnern|Was muss aktualisiert werden
---|---
 Auf den Clients| [DAVINCI](https://download.stueber.de/bin/de/davinci/v6/davinci6.msi) <br/>[DAVINCI LOOK](https://download.stueber.de/bin/de/davinci/v6/davinci6look.msi)
 Auf dem oder den Serverrechner(n) <br/>(ggfs. laufen der DAVINCI INFOSERVER und der DAVINCI Server auf getrennten Rechnern) |[DAVINCI Server](https://download.stueber.de/bin/de/davinci/v6/davinci6server.msi)<br/>[DAVINCI INFOSERVER](https://download.stueber.de/bin/de/davinci/v6/davinci6infoserver.msi)<br/>[WEBBOX Dateien](https://davinci-webbox.stueber.de/)
  
## Den DAVINCI Server aktualisieren

Möchten Sie eine neue Version des DAVINCI Servers einspielen, gehen Sie wie folgt vor:

1. Stellen Sie sicher, dass die DAVINCI Benutzer abgemeldet sind.
2. Führen Sie die Installation mit einem aktuelleren [Installationspaket](https://download.stueber.de/bin/de/davinci/v6/davinci6server.msi) des DAVINCI Servers aus. Das Setup ersetzt dabei automatisch Ihre bisherigen DAVINCI Server Dateien.

## Den DAVINCI INFOSERVER aktualisieren

Möchten Sie eine neue Version des DAVINCI INFOSERVER einspielen, gehen Sie wie folgt vor:

1. Stoppen Sie Ihren Web-Server.
2. Führen Sie die Installation mit einem aktuelleren [Installationspaket](https://download.stueber.de/bin/de/davinci/v6/davinci6infoserver.msi) des DAVINCI INFOSERVERS aus. Das Setup ersetzt dabei automatisch Ihre bisherigen DAVINCI INFOSERVER Dateien.
3. Starten Sie den Web-Server neu.

## Die DAVINCI WEBBOX aktualisieren

Möchten Sie eine neue Version der DAVINCI WEBBOX einspielen, gehen Sie wie folgt vor:

1. Prüfen Sie, welche Version Sie aktuell einsetzen. Rufen Sie Ihre WEBBOX-Seite auf und schauen unten rechts unter dem i-Symbol.

Klicken Sie auf das i-Symbol!

[![Klicken Sie auf das i-Symbol!][1]][1] 

Die eingesetzte Version wird gezeigt

[![Beschriftung][2]][2]

Ob eine neuere Ausgabe der WEBBOX-Dateien vorliegt, können Sie unter [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/)prüfen.

Laden Sie gegebenenfalls das zip-Archiv mit den WEBBOX-Dateien auf den Rechner auf dem Ihr Webserver läuft und entpacken die Dateien in das entsprechende Verzeichnis. Die bereits vorhandenen Dateien können vorher gelöscht oder mit dem Inhalt des Zip-Archivs überschrieben werden.

Webserver|Standardverzeichnis für die WEBBOX-Dateien
---|---
Apache|`c:\xampp\htdocs`
InternetInformationServer|`C:\inetpub\wwwroot`

!!! warning "Wichtig"

    Starten Sie bitte abschließend den Web-Server und Ihren DAVINCI-Server neu!
    
[1]:/assets/images/is/webbox01.png
[2]:/assets/images/is/webbox02.png
