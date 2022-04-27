# Einbinden von Gebäudeplänen

SIe können mit der Nutzung der Webbox interaktive SVG Gebäudepläne in Ihre Website einbinden. Voraussetzung für die Einbindung der Gebäudpläne ist eine funktionierende Webbox.

Sie haben von uns eine Reihe von Dateien zur Darstellung des Gebäudeplanes erhalten. Dies sind folgende:

* Gebäudeplan welcher als SVG Datei erstellt wurde `floorplan.svg`
* Index Datei des Gebäudeplanes `floorplan.json`
* (optional) eine Metadaten Datei des Gebäudeplanes erstellen `floorplan.csv`

Bitte legen Sie diese Dateien im Webbox Ordner auf Ihrem Internet Information Server ab. Standardmäßig sollte das dieser sein `C:\inetpub\wwwroot`

Die DAVINCI WEBBOX-Anzeige wird von JSON-Daten und entsprechenden Aufrufparametern gesteuert. Die Parameteraufrufe sind vollständig entkoppelt – Sie geben Parameter an (.d.h. sie werden der Attributkollektion hinzugefügt), die WEBBOX verarbeitet die Parameter (d.h. nimmt sie aus der Kollektion). Alle Werte sind vom Typ string oder array oder strings oder object. Sie definieren ein Wert Array, indem Sie die Werte durch "|" voneinander trennen. Sie verweisen auf Objekte, indem Sie "." an den Parameternamen anfügen. 

Zur Anzeige der Gebäudepläne nutzen Sie bitte folgenden URL - Parametermeter:

`views=timetable|calendar|substitutions|floorplan` 

Beispiel: https://davinci.local/davinci-timetable.html?views=timetable|calendar|substitutions|floorplan

Weitere Ausführungen dazu finden Sie [hier](https://test.davinci-webbox.stueber.de/).

[Hier](https://test.davinci-webbox.stueber.de/) finden Sie Beispiele anderer Gebäudepläne, die mit verbundenen URL Parameter arbeiten.