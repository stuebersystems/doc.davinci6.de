# Gebäudepläne

Sie können die Raumbelegungsdaten aus DAVINCI aufmerksamkeitswirksam in digitalen Gebäudeplänen verwenden. Der Gebäudeplan kann über über DAVINCI MOBILE auf Tablets oder per DAVINCI WEBBOX auf Ihrer Webseite angezeigt werden. Ein Beispiel finden Sie auf der [Webseite für Gebäudepläne](http://davinci.stueber.de/floorplan.php).

## Gebäudepläne anfertigen lassen

Sie können uns beauftragen für Ihre Gebäude individuelle Pläne anzufertigen.

So funktioniert's:<br/>Sie senden uns Ihren Gebäudeplan mit den Gebäudeebenen-Layouts und eindeutiger Benennung der Räume als PDF-Dokument oder bereits als SVG-Datei. Wir erstellen auf dieser Grundlage ein Angebot für Sie.

Nach Beauftragung fertigen wir für jede Ebene eine SVG-Datei an. Die Räume in der SVG-Datei werden dann mit einer ID versehen. Die Räume sind über die jeweilige ID per JavaScript identifizierbar und können von einer Applikation mit Informationen gefüllt werden.

Wenn Sie möchten, helfen wir Ihnen Ihren SVG-Flurplan in Ihre Anwendung einzubetten.

## Einbinden von Gebäudeplänen

Sie können mit der Nutzung der Webbox interaktive SVG Gebäudepläne in Ihre Website einbinden. Voraussetzung für die Einbindung der Gebäudpläne ist eine funktionierende Webbox.

Sie haben von uns eine Reihe von Dateien zur Darstellung des Gebäudeplanes erhalten. Dies sind folgende:

* Gebäudeplan welcher als SVG Datei erstellt wurde `floorplan.svg`
* Index Datei des Gebäudeplanes `floorplan.json`
* (optional) eine Metadaten Datei des Gebäudeplanes erstellen `floorplan.csv`

Bitte legen Sie diese Dateien im Webbox Ordner auf Ihrem Internet Information Server ab. Standardmäßig sollte das dieser sein `C:\inetpub\wwwroot`

Die DAVINCI WEBBOX-Anzeige wird von JSON-Daten und entsprechenden Aufrufparametern gesteuert. Die Parameteraufrufe sind vollständig entkoppelt – Sie geben Parameter an (.d.h. sie werden der Attributkollektion hinzugefügt), die WEBBOX verarbeitet die Parameter (d.h. nimmt sie aus der Kollektion). Alle Werte sind vom Typ string oder array oder strings oder object. Sie definieren ein Wert Array, indem Sie die Werte durch "|" voneinander trennen. Sie verweisen auf Objekte, indem Sie "." an den Parameternamen anfügen. 

Zur Anzeige der Gebäudepläne nutzen Sie bitte folgenden URL - Parametermeter:

`views=timetable|calendar|substitutions|floorplan` 

Beispiel: [https://davinci.local/davinci-timetable.html?views=timetable|calendar|substitutions|floorplan](https://davinci.local/davinci-timetable.html?views=timetable|calendar|substitutions|floorplan)

Weitere Ausführungen dazu finden Sie unter [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/).

Unter [[https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/) finden Sie Beispiele anderer Gebäudepläne, die mit verbundenen URL-Parameter arbeiten.

## Zwischen Ebenen wechseln

Gebäudepläne können mehrere Ebenen beinhalten. Um zwischen den Ebenen zu wechseln, gibt es mehrere Möglichkeiten.

> Es wird in den nachstehenden Beispielen mit Parametern gearbeitet, eine vollständige Auflistung der zur Verfügung stehenden Parameter finden Sie hier: [https://davinci-webbox.stueber.de/](https://davinci-webbox.stueber.de/)

### Variante 1

`Ihr Server/davinci-timetable.html?views=timetable|calendar|substitutions|floorplan#`

Im oben stehenden Link wird die Vorlage `davinci-timetable.html` in Kombination mit dem Parameter `views=timetable|calendar|substitutions|floorplan#` verwendet. Damit wird im unteren Bereich ein Symbol zum Aufrufen des Gebäudeplans (zusätzlich zu den Symbolen für Stundenplan, Kalender und Vertretungsplan) gezeigt.

![Symbol zum Aufrufen der Ansicht Gebäudepläne](/assets/images/gebaeudeplaene/01.png)

Zwischen den Ebenen wechseln Sie über die Auswahl am rechten oberen Fensterrand.

![Wechseln zwischen den Ebenen](/assets/images/gebaeudeplaene/02.png)

### Variante 2

Alternativ können Sie auch, wenn Sie keine Stundenpläne oder Vertretungspläne anzeigen möchten, die Vorlage `DAVINCI-floorplan.html` verwenden.
Hier können Sie per Parameter gezielt eine bestimmte Ebene aufzurufen, beispielsweise um auf dem Bildschirm auf Etage 1 genau den Plan der Etage zu zeigen. 

Beispiellink: <br/>`Ihr Server/davinci-floorplan.html?floor=1`

Hier wird die Vorlage DAVINCI-floorplan.html verwendet und es wird gezielt die Ebene/Etage 1 gezeigt.
Die Ebenen werden von Ebene 0 aus aufsteigend nummeriert, dass Erdgeschoss wäre die `Floor=0`, das erste Geschoss wäre `Floor=1` usw. 

### Variante 3

Sie verwenden die DAVINCI-floorplan.html und möchten Ebenen per Klick auswählen können.

Beispiellink: <br/>`Ihr Server/davinci-floorplan.html?showFloorSelector=true`

Obenstehender Link ruft die Vorlage `DAVINCI-floorplan.html` auf und aktiviert die Ebenenauswahl über den Parameter `showFloorSelector=true`.
Die Ebenenauswahl wird im unteren Bereich der Seite gezeigt.

![Wechseln zwischen den Ebenen](/assets/images/gebaeudeplaene/03.png)