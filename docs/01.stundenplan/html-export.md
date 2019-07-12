# Export statischer HTML-Dateien

DAVINCI bietet zwei alternative Wege an, um HTML-Seiten zu erzeugen:

* **Statische HTML-Seiten** durch den HTML-Export über das gleichnamige Dialogfenster in daVinci. Dabei werden eine Reihe von Dateien für die angefragten Stundenpläne bzw. Vertretungspläne erzeugt, die Sie auf Ihre Website hochladen können. Diese Seiten können von [CONFIRE SHOWTIME](https://showtime.stueber.de/) und anderen Anzeigeprogrammen für Info-Bildschirme (Digitales Schwarzes Brett) an Ihrer Schule verwendet werden.
Hierfür benötigen Sie eine Lizenz für DAVINCI INTERNET.

* **Dynamische HTML-Seiten** über den [DAVINCI INFOSERVER](https://davinci.stueber.de/davinci-infoserver.php). Der Webbrowser erhält dabei mittels des daVinci INFOSERVER vom DAVINCI ENTERPRISE Server die jeweils angeforderte aktuelle Seite, das ständige Erzeugen und Hochladen von Dateien z.B. bei Planänderungen entfällt. Weitere Informationen finden Sie in der Dokumentation zum [DAVINCI INFOSERVER](https://doc.davinci6.stueber.de/09.infoserver/setup-infoserver/).
Hierfür benötigen Sie eine Lizenz für DAVINCI INFOSERVER.

!!! info "Hinweis"

    Für den HTML-Export ist eine Lizenz von DAVINCI INTERNET bzw. DAVINCI INFOSERVER erforderlich. 
    Die nachstehenden Kapitel beziehen sich auf das Erstellen **statischer HTML-Seiten**.  Informationen zum Erstellen **dynamischer HTML-Seiten** finden Sie in der Dokumentation zum [DAVINCI INFOSERVER](https://doc.davinci6.stueber.de/09.infoserver/setup-infoserver/).

Sie können Pläne mit und ohne Vertretungsplaninformationen sowie Vertretungspläne als HTML-Seiten exportieren und so auf Ihrer Website publizieren. Rufen Sie dazu das HTML-Export-Fenster auf, welches im Wesentlichen die gleichen Einstellungen wie das Drucken-Fenster (siehe [Publikation per Ausdruck](/davinci-stundenplan/9-stundenplane-drucken/publikation-per-ausdruck.md) aufweist, weshalb wir im vorliegenden Kapitel nur auf die Unterschiede eingehen werden.

Klicken Sie auf `Publizieren > HTML-Pläne exportieren` um das Dialogfenster `HTML-Export`-zu öffnen.

![Publizieren > HTML-Pläne exportieren](/assets/images/HTML-Pläne.Drucken.png)

![Dialogfenster "HTML-Export"](/assets/images/Dialogfenster.HTML-Pläne.Drucken.png)

## HTML-Ordner festlegen

Bevor Sie mit dem HTML-Export beginnen, müssen Sie im Fenster `Extras > Optionen` in der Ansicht `Internet` den Ordner für alle HTML-Exporte eingeben. Beim Exportieren von HTML-Plänen werden diese in diesem Ordner abgelegt und können von dort auf Ihre Website kopiert werden.

!["HTML Vorlagen Ordner“ und „HTML Export Ordner“ im Optionen-Fenster festlegen](/assets/images/HTML-Pläne.Ordner.png)

Der „HTML Vorlagen Ordner“ enthält die für den HTML-Export wichtigen Unterordner:

* CSS
* HTML
* JS
* Sandbox

Diese Ordner werden in den folgenden Kapiteln erläutert.

## HTML-Exportformate

![Klassen-Einzelplan HTML-Exportformat](/assets/images/HTML.Export01.png)

Wie auch beim Drucken richtet sich das Aussehen der gedruckten Pläne nach dem im HTML-Export-Fenster unter „HTML-Exportformat“ eingestellten Exportformat. Es wird bei jedem Export eine Indexdatei „index.html“ und eine entsprechende Anzahl von Plandateien erzeugt. Die HTML-Exportvorlage in der Datei daVinci.hfm verweist auf eine HTML-Seitenvorlagedatei für die Inhaltsseiten und eine Seitenvorlagedatei für die Indexseite.

Einstellung|Anmerkung
-|-
Index |* Mit `Index gruppiert` können Sie angeben, ob der Inhalt ggf. gruppiert angezeigt werden soll, d.h. nach dem ersten Buchstaben (bei Kürzel- oder Namenslisten, bei Klassen wird nach Klas-senstufe und erstem Buchstaben gruppiert) bzw. nach Monaten (bei Tagesvertretungen).
Index HTML-Vorlage| Wählen Sie eine der mitgelieferten Vorlagen aus.
Allgemeine HTML-Vorlage|Wählen Sie eine der mitgelieferten Vorlagen aus.
Sandbox-Ordner kopieren|Wenn diese Option markiert ist, wird der gesamte Inhalt des Sandbox-Ordners in den Export-Unterordner kopiert. <br/>Der Sandbox-Ordner ist ein Unterordner des HTML Vorlagen Ordners und enthält die Layout-Informationen für die HTML-Dateien, z.B. Bilddateien für das Logo und die Schaltflächen.
Export-Unterordnerinhalt zuvor löschen|Vor dem Neuanlegen der Exportdateien wird das eingestellte Verzeichnis geleert.
Dateinamen Präfix|Optional kann ein Präfix gewählt werden
Diesen Export-Unterordner verwenden| Wenn Sie diese Option markieren und im Eingabefeld einen Unterordner angeben, werden die Ausgaben mit diesem Exportformat in diesem Unterordner innerhalb des HTML-Export-Hauptordners angelegt.<br/> Den HTML-Export-Hauptordner können Sie eingeben, wenn Sie auf die Schaltfläche `Export-Hauptordner auswählen...` klicken <br/>(siehe dazu auch [HTML-Ordner festlegen](/davinci-stundenplan/html-export/html-ordner-festlegen.md)).
Schaltfläche Home|Hier können Sie die Schaltflächen in den HTML-Seiten benennen.

## HTML-, JavaScript- und CSS-Vorlagen

![Der daVinci HTML-Präprozessor](/assets/images/Grafik.png)

Der daVinci HTML Präprozessor erzeugt aus

* den DAVINCI Plandaten
* einer HTML-Seitenvorlage Datei (das ist die im HTML-Exportformat angegebene HTMLSeitenvorlagedatei aus dem Ordner „HTML“, die Standardvorlagedatei heißt „davinci.
content.main.html“)
* einer CSS-Layoutvorlage Datei (das ist die im HTML-Exportformat angegebene CSSVorlagedatei aus dem Ordner „CSS“, die Standardvorlagedatei heißt „davinci.
content.main.css“)
* den JavaScript-Dateien aus dem Ordner „JS“ die HTML-Dateien, die in dem im HTML-Exportformat angegebenen Export-Unterordner abgelegt werden. DAVINCI erzeugt HTML5 und CSS3 kompatible HTML-Seiten. Im Export-Unterordner werden folgende Dateien bzw. Ordner angelegt:

* Die Indexdatei index.html, die den Index für die nachfolgenden HTML-Dateien enthält
* Die HTML-Dateien für die Pläne bzw. Vertretungspläne
* Den Unterordner „Sandbox“, der die Layout-Dateien enthält, insbesondere die CSS-Datei, die Grafikdateien sowie ggf. JavaScript-Dateien.

|Was ist wofür zuständig?|
|-|
|Die **HTML-Seitenvorlage-Datei** gibt den Rahmen für alle von DAVINCI erzeugten HTML-Seiten vor. Sie enthält die Inhaltsstruktur der HTML-Datei, aber keine Layoutinformationen.|
|Die** CSS-Layoutvorlage-Dateien** enthalten alle Layoutinformationen für die Anzeige der HTML-Dateien in einem Webbrowser, aber keine Inhalte.|
|Die **JavaScript-Dateien** enthalten JavaScript Code mit speziellen Anzeige-Effekten.|
|Der **DAVINCI Ordner SANDBOX** wird beim Erzeugen der Ausgabedateien von daVinci ebenfalls mit Inhalt in den Export-Unterordner kopiert.<br/>Er dient sozusagen als Transportordner für alle weiteren Dateien, die für das Layout benötigt werden, z.B. die Logo-Bilddatei.<br/>Insbesondere wird die CSS-Datei in den Sandbox-Ordner kopiert.

!!! info "Hinweis"

    **CSS** steht für „Cascading Style Sheets“ (engl. für stufenförmige geschachtelte Layout Vorlagen), womit eine Beschreibungssprache für Stilvorlagen (engl. stylesheets) für strukturierte Dokumente gemeint ist. CSS-Dateien werden in der Regel benutzt, um das Layout von HTML-Dokumenten zu bestimmen. Weiterführende Informationen dazu finden Sie unter dem Stichwort „CSS“ im Internet.

Sowohl die HTML-Seitenvorlage-Datei wie auch die CSS-Layoutvorlage Datei kann DAVINCI-spezifische Platzhalter enthalten, die vom daVinci HTML-Präprozessor beim Erzeugen der Ausgabedateien entsprechend mit DAVINCI-Inhalten ersetzt werden. Ersetzungen werden nur in Dateien mit dem Präfix „davinci.“ durchgeführt. Z.B. wird der Platzhalter %HOMEPAGE% durch den Link zu Ihrer Homepage ersetzt. Die möglichen daVinci Platzhalter sind in den beiden nachfolgenden Kapiteln beschrieben.

!!! info "Hinweis"

    Sie müssen die Layout Informationen im Sandbox-Ordner und auch die CSS-Datei nicht bei jedem HTML-Export immer wieder mitkopieren, da sie sich in der Regel nicht ändern. Demarkieren Sie in diesem Fall die Optionen `Sandbox-Ordner kopieren`. Der Sandbox-Ordner kann auch in einem anderen öffentlichen Ordner auf Ihrem Webserver liegen. In diesem Fall müssen Sie die korrekten URL-Pfade in der HTML-Datei ersetzen.

## Die HTML-Seitenvorlage-Datei

!!! info "Hinweis"

    Alle in DAVINCI-Layouts (HTML- und CSS-Dateien) sind für unterschiedliche Bildschirmauflösungen geeignet und können insbesondere auch für iPad/Tablets und iPhone/SmartPhone verwendet werden.

Die HTML-Seitenvorlagedatei gibt den Rahmen für alle von DAVINCI erzeugten HTML-Seiten vor, also die Index-Datei und alle weiteren HTML-Dateien. Sie enthält die Inhaltsstruktur der HTML-Datei und ggf. Platzhalter, aber keine Layout Informationen. Die Standard Seitenvorlagedatei heißt **davinci.content.main.html**. Den einzige Platzhalter der zwingend in der HTML-Vorlagedatei verwendet werden muss, ist der Platzhalter %DAVINCICONTENT%, der von DAVINCI durch den eigentlichen Inhalt, d.h. den Index, den Plan oder die Vertretungsliste ersetzt wird. Die meisten Platzhalter werden durch die Angaben unter `Meine Daten` im Optionen-Dialogfenster ersetzt.

### Platzhalter für HTML-Seitenvorlage Datei

Platzhalter | Beschreibung | Quelle
-|-|-
%HOMEPAGE% | URL zu Ihrer Homepage, z.B. http://www.stueber.de |Eingabefeld „Homepage“ in `Extras > Optionen > Meine Daten`
%AUTHOR% | Autor | Eingabefelder `Allgemein > Name` und `Allgemein > Stadt` in `Extras > Optionen > Meine Daten`
%CREATOR% | Programmname | Von DAVINCI vorgegeben, nicht eingebbar
%SITENAME1% | Name Ihrer Institution | Eingabefelder `Allgemein > Name` in `Extras > Optionen > Meine Daten`
%SITENAME2% | Name Ihrer Institution | Eingabefelder `Allgemein > Name` in `Extras > Optionen > Meine Daten`
%SITENAME3% | Name Ihrer Institution | Eingabefelder `Allgemein > Name` in `Extras > Optionen > Meine Daten`
%SITECITY% | Ort Ihrer Institution | Eingabefeld `Allgemein > Stadt` in `Extras > Optionen > Meine Daten`
%SITECODE% | Postleitzahl Ihrer Institution | Eingabefeld `Allgemein > Postleitzahl` in `Extras > Optionen > Meine Daten`
%SITESTREET% | Straße Ihrer Institution | Eingabefelder `Allgemein > Straße` in `Extras > Optionen > Meine Daten`
%TIME% | Ausgabeuhrzeit | Wird von DAVINCI automatisch erzeugt
%NOW<format>% | Ausgabe-Datum-/Zeitangabe | Wird von DAVINCI automatisch erzeugt.<format> beschreibt das Ausgabeformat der Zeitangabe z.B. in der Form „dd.mm.yyyy hh:mm“ für „12.04.2014 11:55“
%DAVINCICONTENT% | DAVINCI HTML-Plan-/Vertretungsplaninhalt | Wird von DAVINCI automatisch erzeugt
%PREV% | URL zur vorherigen Datei | Wird von DAVINCI automatisch erzeugt
%NEXT% | URL zur nächsten Datei | Wird von DAVINCI automatisch erzeugt
%INDEX% | URL zur Indexdatei | Wird von DAVINCI automatisch erzeugen

### HTML-Vorlagedateien

Folgende HTML-Vorlagedateien werden durch die Installation mitgeliefert:

HTML-Vorlage | Bemerkung
-|-
davinci.index.main.html | Hauptvorlage für die Indexseite, CSS-Dateien werden von der Website www.stueber.de dazugelinkt.
davinci.index.local.html | Wie die Hauptvorlage für Indexseite, nur dass die CSS-Dateien lokal aus dem Ordner „Sandbox“ dazugelinkt werden.
davinci.content.main.html | Hauptvorlage für Inhaltsseiten, CSS-Dateien werden von der Website www.stueber.de dazugelinkt.
davinci.content.local.html | Wie die Hauptvorlage für Inhaltsseiten, nur dass die CSS-Dateien lokal aus dem Ordner „Sandbox“ dazugelinkt werden.
davinci.content.minimal.html | Wie die Hauptvorlage für Inhaltsseiten, aber ohne Kopf- und Fußzeile.
davinci.showtime.subst.main.html | Vorlage für automatisch umblätternde HTML-Vertretungslisten, insbesondere für SHOWTIME Systeme.
davinci.showtime.subst.local.html | Wie die Hauptvorlage für automatisch umblätternde HTML-Vertretungslisten (insbesondere für SHOWTIME Systeme?, nur dass die CSS-Dateien lokal aus dem Ordner „Sandbox“ dazugelinkt werden.

## Die CSS-Layoutvorlage

!!! info "Hinweis"

    Alle im Ordner „CSS“ standardmäßig mitgelieferten CSS Layout Vorlage-Dateien sind für alle gebräuchlichen Webbrowser geeignet.

Die CSS Layout Vorlage Datei enthält alle Layout Informationen (z.B. Schriftart, Schriftgröße, Farben) für die Anzeige der HTML-Dateien in einem Webbrowser.
Standardmäßig sind dies die Dateien davinci.index.main.css und davinci.content.main.css.

Wenn Sie Schriftart, Schriftgröße, Farben usw. verändern möchten, nehmen Sie CSS-Datei und verändern Sie die Attribute entsprechend.

## Die JavaScript-Layoutskripte

!!! info "Hinweis"

    Alle im Ordner „JS“ standardmäßig mitgelieferten JavaScript-Dateien werden beim Export in den Sandbox-Ordner kopiert.

Die JavaScript Dateien werden für diverse Effekte verwendet.

### Platzhalter für JavaScript Dateien

Platzhalter | Beschreibung | Quelle
-|-|-
%MAXROWSPERPAGE% | Maximale Anzahl von Zeilen in einer Tabelle, nach der die Liste weitergeschaltet wird | HTML-Format „Zeilen je Seite maximal, dann nächste Seite erzeugen“

## HTML-Export in eigene Website einbinden

Durch die Veränderung der HTML-Seitenvorlage Datei und der CSS-Layoutvorlage Datei können Sie die Gestaltung des DAVINCI HTML-Exports frei an die Stilvorgaben Ihrer Website anpassen. Ein gutes Nachschlagewerk für die Themen HTML5, CSS und JavaScript finden Sie z.B. auf der Website [http://www.w3schools.com](http://www.w3schools.com).

!!! info "Hinweis"

    Der DAVINCI INFOSERVER ermöglicht es dynamische Internetseiten zu erzeugen, d.h. die Seite wird erst zum Zeitpunkt des Aufrufs aus einem Webbrowser vom DAVINCI ENTERPRISE Server erzeugt und über den DAVINCI INFOSERVER an den Webbrowser zurückgeliefert. **Vorteil**: Das ständige Exportieren und Hochladen von HTML-Dateien nach jeder Änderung entfällt. Weitere Informationen dazu finden Sie unter [www.stueber.de](https://davinci.stueber.de/davinci-infoserver.php) oder in unserer [Dokumentation](/internet-publication/setup-infoserver/README.md).

## HTML-Export für Public Displays

Folgende Vorlagen werden spezielle für HTML-Exporte für Public Displays (z.B. [CONFIRE SHOWTIME](https://showtime.stueber.de/)) mitgeliefert:

HTML-Vorlage | Verwendung für
-|-
davinci.content.showtime.subst.html | Automatisch weiterblätternde HTML-Vertretungslisten auf Public Displays

Der DAVINCI INFOSERVER erlaubt es Ihnen, HTML-Seiten auf Ihrer Website zu publizieren, ohne expliziten HTML-Export. Weitere Informationen hierzu finden Sie unter [www.stueber.de](https://davinci.stueber.de/davinci-infoserver.php) oder in unserer [Dokumentation](/internet-publication/setup-infoserver/README.md).

## Vertretungslisten für Public Displays

Verwenden Sie die Seitenvorlage **davinci.content.showtime.subst.html** um Vertretungslisten auf Public Displays anzuzeigen. Die Vertretungslisten per JavaScript werden automatisch weitergeblättert, wenn die Anzahl der Zeilen die angegebene Maximalanzahl für eine Seite überschreitet. Diese Seitenvorlage Datei verweist auf die Dateien:

* davinci.listflip.js
* davinci.content.main.css

Erzeugen Sie einmal einen HTML-Export mit DAVINCI. Anschließend befinden sich veränderte Kopien dieser beiden Dateien im Ordner „Sandbox“:

* Die Datei davinci.content.main.css enthält jetzt die angegebene Schriftgröße und die Datei davinci.listflip.js die Anzahl der Zeilen je Seite. 
* Kopieren Sie beide Dateien in ein öffentliches Verzeichnis auf Ihrer Website und ändern Sie die URLs auf diese beiden Dateien in der Datei davinci.content.showtime.subst.html.

Variablen in der Datei davinci.listflip.js | Wert
-|-
showCount | %MAXROWSPERPAGE% ist der Platzhalter die Anzahl der Zeilen pro Seite. Die Variable %MAXROWSPERPAGE% wird bei einem HTML-Export über DAVINCI automatisch ersetzt.
newPageTime | Zeit bis zum Umblättern auf nächste Seite in 1/1000 Sekunden.

### Ausschnitt aus der Datei "davinci.listflip.js"

```js
// davinci.listflip.js -- STÜBER SYSTEMS
//
var reloadFlag = false;
$.fn.scrollUp=function(){
// set vars
var showCount = %MAXROWSPERPAGE%; // rows per page
var newPageTime = 10000; // next page time in 1/1000sec
var tableRows = $(this).children(); // this = tbody
var rowCount = tableRows.length;
// check rowCount
if (rowCount <= showCount) return;
// set startNo, endNo, pageNo, pageCount
var pageCount = Math.ceil(rowCount/showCount);
var startNo = 0, endNo = showCount, pageNo = 1;
// hide all rows, show startNo...endNo and set pageInfo
tableRows.slice(0).hide();
tableRows.slice(startNo, endNo).fadeIn();
$('#PageInfo').text(pageNo + "/" + pageCount);
```

### Datei "davinci.content.showtime.subst.html"

```js
//<!DOCTY html>
<!-- daVinci substitution list with SHOWTIME like JavaScript list flipping -- STÜBER SYSTEMS 2013 -->
<html class="no-js">
<head>
<meta http-equiv="content-type" content="text/html; charset=UTF-8">
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
<title>daVinci</title>
<meta name="description" content="timetable">
<meta name="GENERATOR" content="%CREATOR%" >
<meta name="Author" content="%AUTHOR%">
<meta name="Keywords" con-tent="daVinci,timetable,timetabler,Stundenplanprogramm,Stundenplansoftware,Stundenplan">
<meta http-equiv="expires" content="0">
<meta http-equiv="content-type" content="text/html; charset=utf-8">
<meta name="page-topic" content="daVinci Stundenplan" >
<meta name="language" content="de, deutsch, at, ch, german" >
<meta name="viewport" content="width=device-width">
<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script type="text/javascript" src="sandbox/davinci.listflip.js"></script>
<link rel="stylesheet" href="sandbox/davinci.content.main.css">
</head>
<body>
<div id="PageInfo">1/1</div>
%DAVINCICONTENT%
</body>
</html>
```

!!! info "Hinweis"

    Kopieren Sie ggf. die Dateien jquery.min.js, davinci.listflip.js und davin-ci.content.main.css auf Ihren Webserver und ändern Sie die Verweise in der davin-ci.content.showtime.subst.html entsprechend.ndern Sie ggf.Dateien mit dem Präfix „davinci.“ werden vom daVinci HTML-Präprozessor ggf. verändert, indem die Variablen ersetzt werden.

Wichtige Dateien | Beschreibung
-|-
jquery.min.js | Datei aus der jQuery-Bibliothek wird von davinci.listflip.js benötigt. Sie können Sie von den Google-Website laden und in einen Ordner auf Ihrer Website kopieren
davinci.listflip.js | Der DAVINCI List-Flip Effekt. Dort können Sie die Anzeigedauer einer Seite und die Anzahl der Zeilen pro Seite einstellen.
davinci.content.main.css | Die eigentliche daVinci CSS-Datei, die das Layout, d.h. Farben, Schriftgrößen usw. bestimmt.

!!! info "Hinweis"

    jQuery ist eine häufig genutzte freie JavaScript Bibliothek, die nützliche Funktionen für HTML-Seiten zur Verfügung stellt.
