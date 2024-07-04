# Änderungen 2016

## DaVinci Version 6.5.18

Veröffentlichung: 27.12.2016

### Fehlerkorrektur

* Stundenplan: Veranstaltungen können wieder bearbeitet werden.

## DaVinci Version 6.5.17 \ WebBox Version 1.9.7

Veröffentlichung: 23.12.2016

### Fehlerkorrektur

* Vertretungsplan: es können wieder vorziehbare Stunden ausgewählt werden.
* WebBox: Korrektur bei der Sortierung in der Vertretungsliste
* WebBox/App: offene Raumfehlzeiten werden nun korrekt angezeigt
* Vertretungsplan: vorgezogener Unterricht wird nun wieder korrekt zurückgesetzt wenn dieser Lehrer als fehlend erfasst wird
* Stundenplan: bei der Verplanung einer Doppelstunde über eine große Pause wurde in der Veranstaltungsliste in der Spalte "Dauer" der Wert falsch ausgegeben. Dies hatte auch zur Folge, dass die IST-Stunden in den Zeitkonten falsch berechnet wurden. Dies ist nun korrigiert.
* Stundenplan: Fehler beim Anlegen neuer Veranstaltungen in der Unterrichtsmatrix behoben.

## DaVinci Version 6.5.16 \ WebBox Version 1.9.6 

Veröffentlichung: 16.12.2016

### Fehlerkorrektur

* Explorer: Import der Benutzerdaten korrigiert - die Spalten "Vorname" und "Nachname" werden mit den richtigen Inhalten befüllt
* Vertretungsplan: Freistellung Lehrer und Raum inkl. Vertretungsregelung wird nun wieder korrekt in DaVinci Look angezeigt
* Vertretungsplan: Ausdruck/HTML-Export - korrigierte Ausgabe fehlender Lehrer (es werden keine mehr doppelt ausgegeben)
* Stundenplan\|Aufsichtsplan: Wenn man im Aufsichtsplan Bereich einen Lehrer gesucht hat und ihn hier eingeben hat, ist das Programm in den Stundenplanbereich gewechselt - dies geschieht nun nicht mehr, man bleibt weiterhin im Bereich Aufsichtsplan.
* Stundenplan: Bei der Verplanung einer Doppelstunde über eine große Pause wurde in der Veranstaltungsliste in der Spalte "Dauer" der Wert falsch ausgegeben. Dies ist nun korrigiert.
* WebBox: Korrektur der Anzeige, wenn ein Raum nicht verfügbar ist.

### Verbesserte bzw. geänderte Funktion

* Server: Verbesserte Verarbeitung bei Anfragen der DaVinci-WebBox und von DaVinci-Mobile über den DaVinci-InfoServer.
* WebBox: Verbesserte Verarbeitung von Anfragen den DaVinci-InfoServer
* WebBox: Neuer Parameter "substitutionShowSupervision" zur optionale Anzeige der Aufsichtsänderungen in der Vertretungsliste nach Stunden.
* Explorer: neue Richtlinie für DaVinci InfoServer: "DaVinci WebBox/Mobile Lehrernamen anzeigen". Damit können Sie entscheiden, ob im Stundenplan/Vertretungsplan das Kürzel oder der Name des Lehrer angezeigt werden soll.
* Vertretungsplan: In den Druckformaten bzw. HTML-Exportformaten für den Vertretungsplan (Tagesvertretungen nach Klassen, nach Stunden, nach Lehrern) können Sie über die neue Option "Aufsichten anzeigen" individuell festlegen, ob die Aufsichtsänderungen mit ausgegeben werden sollen. 
 
## Version 6.5.15

Veröffentlichung: 04.12.2016

### Fehlerkorrektur

* Stundenplan: Befristungen von Veranstaltungen werden bei der Berechnung berücksichtigt
* Kursplan: Periodenzuweisung wird nun bei Kursen mit Lehrer- und Raumzuweisung) innerhalb eines Blockes geprüft, Konflikte die fälschlicherweise angezeigt wurden, sind somit gelöst 
* HTML-Export: fehlende Lehrer / Klassen werden wieder korrekt über dem entsprechenden Vertretungstag ausgegeben
* Vertretungsplan: Lehrerzuweisung bei einer nachträglich eingesetzten Fehlstelle korrigiert
* Vertretungsplan: Beim Eintrag einer Fehlzeit für eine Klasse oder einen Raum können die Fehlgründe wieder korrekt ausgewählt werden.
* Vertretungsplan: HTML-Export von Klassenvertretungen blendet jetzt korrekt Aufsichten aus.
* Vertretungsplan: Einsatz eines Vertretungslehrers und gleichzeitige Raumänderung sind jetzt wieder in einem Vertretungslement möglich.
* Vertretungsplan: Ausdruck | ganztägige Mitteilungen erscheinen wieder unter "Tagesvertretungen nach Klassen/Lehrern"
* Vertretungsplan: wird der Vertretungslehrer krank, wird nun richtig die Vertretungserstellung wieder zurückgesetzt
* Vertretungsplan: Ausdruck | eingetragener Zusatzunterricht von Lehrern ohne Klassenzuweisung wird nicht mehr im Druckformat "Tagesvertretungen nach Klassen" ausgegeben
* Vertretungsplan: Druckformat "Klassenvertretungen" - arbeitet man mit Teamfilterungen werden nun wieder korrekt alle Einträge gemäß der Filterung im Ausdruck angezeigt
* Vertretungsplan: Ausdruck | fehlende Anzeige im Ausdruck Einzelplan Klassen 2zeilig korrigiert
* Vertretungsplan: Ausdruck | Raumvertretungen für Räume, denen keine Lehrer zugewiesen ist, werden beim Drucken mit angezeigt
* Vertretungsplan: Ausdruck | Ganztägige Mitteilung werden in den Tagesvertretungsplänen wieder angezeigt
* Vertretungsplan: Ausdruck und HTML-Export | die Originalposition einer verschobene Stunde wird in den Vertretungslisten wieder korrekt mit angezeigt (z.B. mit dem Hinweis "auf Mo 5.12. 1. Std verschoben").
*  Vertretungsplan: HTML-Export | im Exportformat "Tagesvertretungen nach Stunden" werden Aufsichten nicht mehr mit ausgegeben. 

### Verbesserte bzw. geänderte Funktion

* Vertretungsplan: Ausdruck | im Druckformat "Vertretungslehrerliste" und "Lehrervertretungen" wird im Feld "Zeit" nun die Beginn und Endzeit einer Unterrichtsstunde ausgegeben. 
* FACHWAHL: neue Fachwahlskripte (Gymnasium und berufliches Gymnasium) für Hessen, für die Anleitung klicken Sie bitte auf die Links:
  * [HES-FW-APO-BGY-2015.js](https://doc.la.stueber.de/fachwahl/hes-fw-apo-bgy-2015js/)
  * [HES-FW-APO-2015.js](https://doc.la.stueber.de/fachwahl/hes-fw-apo-2015js/)

## Version 6.5.14

Veröffentlichung: 17.11.2016

### Fehlerkorrektur

* Vertretungsplan: Will man in eine bestehende Vertretung eine andere Vertretung einsetzen, muss man nicht mehr zuerst die Schaltfläche "Zurücksetzen" wählen, um dann einen anderen Vertreter einzusetzen. Durch erneute Anwahl der Schaltfläche "Einsetzen" wird die bestehende Vertretung überschrieben - diese neue Funkion ist korrigiert.
* Vertretungsplan: "Nicht öffentliche" Elemente werden nicht mehr in den Ausdruck übergeben.
* Vertretungsplan: Ansicht Vertretungsplan|Fehlzeiten (Ansicht Plan und Zeitplan): beim Aufruf eines Lehrers eines Lehrers über den Plan wird die Ansicht Zeitplan mit aktualisiert
* AUSDRUCK: Im Druckformat "Gesamtplan Aufsichten" gibt es im Design nun auch die Registerkarte "Seite", damit lässt sich nun bestimmen, ob das Kürzel oder der Langname des Lehrers im Ausdruck erscheint.
* AUSDRUCK: Gültigkeit einer Veranstaltung wird im Druck mit ausgegeben 
* AUSDRUCK: Konferenzliste - der Klassenfilter wurde korrigiert, es werden nur Lehrer die in der Klasse unterrichten ausgegeben
* Explorer: im Dialogfenster "Richtlinie bearbeiten" wird der Wert im Feld ''Richtlinie'' wieder korrekt angezeigt
* HTML-Export: Aufsichten werden im HTML Export wieder mit ausgegeben
* KALENDER: beim Eintrag einer Fehlzeit für einen Lehrer über den Kalender wird als Info "abwesend" mit ausgegeben
* InfoServer: Aufruf der Vertretungsansichten funktioniert wieder
* WebBox/InfoServer: offene Vertretungen werden nicht mehr in den Vertretungslisten angezeigt

## Version 6.5.13

Veröffentlichung: 28.10.2016

### Fehlerkorrektur

* DRUCKEN: Problem des fortlaufenden Datums für Klassenpläne behoben
* DRUCKEN: Problem bei Anzeige der Vorschau  für alle Klassen oder allen Räumen für die Druckformate "Gesamtplan Klassen (Tage und Stunden oben)" und "Gesamtplan Räume (Tage und Stunden oben)" behoben
* HTML-Export: beim Export mehrerer Tage werden nun wieder korrekt wie im gewählten Exportformat eingestellt, "Je Tag eine Datei" oder wenn diese Option deaktiviert ist, nur eine Datei für mehrer Tage exportiert

### Verbesserte bzw. geänderte Funktion

* KALENDER: Für Ereignisse im Kalender, die eine Fehlzeit im Stundenplan zu Folge haben, wird die Fehlzeit im Plan bezeichnet (zuvor nur schraffiert).
* KALENDER: Der Kalenderexport überträgt jetzt auch für ical-Dateien die Detailkalender der einzelnen Kollegen, wenn diese mit angekreuzt werden.

## Version 6.5.12

Veröffentlichung: 20.10.2016

### Fehlerkorrektur 

* Vertretungsplan: Funktionstaste F3 klappt wieder unter ``Vertretungen > Vertretungen``. 
* DRUCKEN: Fehler beim Teamfilter in den Druckformaten für den Vertretungsplan behoben
* DRUCKEN: Fehler in den Original-Druckformatvorlagen behoben, damit Druckformate im Dialogfenster "Druckformate" über die Schaltfläche `` Aktualisieren`` wieder aktualisiert werden können. Eigene Formate, die über ```Hinzufügen``` oder ```Duplizieren``` hinzugefügt und abweichend benannt wurden, bleiben unverändert.
* DRUCKEN: Kursplan | fehlender Kurs, im Ausdruck erscheint fehlende Klasse und Kursbezeichnung 
* DRUCKEN: Ausdruck | Lehrer Zeitkonto - Benutzerdefinierte Spaltenbreite - ändern nicht möglich 
* DRUCKEN: Format "Gesamtplan Klassen (Tage oben Stunden links 3zeilig)" funktioniert
* DRUCKEN: Schienendarstellung im Klassenplan
* KALENDER: um im Kalenderdruck Kalender|Ereignisse|Drucken die gesamten Notizen zu drucken, im Bildschirm mit der Maus den Spaltentitel vergrössern, das überträgt sich auf den Ausdruck.
* InfoServer: Teamfilter klappt
* InfoServer: Aufsichten vor Unterrichtsbeginn werden korrekt angezeigt

### Verbesserte bzw. geänderte Funktion

* Stundenplan: Durch die Einführung des neuen Druckformattyp "Gesamtplan Aufsichten" konnten die bisherigen Druckformate des Druckformattypes "Aufsichtsplan" nicht übernommen werden. Sie müssen in diesem Fall Ihre selbst erstellten Druckformate vom Typ ""Aufsichtsplan" neu erstellen oder über die Schaltfläche `` Aktualisieren`` die Originalvorlage "Aufsichtsplan" neu importieren.
* ALLGEMEIN: Filtermöglichkeiten – es gibt jetzt die Möglichkeit vorhanden Filter aufzurufen –„Filter laden“
* Stundenplan: Stammdaten der Räume - ein Raum kann jetzt mehreren Teams zugeordnet werden 

## Version 6.5.11

Veröffentlichung: 12.10.2016

### Fehlerkorrektur

* ALLGEMEIN: Bayern: Ausgabe der Statistik für WinLD korrigiert.

* VERTRETUNGPLAN: Beim Drucken von Klassenvertretungen, Lehrervertretungen und Vertretungslehrerlisten wird jeweils im Kopf der Listen wieder das Datum mit ausgegeben.
* Vertretungsplan: Beim Drucken/HTML-Export von Klassenvertretungen werden jetzt Aufsichten wieder ausgeblendet.
* Vertretungsplan: Korrektur beim HTML-Export von Tagesvertretungen
* Vertretungsplan: Funktionstaste F5 klappt wieder
* Vertretungsplan: Im Ausdruck werden wieder Termine, die über den Befehl ```Termine vertauschen``` vertauscht wurden, angezeigt

* Stundenplan: Beim Drucken von Gesamtplänen werden jetzt Sperrungen bei Doppelstunden korrekt ausgegeben.
* Stundenplan: Stundentafel Eingabe positiver und negativer Anrechenstunden

* Kursplan: von der Automatik ausgenommene Kurse und Blöcke werden bei der Optimierung nicht mehr berücksichtigt
* Kursplan: Weiterblättern - Ansicht "Kursplan|Fachwahlen" über die Tasten Pfeil nach oben, Pfeil nach unten

* Look: Vertretungsanzeige der Klassen korrigiert

* DRUCK: Ausdruck | Veranstaltungsliste Lehrer -  Sortierung für ausgegebene Spalten nach Klassen
* DRUCK: Klassenplänen |Zusatzinformation Klassenleiter 
* DRUCK: Vertretungslehrerliste | Bemerkungen --> geänderte Schriftart im Druckformat  gespeichert 
* DRUCK: Ausdruck/HTML-Export | Tagesvertretungen | exportiert offene Vertretungen korrigiert
* DRUCK: Veranstaltungsliste Lehrer: Werte in der Spalte "Ist/W" entsprechen jetzt wieder der Anzeige in DaVinci.
* DRUCK: Ausdruck Vertretungsplan | "Termine Vertauschen"  erscheinen wieder im Ausdruck
* Druck: Anschnitt der Buchstaben im Klassenplan korrigiert

* KALENDER: Bereich "Kalender|Kalender" Pfeile zum Blättern in die nächste Woche sind wieder vorhanden

* Mehrbenutzer-Betrieb: Systemfehler (Fehlercode 5) beim Wechsel zwischen Stundenplan und Vertretungsplan (Datei" _backup" konnte nicht gefunden werden) ist gelöst
* Mehrbenutzer-Betrieb: Server speichert letzten Eintrag aus „Vertretungen – Anrechnungen“ beim Trennen 

### Verbesserte bzw. geänderte Funktion

* Look: Ansicht - für die Ausgabe der Ist- Werte aus den Lehrer Zeitkonten ist einstellbar, ob mit geplant oder verplant Werten gerechnet wird

* Stundenplan: Hat man im Nachhinein Änderungen im Zeitrahmen vorgenommen, kann man die gesetzten Stunden an den neuen Zeitrahmen über den Dialog ```Extras > Weitere Aktionen > Terminzeiten anpassen```. Dieser Dialog wurde erweitert. Bitte stellen Sie Folgendes ein: ```Nächste Startzeit davor``` und ```Nächste Endzeit danach```.

![Dialogfenster Terminzeiten anpassen](Terminzeiten anpassen.png)

* Stundenplan: Im Eigenschaften-Dialog ```Plan > Eigenschaften > Statistik ``` kann man jetzt per Option einstellen, ob die Statistikwochenanzahl automatisch berechnet oder manuell eingestellt wird.
![Dialogfenster Eigenschaften](Plan-Eigenschaften.png)
* Stundenplan: Wenn Sie in den Klassenstundentafeln die Spalte Kategorie [Veranstaltungskategorie] gefüllt haben, wird der Wert geklammert in der Veranstaltungsliste eingeblendet, es sein denn, Sie haben der Veranstaltung direkt eine Kategorie zugewiesen.
* Stundenplan: beim Drucken von Gesamtplänen gibt es jetzt den neuen Druckformattyp "Gesamtplan Aufsichten". Damit können Aufsichten jetzt auch als Gesamtplan gedruckt werden.
* Stundenplan: beim Drucken von Stundenplänen ist es jetzt im Druckformat auf der Registerkarte "Weitere Listen" möglich, die "Fach/Lehrer-Legende unter dem Plan" auch optional erst auf der nächsten Seite auszugeben.
* Stundenplan: Im ```Stammdatenfenster > Räume > Teams``` kann man jetzt anstatt eines Teams Räumen eine Liste von Teams zuweisen
* Stundenplan: Markiert man einen Termin im Stundenplan, so kann man jetzt über ```Rechte Maustaste > Terminzeitspanne bearbeiten``` mit der Option ```Pause zählt als Unterrichtszeit``` festlegen, ob eine Pause innerhalb des Termins als Unterrichtszeit mit gezählt werden soll.

* Vertretungsplan: In den Termindetails werden nun neben der Bemerkung auch die Mitteilung und Info angezeigt 
![Veranstaltungsdetails](Veranstaltungsdetails.png)
* Vertretungsplan: Über eine Option im Optiondialog auf Vertretungsplan ```Extras > Optionen > Vertretungsplan```kann man nun einstellen, ob bei einer nachträglichen Raum-/Fachänderung gefragt werden soll, ob alle Räume des Block verändert werden sollen oder nicht
![](dav Optionen.png)
* Vertretungsplan: Man kann jetzt in Listen und Plänen die Schriftart (Schriftart, Schriftschnitt, Schriftgrad) für Hinweise (Schrifteinstellung INFOBEREICH) und andere Texte (Schrifteinstellung BEMERKUNG) getrennt einstellen.(siehe Ausdruck/HTML-Export)
![](Hinweise Bemerkungen.png)

![](Hinweise Bemerkungen_HTML.png)

* Vertretungsplan: Will mean eine bestehende Vertretung eine andere Vertretung einsetzen, muss man nicht mehr zuerst die Schaltfläche "Zurücksetzen" wählen, um dann einen anderen Vertreter einzusetzen. Durch erneute Anwahl der Schaltfläche "Einsetzen" wird die bestehende Vertretung überschrieben. 
* InfoServer: die ```daVinciIS.dll``` gibt es zusätzlich als 64-bit-Variante. Wie genau und in welcher Situation Sie diese einsetzen sollten, beschreiben wir in der InfoServer-Dokumentation im Abschnitt [Verwenden Sie eine 64-bit-Version von Windows?](https://doc.davinci6.stueber.de/09.infoserver/setup-infoserver/). 
* InfoServer: Ausgabe von Vertretungslisten. Erfolgt die Ausgabe ohne weitere Parameter (z.B. ```localhost/davinciis.dll?type=daysubstclass```), so wird unabhängig von der Uhrzeit des Rechners immer die gesamte Vertretungsliste ausgegeben. Bei der zusätzlichen Verwendung des Parameters starttime=now (z.B. ```localhost/davinciis.dll?type=daysubstclass&starttime=now```) wird die Vertretungsliste nur ab dem aktuellen Rechnerdatum ausgegeben.  

* Explorer: neues Recht für den InfoServer: eigener Lehrerplan plus alle Vertretungen 

## Version 6.5.10

Veröffentlichung: 27.09.2016

### Fehlerkorrektur

* Stundenplan: Drucken der "Veranstaltungsliste Lehrer" mit der Option "Lehrer-Zeitkonto unter Veranstaltungsliste" korrigiert
* Stundenplan: Unter ```Stundenplan > Stundenplan``` wird jetzt unter "Summen" auf der Registerkarte "Wochendurchschnitt" auch der Wert von Angleichstunden der Stundentafel korrekt berückschtigt.
* Stundenplan: Beim Drucken von Stundenplänen werden jetzt die Zusatzinformationen wieder korrekt ausgegeben.
* Vertretungsplan: Tagesvertretungsplan berücksichtigt jetzt die Einstellung "Klassenausfall Termine anzeigen" korrekt.
* Vertretungsplan: Aufsichtsänderungen erscheinen wieder im Ausdruck, HTML-Export und im InfoServer.
* Vertretungsplan: Zusatzunterricht ohne Angabe einer Klasse erscheint wieder korrekt im Ausdruck von Tagesplänen und HTML-Export 
* Allgemein: Importieren von Teilstundenplänen 
* NETZ: Hinweis zum Schreibschutz beim mehrfachen parallelen Aufruf der gleichen Plandatei 
* HTML-Export: es können wieder nur Perioden (Kürzel) OHNE Ausgabe der Kalenderwochen ausgeben werden 
* WebBox: Zusatzunterricht wird nun wieder richtig mit Fach- und Raumkürzel ausgegeben
* WebBox: Parameter dateOffset= korrigiert [(Webboxparameter ansehen)](http://davinci-webbox.stueber.de/)
* InfoServer: Stundenpläne, deren Gültigkeitsdatum in der Vergangenheit liegt, werden jetzt korrekt angezeigt
* InfoServer: Fehler bei der uhrzeitabhängigen Anzeige von Vertretungsplänen behoben
* Kursplan: Bei ```Kursplan > Fachwahlen``` kann in der Liste der Schüler wieder die Spalte "Klasse" ein- und ausgeblendet werden. 
* Kursplan: Bei ```Kursplan > Schüler``` kann in der Liste der Schüler wieder die Spalte "Bemerkung" editiert werden. 
* Allgemein: Im Export der EXTERN.dat (BBS und ABS NRW) wurde die Ausgabe der Schülerzahlen korrigiert
* Allgemein: Bayern - Export nach WinLD korrigiert. 
* Look: Suchen über Namen/Kürzel mit Umlauten korrigiert.

### Verbesserte bzw. geänderte Funktion

* Stundenplan: Bei '''Extras > Weitere Aktionen > Terminzeiten anpassen''' gibt es jetzt die neuen Optionen "Termin Startzeit anpassen auf" und "Termin Endezeit anpassen auf".
* WebBox: Neue Richtlinie im DaVinci Explorer unter ```Plandateien > Richtlinien > Richtlinien für DaVinci InfoServer > Stundenpläne anzeigen``` => "Lehrer: eigener Plan und alle Vertretungen" 
* Vertretungsplan: Unter Vertretungsplan > Vertretungen kann man jetzt auch in der Stundenplananzeige Änderungen zurücksetzen.
* Look: Die Schaltflächen "Suchen" und "Lehrer jetzt" sind jetzt auch in der Ansicht "interaktives Vollbild für Touch Screens" verfügbar.
*  InfoServer: Werden mehrere blätternde Listen (zum Beispiel mehrere Tage für den Parameter "daysubstclass") gezeigt:
  * blättern die Listen gleichzeitig, nicht mehr nacheinander. 
  * hat eine der Liste weniger Zeilen, als für den Umbruch eingestellt wurde, blättert sie nicht mit.
  * Die Tabellenhöhe ändert sich beim Blättern nicht (Beispiel Umbruch nach 3 Zeilen, Sie haben insgesamt 4 Zeilen, die zweite Seite hätte dann nur eine Zeile, es werden 2 Leerzeilen ergänzt)
* InfoServer: Zeigen Sie nur eine Liste an und diese hat weniger Zeilen, als für den Umbruch eingestellt wurden, aktualisiert sich die Seite nach einer Minute automatisch.

  >Wenn Sie die HTML-Vorlage "davinci.showtime.subst.local.html" verwenden, wird die für das Blättern verantwortliche Datei "davinci.listflip.js" aus dem Rootverzeichnis (Unterverzeichnis WebBox) Ihres Webservers genutzt. Bitte kopieren Sie nach dem Update der DaVinci-Installation die Datei "davinci.listflip.js" aus dem Pfad C:\ProgramData\Stueber Systems\daVinci 6\HTML\JS in das Verzeichnis "sandbox" ims Rootverzeichnis Ihres Webservers.
> 
InternetInformationServer: ```C:\inetpub\wwwroot\sandbox```
> 
Apache: ```C:\xampp\htdocs\sandbox```

## Version 6.5.9

Veröffentlichung: 03.08.2016

### Fehlerkorrektur

* Stundenplan: Konfliktanzeige bei nicht geblockten Veranstaltungen auf der gleichen Position behoben 
* InfoServer: Aufruf mit Parameter startdate und enddate klappt wieder für den aktuellen Tag 

## Version 6.5.8

Veröffentlichung: 01.08.2016

### Fehlerkorrektur

* Stundenplan: Termin bearbeiten wieder aktiv bei gesetztem Haken unter ```Planansicht > Termine der Veranstaltung hervorheben```
* Stundenplan:  Beim Weiterschalten auf den nächsten Klassenplan in der Ansicht "Plan und Liste" wird die Liste mit aktualisiert.
* DRUCK: bei neuen Druckformaten wird zukünftig die Textfarbe explizit mit schwarz vorbesetzt.
* Stundenplan: Beim Ändern der Terminstückelung im Fenster "Veranstaltung bearbeiten", wird die Unterrichtsart nicht verändert.
* Stundenplan: beim Ändern der Periode einer duplizierten Veranstaltung wird das IST\/W korrekt angepasst.
* Stundenplan: Im Fenster "Neue Veranstaltung" kann das Fach ausgewählt werden, nachdem die Terminstückelung erfasst wurde.
* Stundenplan: Bei Veranstaltungen mit Perioden und einer begrenzten Dauer wurden Konflikte gezeigt, die durch das von-bis-Datum hätten nicht gezeigt werden dürfen. 
* Stundenplan: Im Fenster "passenden Räume" wurden fälschlich bereits für andere Termine der Veranstaltung genutzte Räume als frei gekennzeichnet.

### Verbesserte bzw. geänderte Funktion

* Stundenplan: Beim Setzen per Doppelklick aus dem Unverplantfenster in den Plan, wird nach dem ersten Setzen einer Veranstaltung die nächste Veranstaltung vormarkiert zum Setzen.
* DRUCK: Terminzeilen umbrechen -&gt; Beim Druck von Plänen gibt es in den Optionen zum einzelnen Druckformat die Möglichkeit lange Termininhalte umbrechen zu lassen.
*  Kursplan: Im Kursplan wird bei der Verteilung die Klassenzugehörigkeit innerhalb eines Jahrgangs berücksichtigt.
* Stundenplan: Im Fenster "Veranstaltung bearbeiten" im Unterpunkt "Teilnehmer Termine" werden die Reiter der noch nicht gesetzten Termine jetzt "Termin" (statt Zusatzunterricht) benannt.

![Publizieren > Vorschau > Design > Termine > Terminzeilen umbrechen](/assets/images/imagesumbruch.png)
 
## Version 6.5.7

Veröffentlichung: 11.07.2016

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

> Bitte prüfen Sie, ob Sie die aktuelle WebBox nutzen.Die aktuelle WebBox finden Sie hier [davinci-webbox.stueber.de](http://davinci-webbox.stueber.de/)

## Fehlerkorrektur 

* Stundenplan: Raumverplanung | manuelle Verplanung: Räume der Veranstaltungsliste werden bei der manuellen Verplanung wieder berücksichtigt
*  Stundenplan: Kontextmenübefehl "Plan anzeigen" klappt an allen Stellen wieder
*  Stundenplan: Veranstaltung bearbeiten|Teitdetails Zeitpräferenzen eintragen wieder möglich
*  Stundenplan:  Veranstaltung bearbeiten|Termindauer ändern funktioniert wieder

*  VERTETUNGSPLAN: gibt man eine Raumfehlzeit ein über mehrere Tage, erstellt die Vertretungen und ändert dann die Raumfehlzeit über "Änderung bearbeiten" bleiben nun alle Vertretungen bestehen
*  VERTETUNGSPLAN: Eintrag einer 1stündigen Klassenfehlzeit bei einer Doppelstunde wieder möglich

* InfoServer: Darstellungsfehler im Raumplan bei mehreren gleichzeitigen Veranstaltungen behoben

* AUSDRUCK: Veranstaltungsliste Lehrer mit Lehrerzeitkonto erzeugte eine Zugriffsverletzung
* AUSDRUCK: Veranstaltungsliste Lehrer: bei der Einstellung in den Optionen/Ansicht/Lehrer-Ist-Werte-Zeitkonten = "verplante Stunden" wurden Jahreswerte ausgegeben
* AUSDRUCK: Klassenfehlzeiten können in Tagesvertretungen nach Klassen/Lehrern/Stunden nicht unterdrückt werden
*  AUSDRUCK: Fehlende Klasse wird im Ausdruck wieder angezeigt 

## Verbesserte bzw. geänderte Funktion

* Allgemein: Optionen-Bezeichnungen-Benutzername: hier kann jetzt eingestellt werden, welche Form der Benutzername beim Erzeugen des Benutzernamens haben soll
* MOBIL: In der DaVinci-App und in der DaVinci-WebBox werden aus der Vergangenheit nur die zwei letzten Wochen gezeigt, damit wird die Ladezeit verringert.


## Version 6.5.6

Veröffentlichung: 15.06.2016

!!! info "Hinweis"

     Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!
     Bitte prüfen Sie, ob Sie die aktuelle WebBox nutzen.Die aktuelle WebBox finden Sie hier [davinci-webbox.stueber.de](http://davinci-webbox.stueber.de/)

## Fehlerkorrektur 

* STAMMDATEN: Stammdaten|Räume löschen 

* ALLGEMEIN: Eigenschaften|Zeitraum Änderung von Start- und Enddatum der Datei wird sofort auf die Registerkarte Eigenschaften|Statistik für die Wochenauswahl übernommen

* Stundenplan:Unterrichtsmatrix "Zellen ohne Zuweisung hervorheben" korrigiert
* Stundenplan: Anzeige der Symbole beim Zuweisen der Räume über "Passende Räume"
* Stundenplan: Zeile "verplant" bei den Summen der Klassen bei allen Berechnungsarten ersichtlich

* WebBox: Stundenplan beginnt in der Zukunft: Nur erste Woche wurde für App/WebBox in JSON exportiert  
* WebBox: Anzeige fehlender Klassen im Lehrerplan und in der Vertretungsansicht

* Vertretungsplan: F3 für den Eintrag von Zusatzunterricht
* Vertretungsplan: Vertretungsentfallgrund für Klassen wird wieder angezeigt
* Vertretungsplan: hat man im Schlüsselverzeichnis Lehrerfehlgründe den Haken beim Anrechnen gesetzt, kann man beim Eintrag einer Fehlzeit diesen entfernen, umgekehrt genauso
* Vertretungsplan: fehlender Raum wurde zur eigenen Vertretung angeboten 
* Vertretungsplan: beim Ändern eines Raumes oder Faches nach dem Einsetzen einer Vertretung wird nur für geblockten Unterricht die Möglichkeit geboten, Fach und Raum für den gesamten Block zu ändern
* Vertretungsplan: Fehler beim Lehrer-/Raumtausch mit gleichem Raum

* Explorer:  Mandantenauswahl und Löschen beim Benutzer "admin" nicht mehr möglich

* Kursplan: Zugriffsverletzung beim Öffnen des Kursplanes
 
* OPTIONEN: automatische Speicherung im lokalen Betrieb ist wieder mehr möglich

* EXPORT: JSON Export korrigiert, Feld lessontimes


## Verbesserte bzw. geänderte Funktion

* STAMMDATEN: Stammdaten|Fächer neue Fachkategorie "Literatur"

* Look: beim Eintrag einer Lehrerfehlzeit in Look werden automatisch Anrechstunden vergeben, wenn dies im Schlüsselverzeichnis Lehrerfehlgründe vorgegeben ist

* Vertretungsplan: Anrechenstunden beim Eintrag eines Zusatzunterrichtes für mehrere Lehrerwerden jetzt pro Lehrer in einer Zeile ausgegeben

## Version 6.5.5

Veröffentlichung: 28.05.2016

!!! info "Hinweis"

    Bitte prüfen Sie, ob Sie die aktuelle WebBox nutzen. Die aktuelle WebBox finden Sie hier [davinci-webbox.stueber.de](http://davinci-webbox.stueber.de/)

## Fehlerkorrektur 

* InfoServer: Teilweise vorhanderer Installationfehler beim Start des IIS nach dem Update behoben.
* Vertretungsplan: Ansicht "Vertretungen" Spalte "Fach" wir jetzt wieder korrekt gefüllt angezeigt.
* Look: Fehler bei der Anzeige "Lehrer jetzt", "Klassen jetzt" und "Räume jetzt" bei eingestellter Eigenschaft "Immer Uhrzeit anzeigen" behoben.

## Version 6.5.4

Veröffentlichung: 26.05.2016

!!! info "Hinweis"

    Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten! Bitte prüfen Sie, ob Sie die aktuelle WebBox nutzen. Die aktuelle WebBox finden Sie hier [davinci-webbox.stueber.de](http://davinci-webbox.stueber.de/)

### Fehlerkorrektur 

* STAMMDATEN: Stammdaten|Stundentafeln: Fächer einer Stundentafel kopieren und einfügen 

* Stundenplan: erneute Korrektur der Lehrerstundensummen
* Stundenplan: aktuell gewählter Aufsichtbereichsplan bleibt mit Lehrerzuweisung geöffnet
* Stundenplan: das Löschen von Perioden im Stammdatenfenster, die nur auf Terminebene zugewiesen wurden, hat zu einem Problem in DaVinci geführt, welches nun gelöst ist
* Stundenplan: Wenn Sie unter `Start > Planansicht > Positionskonflikte anzeigen`aktiviert haben, ist der erwartete "gelbe Streifen", der die mögliche Position für einen Termin bei manueller Verplanung anzeigt, wieder vorhanden.
* Stundenplan: Beim Anlegen einer neuen Plandatei für das neue Schuljahr werden in den Plan-Eigenschaften|Statistik unter Wochenbezogenen Summen wieder alle Wochen als markiert angezeigt (in diesen Wochen wird Unterricht verplant/stattfinden). Sie müssen nun wie gewohnt den Haken vor ganzen Ferien-Unterrichtsfreien-Wochen entfernen.

* Vertretungsplan: Fach/ Raum ändern nach Vertretungserstellung
* Vertretungsplan: Lehrer-Raum Tausch wieder möglich 
* Vertretungsplan: Vertretung von Aufsichtsbereichen wieder möglich
* Vertretungsplan: Fehlzeiten löschen führt nun auch zum zurücksetzen des vorgezogenen Unterrichts
* Vertretungsplan: Beim Erfassen einer Klassenfehlzeit in einer Woche in der Zukunft werden nun wieder richtig im weiteren Fenster die vom Fehlen der Klasse betroffenen Lehrer angezeigt

* KALENDER: Erfasst man über die Ansicht "Kalender" ein Ereignis für Klassen, werden nun richtig die Lehrer aufgelistet, die die Klassen zum Zeitpunkt des Ereignisses unterrichten. Diese erhalten eine entsprechende Fehlzeit. Sie können nun entscheiden, ob diese Stunden angerechnet werden sollen oder nicht.

* DaVinci-Optionen: Meine Daten: Schulnamenzeile wird nicht mehr gedoppelt

* AUSDRUCK: Wochengesamtplan Räume - Sperrungen werden nun für alle Räume richtig im Ausdruck angezeigt

* Kursplan: Blockungsautomatik erneut überarbeitet

* Look: Wurde in den DaVinci Look-Optionen unter 'Ansicht>Sichtbarkeit' "keine Lehrerplan-Ansicht" eingestellt, gelangt man nicht mehr über die Suche zum Lehrerplan.

* ÜBERSICHTEN: Übersicht "Unterrichtsstatistik" - werden im Klassenplan Veranstaltungen eines Lehrers, der an diesem Tag fehlend ist, verschoben, (1. Schritt: Unterricht des Lehrers am Tag "X" wird verschoben, 2. Schritt: Lehrer wird an Tag "X" als fehlend erfasst) werden diese verschobenen Stunden nicht mehr als Ausfallstunden gelistet.

* WebBox und App: Pläne mit einem Startdatum in der Zukunft werden dargestellt.

* InfoServer: Ansicht der Schülerstundenpläne funktioniert wieder

### Verbesserte bzw. geänderte Funktion

* WebBox und App: Aufsichten werden mit angezeigt

* STAMMDATEN: Stammdaten|Lehrer: Zeitkontoanzeige überarbeitet, Anrechnungen = Summe aus Mehr- und Mindergründen 

* HINWEIS zum Vertretungsplan: Überlagerung von Fehlzeiten - Trägt man eine Klassenfehlzeit ein, erhalten einige Lehrer dadurch negative Anrechenstunden. Wenn nun einer dieser betroffenen Lehrer für den gleichen Zeitraum als fehlend erfasst wird (hier "Ohne Anrechenstunden" verbucht), bleiben die negativen Anrechenstunden durch eingetragene Klassenfehlzeit bestehen. Diese müssen Sie manuell löschen. 

* Vertretungsplan: im Schlüsselverzeichniss "Lehrerfehlgründe" kann man festlegen, ob bei einem Fehlgrund generell Anrechenstunden vergeben werden sollen oder nicht, der Haken bei "Anrechnen" beim Erfassen der Fehlzeit ist dann automatisch (nicht) gesetzt

* Schuldatentransferformat: Im Format gibt es die neuen Datensätze UC und U7. Sie dienen dazu die Daten mit DaVinci zu synchronisieren, d.h. bestehende Veranstaltungen/Termine werden ggf. überschrieben anstatt neu angelegt. Siehe [http://doc.sdtf.stueber.de/](http://doc.sdtf.stueber.de/)

* Statistik: NRW GPC Statistik: aus der Übersicht "Lehrer-Arbeitstage" wählen Sie bitte Importieren/Exportieren|Statistikdaten Nordrhein Westfalen GPC exportieren

## Version 6.5.3

Veröffentlichung: 07.05.2016

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Fehlerkorrektur

* Stundenplan: Problem bei manueller Verplanung von Stunden und möglichem Raumverlust gelöst - es lag an einem falsch erkannten Wegzeitproblem, das hier zum entfernen des hinterlegten Raumes geführt hat 
* Stundenplan: im Aufsichtsplan werden wieder mögliche Aufsichtslehrer richtig mit Ihren Stundenplaninformationen angezeigt, davor wurde fälschlicherweise bei allen Lehrern "kein Unterricht an diesem Tag" ausgegeben
* Stundenplan: Fehler bei Summierung der Iststunden im Zeitkonto behoben
* Stundenplan: Anzeige der Summen-Werte "Geplant je Woche" korrigiert, auch in der Ansicht "Jahresverteilung"
* Vertretungsplan: soll für mehrere fehlende Lehrer der Unterricht entfallen, können Sie die offenen Vertretungen dieser Lehrer über eine Bereichsmarkierung auswählen und auf "entfällt" setzen
* Vertretungsplan: Fehlzeiten für Räume werden jetzt wieder korrekt in der Ansicht "Vertretungen" als zu vertretende Termine angezeigt
* Vertretungsplan: Zugriffsverletzung beim Freistellen (Lehrer, Raum) korrigiert
* Vertretungsplan: Anrechenstunden - durch Erfassen einer Klassenfehlzeit erhalten Lehrer Anrechenstunden, diese bleiben nach Erfassen einer Lehrerfehlzeit für einen von der Klassenfehlzeit betroffenen Lehrer erhalten (stehen weiterhin in Ansicht "Anrechnungen")
* Kursplan: Kursplan|Blöcke Verteilung zurücksetzen getrennt nach Bändern
* AUSDRUCK: "Tagesvertretungen nach Klassen" - die bearbeitete "Bezeichnung (Lehrer)" (z.B. [Saluation] [Surname]) in den Überschriften/Zellen wird wieder korrekt in den Ausdruck übergeben
* Look: eingestellte Optionen bei Programmstart (unter DaVinci Optionen|Einstellungen) werden beim Öffnen von DaVinci Look wieder übernommen

### Verbesserte bzw. geänderte Funktion

* Stundenplan: unter "Start|Planansicht" gibt es neu die Option "Wegzeitkonflikte anzeigen"
* Stundenplan: Aufsichtsbereichsplan, neben dem Status "Nicht verfügbar" und "Ausgezeichnet" gibt es den neuen Status "Planbar". Diese Lehrer könnten als Aufsichtslehrer zugewiesen werden, sind aber eher ungeeignet, weil sie "Unterrichtsende davor haben" oder "Unterrichtsbeginn danach haben".
* Vertretungsplan: Das Eintragen von Zusatzunterricht. Mitteilung und Fehlstellen kann jetzt auch optional über die Funktionstasten `F3`, `F4` und `F5` erfolgen. 
* Stundenplan: unter "Stammdaten|Fächer" gibt es jetzt unter "Details" die neue Einstellung "Keine Aufsicht danach". Auf diese Weise kann für Lehrer, die unmittelbar vor einer Aufsicht dieses Fach unterrichten, festgelegt werden, dass für solche Lehrer bei der Wahl als mögliche Aufsichtslehrer dieser Sachverhalt speziell ausgewiesen wird. Der Hinweis in der Ansicht "Stundenplan|Aufsichtpslan" lautet dann in der Spalte "Bemerkung" der betroffenen Lehrer "Aufsicht nach X verboten". X steht hier stellvertretend für ein Fachkürzel.
* Stundenplan: Im Zusatzfenster "Summen" werden die Informationen zur „Angleichung“ ausgeblendet, wenn die Angleichung in der Stundentafel der jeweiligen Klasse "Null" ist. 
* Kursplan: Im Bereich "Kursplan|Schüler" / "Kursplan|Fachwahl" kann man nun über "Start|NEUE FACHWAHL" beim Schüler eine neue Fachwahl eingeben, wenn dieser noch keine Kurse zugeordnet hat. Dies ist als zusätzliche Möglichkeit gedacht. 

## Version 6.5.2

Veröffentlichung: 25.04.2016

### Fehlerkorrektur

* Vertretungsplan: Es wurden keine Änderungselemente erzeugt. Wenn Sie bereits Fehlzeiten engetragen haben, erzeugen Sie bitte mit rechter Maustaste und "Anderungen neu erstellen" die fehlenden Änderungselemente oder löschen Sie die Fehlzeiten und geben Sie sie erneut ein.

## Version 6.5.1

Veröffentlichung: 22.04.2016

!!! info "Hinweis"

    Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Fehlerkorrektur

* KALENDER: erzeugte Fehlzeiten durch einen Kalendereintrag über mehrere Tage werden in die Ansicht Vertretungsplan korrekt übergeben
* KALENDER: Erfassung von Ereignissen (z.B. Klassenfahrten) über den KALENDER haben ggf. Fehlzeiten für Lehrer und Klassen zur Folge. Beim Eintrag einer Klassenfehlzeit, werden Klasse und begleitende Lehrer im Vertretungsplan als fehlend angezeigt. Nun kann man auch entscheiden, ob diese Lehrer Anrechenstunden erhalten sollen oder nicht.
* KALENDER: erfasst man im Kalender ein Ereignis, dass nach dem Unterricht beginnt und bis zum nächsten Tag dauert, werden die Fehlzeiten nun korrekt übernommen
* Vertretungsplan: Verschieben (Ansicht nur ein Plan) von Stunden in eine andere KW wieder möglich
* Vertretungsplan: F6, F6, F7 in der Stundenplanansicht im Bereich Vertretungen|Vertretungen funktionieren wieder
* Vertretungsplan: Vorziehen von Stunden in Plandatei mit unterschiedlichen Zeitrahmen wird wieder mit den richtigen Unterrichtszeiten beim Lehrer angezeigt
* Vertretungsplan: Ansicht "Plan und Zeitplan" - Zeitplan springt nach Fehlzeitenerfassung Lehrer nicht mehr auf die Klasse zurück
* Vertretungsplan: Lehrerfehlzeit wird nach Vertretungsregelung verändert, vorgezogenen Elemente werden korrigiert
* Vertretungsplan: Freistellung von 2 aufeinanderfolgenden Einzelstunden korrigiert
* Vertretungsplan: Vorziehenoptionen korrigiert
* Vertretungsplan: Freistellung bei unterschiedlichen Zeitrahmen korrigiert
* Vertretungsplan: Fehlzeiten / Planung mit unterschiedlichen Zeitrahmen (leere Zeilen in der Liste offenen Vertretungen korrigiert)
* Vertretungsplan: Übersichten|Änderungen - Export korrigiert
* Kursplan: Blockungsautomatik überarbeitet, wenn "Blockkonflikte akzeptieren" markiert ist, werden nun trotz möglicher Konflikte alle Schüler auf Kurse verteilt
* Kursplan: "Blöcke anpassen" korrigiert
* Kursplan: um ungültige Blockbezeichnungen zu löschen, bitte einmal "Extras|Plandatei aufräumen" wählen
* Kursplan: Kursplan|Blöcke Befehl "Optimierung" Optimierung der Schülerzahlen bei Kursen des gleichen Faches innerhalb eines Blockes
* Kursplan: Verplanung der Kurse auf Blöcke prüft nun auch Lehrerüberschneidung  
* Explorer: Nutzer ohne Berechtigung können Ihr eigenes Kennwort nicht ändern
* Stundenplan: Plan|Eigenschaften|Statistik, Bereich "Wochenbezogene Summen", entfernte Haken vor Kalenderwochen werden wieder gespeichert
* Stundenplan: Änderung der Wochen im Bereich "Veranstaltungen" werden auf die Terminebene übertragen  
* Stundenplan: Stundenplan|Ansicht "Plan und Liste": ändert man die Wochenauswahl in der Veranstaltungsliste, aktualisiert sich die Anzeige im Plan wieder
* Stundenplan: Sortierung im Stammdatenfenster über Schaltfläche "AZ-Sortieren"- nun kann aufwärts oder abwärts sortiert werden
* Stundenplan: Fach "Präsenz" wird in die statistische Berechnung einbezogen 
* Stundenplan: Konfliktanzeige korrigiert
* Stundenplan: Unterrichtsmatrix|Klassen/Fächer beim Zuordnen von Lehrern, werden die zugeordneten Stunden in der Lehrerdifferenz mitberechnet
* DRUCK: Ausdruck | "Gesamtplan Räume" Sperrungen werden am korrekten Tag ausgegeben
* DRUCK: im Zeitrahmen definierte Trennlinien können gedruckt werden, wenn die entsprechende Option "Trennlinien aus Zeitrahmen drucken" aktiviert ist.
* DRUCK: Anzeige von Zusatzunterricht im Ausdruck "Klassenvertretungen", wenn diese Klasse als fehlend erfasst ist
* DRUCK: Probleme mit Umbruch "jeder Plan auf neuer Seite" gelöst
* DRUCK: "Originaltermine bei Änderungen nicht anzeigen" korrigiert

### Verbesserte bzw. geänderte Funktion

* Stundenplan: "Veranstaltung Bearbeiten"-Fenster, Bereich "Teilnehmer Termine" - in der Registerkarte Schüler gibt es die neue Filtermöglichkeit "Nur Schüler der Klasse", damit werden Ihnen in der Liste nur noch die Schüler der gewählten Klasse angezeigt
* KALENDER: Erfassung von Ereignissen (z.B. Klassenfahrten) über den KALENDER haben ggf. Fehlzeiten für Lehrer und Klassen zur Folge. Beim Eintrag einer Klassenfehlzeit werden Klasse und begleitetende Lehrer im Vertretungsplan als fehlend angezeigt. Nun kann man auch entscheiden, ob diese Lehrer Anrechenstunden erhalten sollen oder nicht.
* KALENDER: trägt man im Kalender ein Ereignis ein, zu einer Zeit zu der der Lehrer keinen Unterricht hat, wird jetzt auch eine Fehlzeit erzeugt und im Bereich Vertretungsplan angezeigt 
* Vertretungsplan: Fehlzeiten| Ansicht Liste der Fehlzeiten - neue Spalte "Fehlt"
* Vertretungsplan: Änderungsliste - neue Spalte "Schulform"
* Kursplan: Kursplan|Kurse: Spalte "Dauer unabhängig"

## Version 6.0.210 (16.03.2016) Dateiformat 6.0.160

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

## Neue Funktionen

* Stundenplan: In der Stundenplanansicht unter dem Aufruf "PLANANSICHT" sind jetzt die entsprechenden Einstellungen aus dem Automatikvorgaben und dem Optionsfenster direkt sichtbar und einstellbar.
* Stundenplan: Zusatzfenster "passende Räume" und "passende Lehrer" - neue Auswahl: auch verplante Räume anzeigen, auch verplante Lehrer anzeigen
* Druck: Druckformate TERMINE: Neue Option „Termine umbrechen“

## Verbesserte bzw. geänderte Funktion

* Stundenplan: "Veranstaltung bearbeiten": Bei den Teilnehmern können wieder Klassen ausgewählt werden.

## Fehlerkorrektur

* Stundenplan: Fehler mit den Dateidatum (Planungszeitraum) im Servermodus ist jetzt beseitigt.

### Version 6.0.209 (16.03.2016) Dateiformat 6.0.156

## Fehlerkorrektur

* KALENDER: wird ein Ereignis eintragen, wird die Auswahl der markierten Tage korrekt ins die Datumsauswahl übernommen
* Look: Kalender in Look über die Ansicht Ereignisse ist nur noch mit dem entsprechenden Benutzerrecht möglich 
* Vertretungsplan: Befehle in der Menüleiste zum Bearbeiten des Vertretungsplanes aktiv
* Vertretungsplan: Fach ändern, Anzeige korrigiert
* Vertretungsplan: Raum ändern, Anzeige korrigiert
* Vertretungsplan: Verschieben/Vertauschen 
* Vertretungsplan: Eingabe mehrtägiger Fehlzeiten

### Version 6.0.208 (15.03.2016) Dateiformat 6.0.155

!!! info "Hinweis"

    Bitte beachten Sie: Der DaVinci Server erwartet jetzt eine Lizenzdatei, genauer gesagt die übliche DaVinci.LIC Datei. Andernfalls kann der InfoServer nicht genutzt werden. Sie können den DaVinci Server über die Systemsteuerung öffnen und über die neue Schaltfläche "Lizenz" die Lizenzdatei importieren bzw. die Lizenz eingeben. Bitte stoppen uns starten Sie dann einmal den DaVinci Server.

## Neue Funktionen

* Allgemein: über PLAN > Importieren/Exportieren können die Benutzerdaten Klassen, Lehrer, Schüler exportiert werden
* Allgemein: im Stammdatenfenster können Sie über eine Mehrfachmarkierung|rechte Maustaste "Benutzername vorbesetzen", damit werden für Schüler, 
  Klassen und Lehrer die Spalte "Benutzername" gefüllt (falls Spalte "Benutzername" noch nicht gesetzt)
* Allgemein: Perioden bearbeiten - Anzeige zu der Woche im Datumsformat
* Allgemein: Statistikexport NRW GPC – Krankheitsstatistik
* Stundenplan: Neue Option "Stundenplan|Terminzeilen umbrechen" im Dialog "Plan|Eigenschaften", sorgt für bessere Dastellung bei langen Texten in Terminen. 
* Stundenplan: Neue Option "Stundenplan|In der Ansicht alle Wochen auch einmalige Termine einzeigen" im Dialog "Plan|Eigenschaften". Damit werden in der Ansicht "Alle Wochen"" auch alle einmaleigen Termine mitangezeigt.
* Stundenplan: Neue Option "Termin Wochen Format" im Dialog "Plan|Eigenschaften" ermöglicht es, die Anzeige der Terminwochen einzustellen. Verschiedenste Eintragungen sind möglich: keine Wochennummer ("leer"), Kalender-Wochennummer ("W" -> 1,3,5), Datum ("dd.mm.yy" -> 01.02.16, "dd.mm." ->01.02., "dd.mm" -> 01.02, "yyyy-mm-dd" -> 2016-02-01, „W. KW“ -> 32. KW, dd.mmm -> 22.Jan)
* Stundenplan: Neue Option zum Einblenden einmaliger Termine im Dialog "Plan|Eigenschaften"
* Vertretungsplan: neues Schlüsselverzeichnis „Lehrerfehlgrunddetails“ , siehe "Fehlzeit"-Dialog für Lehrer, damit kann man für NRW noch feiner bestimmen, was KRANK bedeutet, also z.B. KRANK mit Attest usw.. (Das Verzeichnis können Sie unter Schlüsselverzeichnisse|Lehrerfehlgrunddetails" importieren "10_Lehrerfehlgrunddetails.keys")
* InfoServer: Teamfilter (Parameter "team=xyz" für HTML) für HTML Vertretungslisten 
* InfoServer: Neue Zeitangabe (Parameter "starttime=12:00") für HTML Vertretungslisten 
* Druck: Spalte "Vertretungslehrerart" eingefügt für Vertretungslisten
* HTML: Spalte "Vertretungslehrerart" eingefügt für Vertretungslisten
* Explorer: für mehrere Benutzer kann das Benutzerkonto automatisch erstellt werden. Dabei werden Kennung (falls noch nicht gesetzt) und Passwort erzeugt. Unter "Optionen" kann man einstellen, ob die Email als Kennung übernommen werden soll oder nicht. Für die Benutzer wird vermerkt, ob es sich um einen LEHRER, SCHÜLER, KLASSE oder GAST handelt. Die Passwörter sind exportierbar (Benutzerliste > Exportieren) und können so nach Excel oder für E-Mails übernommen werden.
* Explorer: Ansicht Benutzer: Passwörter werden nur mit JA/NEIN angezeigt.

## Verbesserte bzw. geänderte Funktion

## Fehlerkorrektur

* Stundenplan: Über das Plus/Minus eingestellte Termingröße wird beim Planwechsel beibehalten
* Stundenplan: Zugriffsverletzung bei "Plandatei aufräumen" behoben
* Vertretungsplan: Zugriffsverletzung im Servermodus beim Aufruf "Vertretungen|Vertretungen" behoben
* Vertretungsplan: zeitliche Begrenzung beim JSON-Export korrigiert 
* Vertretungsplan: Raumanzeige beim Zuweisen eines Vertretungsraumes 
* Vertretungsplan: werden Ereignisse im Kalender gelöscht, die mit Fehlzeiten gekoppelt sind, werden die Fehlzeiten gelöscht
* Vertretungsplan: korrekte Ausgabe der Uhrzeit beim Eintrag einer Fehlzeit über den Kalender
* Look: Funktionstasten F6,F7,F8 funktionieren wieder

### Prerelease 6.0.207 (11.02.2016) Dateiformat 6.0.154

!!! info "Hinweis"

    Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

## Fehlerkorrektur

* Vertretungsplan: Anrechenstunden für Zusatzunterricht werden bei den +AStd und -AStd berücksichtigt (Liste "Direkte Vertreter" und "Indirekte Vertreter")
* Vertretungsplan: Anrechenstunden für Zusatzunterricht werden nun korrekt in die "Vertretungsstatistik" übergeben
* Vertretungsplan: Funktionstasten F6,F7 und F8 für die Umschaltung Klasse-Lehrer-Raum funktionieren wieder
* Stundenplan: Aufsichtsplan | Blättern über Pfeile im Lehrerplan wieder möglich
* Stundenplan: In den Dialogfenstern für eine Veranstaltung bzw. einen Kalendereintrag kann man jetzt bei der Teilnehmerplanung Schüler nach Klasse filtern.
* Kursplan: In der Ansicht "Schüler" wird die Fachwahl jetzt auch automatisch geprüft.
* Server: Der Server benötigt ab jetzt für den Betrieb mit dem DaVinci InfoServer eine Lizenz. Klicken Sie zur Lizenzeingabe im DaVinci Server Control auf die Schaltfläche "Lizenz".
* Server: Fehlerbehebung bei der parallelen Verwendung von unterschiedlichen Plandateien im Mehrbenutzerbetrieb 

### Version 6.0.206 (09.02.2016) Dateiformat 6.0.153

!!! info "Hinweis"

    Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

## Fehlerkorrektur

* Server: Synchronisationsproblem beim Verschieben von Unterricht im Stundenplan behoben
* Vertretungsplan: Korrektur fehlender Vorziehoptionen in der Liste "Direkte Vertreter" 
* Vertretungsplan: Problem beim Emailversand (zb. Strato) behoben
* DRUCK: Ausdruck mehrerer Wochenpläne auf einer Seite wieder möglich (Wochenpläne: ein Lehrer-> drei Wochen //von-bis//, ein Raum-> drei Wochen //von-bis//, eine Klasse-> drei Wochen //von-bis//)  
