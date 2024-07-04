# Änderungen 2015

## Version 6.0.205 (19.12.2015) Dateiformat 6.0.152


!!! info "Hinweis"

    Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Neue Übersicht "Lehrer Arbeitstage" z.B. für die Statistik Nordrhein-Westfalen. Voraussetzung für die Nutzung dieser Übersicht ist das DaVinci-Modul Analytics. 

### Fehlerkorrektur

* Look: Anzahl der gezeigten Positionen korrigiert
* Look: über das Plus/Minus eingestellte Termingröße wird beim Planwechsel beibehalten
* Look: Drucken von Schülerplänen mit Fach-/Lehrelegende auf einer Seite wieder möglich
* Server: Synchronisationsproblem beim Eintragen von Fehlzeiten behoben
* Kursplan: Anzeige der Jahrgänge korrigiert

## Prerelease 6.0.204 (08.12.2015) Dateiformat 6.0.151

!!! info "Hinweis"

     Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* KALENDER: Neue Kalenderdateien mit den Schulferien und Feiertagen für 2016/2017 hinterlegt
* Stundenplan: im Stammdatenfenster "Lehrer" kann in der neuen Spalte "Geb.Datum" das Geburtsdatum eingetragen werden

### Fehlerkorrektur

* Vertretungsplan: Anzeige der Positionen beim Verschieben von Stunden korrigiert
* Vertretungsplan: HTML Export Tagesvertretung nach Klassen: Zusatzunterricht auch ausgegeben, wenn man nach Team filtert bei der Ausgabe
* Vertretungsplan: Funktionstasten F6, F7, F8 funktionieren wieder
* Vertretungsplan: Anrechenstunden für Zusatzunterricht werden wieder korrekt dem Lehrer zugeordnet
* Server: Synchronisationsproblem bei längerer Inaktivität in DaVinci behoben

## Version 6.0.203 (25.11.2015) Dateiformat 6.0.150

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Stundenplan: Sortierung im Stammdatenfenster nun auch nach "ID" möglich
* Vertretungsplan: Zusatzunterricht | Beim Erfassen wurde die Position mitaufgenommen 
* SAC-FW-APO-2014.js
 
### Fehlerkorrektur

* Server: bei Erstinstallation wird die Einstellung Backups erstellen automatisch gesetzt
* Server: Synchronisationsproblem beim Eintragen von Fehlzeiten (hier Klassenfehlzeiten) und serverseitige Fehlermeldungen behoben
* Stammdaten: Aktualisierungsproblem beim Löschen von Stammdaten
* Stundenplan: Konfliktanzeige bei Sperrung in Schienen korrigiert
* Stundenplan: Unterrichtsmatrix | alle Kurse eines Faches werden in der Matrix angezeigt
* Stundenplan: manuelle Verplanung | Lehrer ohne Raum korrigiert 
* Vertretungsplan: Fehler beim Eintragen von Fehlzeiten von Klassen behoben
* Vertretungsplan: fehlender Eintrag nach V-Regelung im Klassenplan 
* Vertretungsplan: Dialog "Vertretung entfällt" Ansicht modifiziert, Auswahlbereich des Vertretungsentfallgrundes vergrößert 
* Vertretungsplan: Vertretungen|Vertretungen per F2 Fehlzeit erfassen
* Vertretungsplan: Raumkonfklikt beim Vorziehen von Terminen
* Vertretungsplan: Fehlzeiten-Erfassen-Fenster - Vorbelegung beginnt/endet ganztätig korrigiert
* Vertretungsplan: Freigestellt | Ansicht "offene Vertretungen" Information wurde um das freigestellte Objekt erweitert
* Vertretungsplan: Zugriffsverletzung beim Aufruf offener Vertretungen korrigiert
* Vertretungsplan: Zugriffsverletztung beim Einsetzen von Vertretungslehrern auf eine Fehlstelle korrigiert 
* Vertretungsplan: "Freistellung" mit Uhrzeiten
* Vertretungsplan: Raum ändern inaktiv (wenn Zusatzunterricht im gleichen Raum stattfand)korrigiert
* Vertretungsplan: Anrechenstunden bei geblockten Klassen
* Look: Abgleich mit Look Uhrzeitanzeige der letzten Änderung aktuell 
* Druck: beim Anlegen von Zusatzunterricht wird der Lehrer in der Spalte VLehrer ausgegeben
* Druck: Titel von Mitteilungen wird in den Vertretungsplänen nur noch in der Spalte "Info" ausgegeben, vormals auch in Spalte "Art"
* Druck: jeder Plan auf neuer Seite Lehrerpläne|BBS Standard
* Druck: Gesamtplan Klassen 
* XML Export: Pausenaufsichten
* NIEDERSACHEN Statistikexport  

## Version 6.0.202 (02.11.2015) Dateiformat 6.0.149

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Fehlerkorrektur

* Vertretungsplan: Problem beim Erfassen einer Lehrerfehlzeit mit Aufsichtsfehlzeit gelöst
* Vertretungsplan: eingetragener Zusatzunterricht kann wieder bearbeitet werden 
* Vertretungsplan: Verschieben von Doppelstd. - Ausgabe der Positionsnummern fehlerhaft 
* Vertretungsplan: Schraffur bei "Von" und "Auf"-verschoben
* Vertretungsplan: Änderung bearbeiten" bei erfassten Fehlzeiten  
* Vertretungsplan: Fehlzeiten-Erfassen-Fenster, Haken vor "Nicht öffentlich" muss mit jeder neuen Fehlzeitenerfassung bei Bedarf neu gesetzt werden
* Vertretungsplan: Vertreter vorziehen, Haken vor "Sollen Fehlstellen für die Klasse(n) erzeugt werden" muss mit jeder neuen Vorziehoption bei Bedarf neu gesetzt werden
* Druck: Zusatzunterricht erscheint wieder korrekt im Ausdruck 

## Version 6.0.201 (21.10.2015) Dateiformat 6.0.148

### Fehlerkorrektur

* Look: Anzeige "Lehrer jetzt", "Klassen jetzt", "Räume jetzt" korrigiert 

## Version 6.0.200 (20.10.2015) Dateiformat 6.0.148

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Vertretungsplan: Änderungen im Stundenplan bei bereits eingetragener Fehlzeit eines Kollegen, können mit dem Befehl AENDERUNGEN NEU ERSTELLEN in die Liste der offenen Vertretungen aufgenommen werden
* Vertretungsplan: Plananzeige beim Wechsel von Stundenplan zu Vertretungsplan wird übernommen (Auswahl)
* DRUCK: Druckformate - im Auswahlfenster wird im Aufklappmenü immer alphabetisch sortiert, man kann so durch den Namen des Druckformates beeinflussen, welches zuerst angezeigt wird
* DRUCK: Ausdruck mehrerer Pläne auf einer Seite wieder möglich
* DRUCK: beim Drucken sämtlicher Pläne ist es wieder möglich die Zusatzinformationen (z. B. Legende der Fächer und Fachlehrer) unter den Plan zu drucken
* DRUCK: Aufsichtspläne - verwendet optional Farben aus dem Plan, hier die Lehrerfarben aus dem Stammdatenfester
* KALENDER: Neue Option in den DaVinci-OPTIONEN>KALENDER für die Synchronisation mit dem Google-Kalender, WICHTIG wenn mehrere Kollegen auf einen DaVinci Look Rechner zugreifen dürfen die Google Anmeldedaten nicht gespeichert werden, dies muss so eingestellt werden
* HTML-Export: Im Dialogfenster "Eigenschaften" begrenzen Sie mit der neuen Option  "x Unterrichtstage inkl. heute publizieren" Sie die Anzahl der Unterrichtstage, für die Änderungen publiziert werden. D.h. eine freigegebene Änderung wird nur dann publiziert, wenn sie innerhalb dieses Zeitraums liegt.
* HTML-Export: Exportformate - im Auswahlfenster wird im Aufklappmenü immer alphabetisch sortiert, man kann so durch den Namen des Formates beeinflussen, welches zuerst angezeigt wird
 
### Verbesserte bzw. geänderte Funktion

* Performanz des DaVinci InfoServer verbessert. 

### Fehlerkorrektur

* Stundenplan: Problem beim Setzen von Perioden-Kalenderwochen im "Veranstaltung Bearbeiten"-Fenster behoben
* Stundenplan: "Termin teilen" ist nun auch möglich bei klassenübergreifendem Block
* Stundenplan: Funktionstaste CTRL-F9 (Zeitpräferenz löschen) und F11 (Neue Zeitpräferenz) funktionieren wieder
* Stundenplan: Räume aus Terminen wurden beim Setzen in Blockelementen entfernt => korrigiert
* Stundenplan: Unverplant-Schaltfläche für Masterplaner (nur Teamveranstaltungen) bleibt an der gewählten Position
* Stundenplan: Anzeige der Differenz in Lehrer Soll Konto und im Zusatzfenster passende Lehrer stimmen wieder überein
* Stundenplan: Veranstaltungen befristen, zugewiesene Periode wird bei einer Befristung (hier mit Hilfe der Bereichsmarkierung) nicht mehr herausgelöscht
* Stundenplan: Aktualisierungsproblem in Raumplananzeige - bitte führen Sie einmalig über "Extras|Plandatei aufräumen" aus
* Stundenplan: Aufsichten in Lehrerplänen außerhalb von Pausen können optional mit oder ohne Uhrzeiten ausgegeben werden (DaVinci-OPTIONEN>Stundenplan)
* Vertretungsplan: Raumkonflikte, die in der Vertretungsregelung angezeigt wurden, obwohl es diese nicht gab, wurden korrigiert
* Vertretungsplan: Zusatzunterricht kann jetzt auch vertreten werden.
* Vertretungsplan: Anzeigefehler beim Stunden verschieben
* Vertretungsplan: Lehrer/Raumfehlzeit in Vertretungsregelung mit Stillarbeit (Teilnehmer haben nicht frei)
* Vertretungsplan: Lehrerfreistellung in Block - "Weitere Termine dieses Lehrers im Block analog vertreten" wurde korrigiert
* Kursplan: Ansicht "Schüler" - Bereichsmarkierung wieder möglich 
* Kursplan: Problem bei der Anzeige der Schülerzahlen der Kurse unter Kursplan|Fachwahl behoben
* Kursplan: Problem bei der Anzeige von Kursen ohne Kursnummer im Schülerplan behoben
* DRUCK: Tagesvertretung nach Klassen, Spalte VRaum wird gefüllt
* DRUCK: Korrketur, wenn man als Anzeigefarbe "keine" auswählt
* DRUCK: geänderte Pläne ab korrigiert
* DRUCK: Pläne auf einer Seite drucken
* DRUCK: Bemerkungen werden über dem Plan oder den Listen ausgegeben
* HTML-Export: Lehrerbezeichnung in Überschriften und Zellen über Seite|Bezeichnung

## Version 6.0.199 (24.09.2015) Dateiformat 6.0.141

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Stundenplan: Beim Vertauschen von Stunden wird ggf. auf "Fach mehrfach am Tag" hingewiesen.
* Stundenplan: Für die automatische Erzeugung der Blockbezeichnung kann unter "Optionen" kann jetzt als Block-Präfix "Klasse" oder "Stufe" gewählt werden (bisher nur "Klasse").
* Vertretungsplan: "Prioritäten" bei V-Lehrern - Kombinationen "Klasse, Fach"
* Kursplan: neue Option: Abweichung vom Originalwert einblenden (DaVinci Optionen|Kursplan)
* Kursplan: neue Option: wahl ob der Blockpräfix aus KLASSE oder STUFE bestehen soll 
* Druck: Veranstaltungsliste Lehrer| Zeitkonteninformationen drucken (Deputat, Entlastung, Zusätzlich)
* Druck: Lehrervertretungen | neue Option im Druckformat "Klassenausfall Termine" anzeigen

### Verbesserte bzw. geänderte Funktion

* Anzeigegeschwindigkeit optimiert bei der Plananzeige für Pläne mit Zeitschienen 

### Fehlerkorrektur

* Allgemein: Optionen|Einstellungen - Trennung vom Server 
* Stundenplan: Stundenverlegung nicht möglich wegen Zeitkonflikten - Konfliktanzeige korrigiert
* Stundenplan: Stundentauschangebot korrigiert
* Stundenplan: Tauschen zweier Veranstaltungen im Plan - Warnung "Fach mehrfach am Tag"
* Stundenplan: Lehrerauswahl über Zusatzfenster passende Lehrer bei Veranstaltung und Terminliste gleich 
* Stundenplan: Stundenplan:Zeitpräferenz löschen per STRG+F9
* Stundenplan: Stundentafeln - Spalten ausblenden führte zu Fehlermeldung
* Stundenplan: Verplante Stunden | Schienen wieder angezeigt
* Stundenplan: Unterrichtsmatrix| im Kursmodus Lehrerzuweisung korrigiert
* Stundenplan: Veranstaltung Bearbeiten-Fenster | Raumbelegung innerhalb eines Blockes wird angezeigt
* Stundenplan: Termine können auch aus der Terminliste per Drag and Drop in den Plan gezogen werden.
* Stundenplan: Planvorbereitungsassistent - Datenübernahme - Blöcke korrigiert
* KALENDER: Kalendereintraganzeige ändern von "alle" auf "nur Teilnehmer" wird dauerhaft gespeichert
* STAMMDATEN: Stammdaten|Klassen|Zeitrahmen auch in daVinci SMART sichtbar
* Vertretungsplan: Zusatzunterricht - Raum wird korrekt als belegter Raum ausgegeben
* Vertretungsplan: Fehlzeit Lehrer - nicht alle zu vertretenden Elemente wurden im Fenster "Vertretungen" angezeigt
* Vertretungsplan: Änderungen mitteilen, Datumsausgabe korrigiert
* Vertretungsplan: Klassen-/ Lehrerfehlzeit, bei eingetragener Klassenfehlzeit wird der mitfahrende Lehrer als "Fehlend" ausgegeben
* Vertretungsplan: Anrechenstunden bei zu vertretenen Doppelstunden, die über eine Pausenzeit (Bsp. 5min) gehen
* Vertretungsplan: falsche Zeitangabe bei Fehlzeit 2. Teil einer Doppelstd. wenn zw. Doppelstd. 5 min Pause 
* Kursplan: Anzeige von Alternativkursen die im selben Block liegen
* Kursplan: Löschen von Kursen führte zum Leeren der Datei: Bitte einmal Plandatei aufräumen wählen
* Kursplan: abgewählte Fächer werden in Schülerplänen trotzdem angezeigt => Korrektur über Extras|Plandatei aufräumen 
* HTML-Export: Aufsichtsänderungen | Ausgabe der Pos.nr. im HTML-Export  
* Export: Export Statistik NRW BBS korrigiert
* Export: SDTF: im P1-Datensatz wird das Geburtsdatum exportiert und auch importiert 
* Druck: Druckformat "Vertretungslehrerliste" Bezeichnung "Lehrer" kann angepasst werden
* Druck: Ausdruck "Schülerpläne", Schüler alter Jahrgänge werden nicht mehr zur Auswahl gestellt 
* Druck: Druck ganztägiger Mitteilungen
* Server: die Backupfunktion im daVinci-Server-Control wurde korrigiert (Systemsteuerung|daVinci-Server|Backup)

## Version 6.0.198 (31.07.2015) Dateiformat 6.0.139

### Fehlerkorrektur

* Stundenplan: Problem beim Aufruf des Punkts Drucken|Typ Lehrerpläne|"ausgewähltes Druckformat" behoben
* Stundenplan: Problem beim rückwärts Blättern (Klassen,Lehrer...)über die Pfeiltasten in der Veranstaltungsliste behoben
* Stundenplan: Beim Export der Unterrichtsmatrix werden alle Zeilen nach Excel übergeben
* Stundenplan: Unter Stundenplan|Unterrichtsmatrix werden die Stundenzahlen für Blockungen angezeigt.
* Kursplan: Problem beim Schüler löschen aus Kursplan|Schüler behoben
* Kursplan: Doppelte Anzeige neuangelegter Schüler unter Kursplan|Schüler behoben
* Kursplan: Die Kursteilnehmeranzahl und Konfliktanzeige unter Kursplan|Fachwahl wurde korrigiert
* KALENDER: Ereignisnotizen  bleiben beim Serverneustart erhalten

## Version 6.0.196 (17.07.2015) Dateiformat 6.0.139

### Neue Funktionen

* Stundenplan: Unterrichtsmatrix | optional für die Oberstufe kann man sich die einzelnen Kurse anzeigen lassen 
* Kursplan: neue Option unter  OPTION|Kursplan Schülerfenster|Anzahl der Kursspalten 
* Kursplan: neue Schüler-Blöcke-Matrix unter Kursplan|Blöcke

### Fehlerkorrektur

* Stundenplan: für daVinci SMART Perioden in der Veranstaltungsliste eingeblendet    
* Stundenplan: Problem beim Löschen von Aufsichten inaktiver Lehrer behoben
* Stundenplan: Fehlermeldung beim "Raum entfernen" aus der Veranstaltungsliste korrigiert
* Stundenplan: Unterrichtsmatrix| Klassen/Fächer - gelbe Markierung (wenn kein Lehrer zugewiesen), wird wieder angezeigt (nicht in der Einstellung Kurse anzeigen)
* Kursplan: Konflikte im Blockfenster durch fehlenden Eintrag der Stundenanzahl beim Kurs korrigiert
* Kursplan: Sortierung Fachwahlen (Grundkurse, die keinen Fachstatus zugewiesen bekommen haben, erscheinen vor den Grundkursen mit Fachstatus)
* Kursplan: Aktualisierungsproblem | Kurs aus Block entfernt, passender Block für Kurs wird wieder angezeigt
* Kursplan: Sperrungen in Klassenplänen werden in unter Kursplan|Stundenplan in den Schülerplänen angezeigt.
* Kursplan: Kursplan|Blöcke: die angezeigten passenden Blöcke bleiben auch beim Ein- und Ausblenden von Spalten korrekt.
* Import/Export: Aufruf für den JSON-Export korrigiert
* DaVinci Server: Aktualisierungsproblem behoben
  
## Prerelease Version 6.0.195 (02.07.2015) Dateiformat 6.0.139

### Fehlerkorrektur

* DaVinci Server: Problem beim Speichern von Änderungen und Lehrerzeitkonten im Enterprise-Betrieb behoben
* DaVinci Kursplan: Arbeitet mit dem "Jahrgang" anstatt der Klasse, d.h. die Klassen 12A, 12B, 12C werden als Jahrgang 12 (Stufe=12) betrachtet. Siehe dazu neues DaVinci Kursplan Benutzerhandbuch.
* DaVinci Kursplan: Überarbeitete Ansichten und überareitete Automatik, siehe dazu neues DaVinci Kursplan Benutzerhandbuch.
* Stundenplan:Problem in der Unterrichtsmatrix beim Entfernen von Lehrern usw. behoben.

## Version 6.0.194 (13.05.2015) Dateiformat 6.0.133

### Neue Funktionen

* Stundenplan: Stunden einer integrierten Klasse werden optisch im Plan mit einem i gekennzeichnet 
* Stundenplan: Eingabe der Fachkategorie in Stammdaten "Stundentafel"
* Stundenplan: Aufsichtsbereichsplan |Neuer Befehl BEARBEITEN > Neue Aufsichtstermine erzeugen
* Stundenplan: Veranstaltungen befristen, Befristung in der Bildschirmansicht aus Sicht aller Wochen sichtbar 
* Stundenplan: In der Unterrichtsmatrix werden für die Oberstufe auch die einzelnen Kurse angezeigt  
* Stundenplan: Neue Elemente fügen Sie der Statistikdatei auf der die Übersichten|Unterricht und Unterrichtsstatistik basieren hinzu, indem Sie die Plandateien nacheinander in der jeweiligen Ansicht öffnen und auf "Sichern" gehen 
* Vertretungsplan: Neuer Befehl und Status GESCHLOSSEN für offene Vertretungen, diese werden nicht mehr farblich markiert in der Liste der offenen Vertretungen angezeigt
* Vertretungsplan: Vertretungsplan|Fehlzeiten: in der Liste gibt es eine neue Spalte "Öffentlicht" die anzeigt, ob eine Fehlzeit "Öffentlich" oder "Nicht öffentlich" ist 
+ Vertretungsplan: eine nicht öffentliche Fehlzeit wird in der Änderungsliste in der Spalte Status als "nicht öffentliche Fehlzeit" markiert. Siehe dazu auch Änderungen in der 6.0.193.
* Kursplan: Schüleranzahl wird im Bereich "Kursplan|Schüler" ausgegeben
* Kursplan: "Kursplan|Schüler" über Entf können einzelne Fachwahlen bzw. Kurse beim Schüler gelöscht werden
* Kursplan: neue Option im Dalog "Automatik starten", mit der man sagen kann, ob man die Kursteilnehmerzahlen (lt. Eintragungen unter Plan-Eigenschaften|Kursplan) beachtet werden sollen oder nicht
* Kursplan: beim Wechsel "Kursplan|Fachwahl" zu "Kursplan|Schüler" - ist im Schülerbereich der aktive Schüler markiert
* Kursplan: Bereich "Blöcke"|passende Kurse" - Spalte "Unterrichtsart" hinzugefügt
* Kursplan: Kursplan -> Bereich "Blöcke|passende Kurse" bei der Eingabe des Faches/Kurskürzel springt der Cursor zum gewünschten Kurs in der Liste der passenden Kurse
* Ausdruck: Tagesvertretungen: neue Option "Doppel-/Blockstunden je Position wiederholen"
 
### Fehlerkorrektur

* Stundenplan: Anlegen einmaliger ganztägiger Sperrungen
* Stundenplan: Anzeige der Wochentage einschränken auf einen Wochentag
* Stundenplan: nicht ganztägige periodische Sperrungen werden korrekt ausgegeben
* Stundenplan: Extras|Terminzeiten anpassen
* Stundenplan: ein in den Stammdaten einem Lehrer zugewiesener Raum, wird bei der Zuweisung des Lehrers zu einem Fach in der Veranstaltungsliste der Klasse in die Splate Raum übernommen
* Stundenplan: "Veranstaltungen fortschreiben", aktuell zugewiesene Blöcke werden mit fortgeschrieben
* Stundenplan: Passende Lehrer | "Lehrer entfernen" aus Veranstaltungsliste funktioniert  
* Stundenplan: Aktualisierungsproblem im Zusatzfenster "passende Lehrer/Räume" bei Planwechsel behoben
* Stundenplan: Aktualisierungsproblem Zusatzfenster "passende Räume" beim Entfernen eines Raumes behoben
* Stundenplan: Aufsichtsbereichsplanung | Pausenzeiten abweichend vom Hauptzeitrahmen, Darstellung korrigiert
* Stundenplan: Zusatzpläne: Zeigten fälschlicherweise Positionskonflikte/Passende Termin an wie im Hauptfenster 
* Stundenplan: Plananzeige: Wechsel "Übersichtsplan" zu "Plan und Liste" korrigiert
* Stundenplan: Öffnen einer Plandatei.davinci.zip Datei  
* Stundenplan: Wechsel von "Jahresverteilung" zu "Stundenplan" - Ansicht "Veranstaltungsliste" Form der Listenansicht wird nicht mehr übernommen
* Stundenplan: In den Konferenzlisten (Fachkonferenz, Klassenkonferenz) kann jeweils nach Fach, Klasse und Team gefiltert werden.
* Stundenplan: einen über die Veranstaltungsliste zugewiesenen Lehrer kann man über die Schaltfläche "Entfernen" im Fenster "Passende Lehrer" entfernen.
* Stundenplan: das SchülerIst bei duplizierten miteinander geblockten, zeitgleichen Terminen wird korrekt gezählt
* Stundenplan: werden zwei Lehrer in der Veranstaltungsliste zugewiesen, werden diese auch in den Plan gesetzt
* Stundenplan: Im Plan markierter Abschnitt wird als zeitliche Vorbelegung mit ins Sperrungsfenster(F4) übernommen. Ausnahme: zuvor wurde der ganztägig-Haken gesetzt.
* Stundenplan: Eine stundenweise Sperrung ist möglich.
* Stundenplan: Ausblenden von Spalten im den Druckformat für "Lehrer-Zeitkonto" ist möglich.
* Stundenplan: Fehler beim bei "Export|Statistikdaten exportieren|Statistik Hessen (LUSD) exportieren" korrigiert
* Stundenplan: Fehler bei der Datenübernahme von Dateien mit Oberstufendaten aus Version 5, wenn sich ein + hinter der Kursbezeichnung befindet, wählen Sie bitte einmal Plandatei aufräumen
* Stundenplan: in der Jahresverteilung|Lehrer wurden die angezeigten Wochenwerte korrigiert
* Stundenplan: Unter Übersichten|Unterricht und Unterrichtsstatistik werden die ein- oder ausgeblendeten Spalten gespeichert.
* Stundenplan: Lehrbefähigung, Einschränkung auf Klassenstufe hat Auswirkung auf Filterung "Passende Lehrer|nur Fachlehrer
* Stundenplan: Export|Statistik|WinLD Ausgabe des Wiederholungsfaktors korrigiert
* Stundenplan: Unter Übersichten|Unterricht und Unterrichtsstatistik wurden die Filtermöglichkeiten überarbeitet, bitte beachten Sie, dass Sie vor neuen Filterungen erst "Zurücksetzen" wählen müssten
* Stundenplan: Fächer mit dem Attribut "Präsenz" bei Stammdaten|Fächer|Vertretung werden jetzt immer in die statistische Berechnung einbezogen, sollte dies nicht so sein stellen Sie "nicht statistikrelevant" bei Stammdaten|Fächer|Details ein
* Vertretungsplan: Vertretung bei Stunden die aus mehreren Positionen bestehen|Stunden teilen 
* Vertretungsplan: freigestellter Lehrer wird als direkter Vertreter für 1 Stunde angeboten, auch wenn seine Freistellung aus 2 x 0,5 h besteht
* Vertretungsplan: unter Vertretungen|Fehlzeiten aktualisiert sich in der Ansicht "Plan und Zeitplan" der Zeitplan beim Aufruf einer neuen Planart
* Vertretungsplan: beim Fachtausch wird das ursprüngliche Fach der Veranstaltung in einer Klammer gezeigt
* Vertretungsplan: Freistellung eines Lehrers erzeugt, wenn die Freistellung vertreten werden soll, nur eine Zeile in der Vertretungserstellung
* Vertretungsplan: Konfliktanzeige bei Ersatzräumen beim Vorziehen von Unterricht korrigiert
* Vertretungsplan: fehlende Aufsicht wird wieder gelb in der Liste der offenen Vertretungen angezeigt
* Vertretungsplan: Änderung der Anzeige bei 2 Lehrer in einer Klasse) | Anzeige bei Fehlzeit einer Lehrkraft- es wird der fehlende Lehrer mit angezeigt
* Vertretungsplan: Vertretungseinstellungen|Vertretungseinschränkungen von 1-10          
* Vertretungsplan: Fachänderungen - Anzeige im Plan und Ausdruck Ursprungsfach wird geklammert 
* Vertretungsplan: Vertretungsregelung beachtet unterschiedliche Zeitrahmen bei der Anzeige der direkten Vertreter  
* Vertretungsplan: "Raum ändern" - Auflistung/Reihenfolge der Räume wie im Stammdatenfenster sortiert 
* Vertretungsplan: "Fach ändern" über rechte Maustaste
* Vertretungsplan: Vertretungsplan|Anrechnungen manuell erfasste Anrechenstunden für einen Lehrer für einen Monat, werden in der Ansicht der möglichen Vertreter korrekt angegeben
* Vertretungsplan: sind einem Unterricht zwei Lehrer zugeordnet, diese fehlen beide, können auch zwei Vertretungslehrer zugeordnet werden
* Vertretungsplan: eine neue eingetragene Fehlzeit hebt keine Terminverschiebung auf
* Vertretungsplan: "Raum ändern" - es werden nicht nur verfügbare Räume angezeigt
* Vertretungsplan: Für Raumvertretungen werden vorgezogenen Räume belegt gezeigt.
* Vertretungsplan: Vertretungsplan|Stundenplan: Verschieben in eine spätere Woche über Markieren|Woche wechseln|Verschieben 
* Vertretungsplan: Termin teilen bei doppelstündiger Raumfehlzeit
* Vertretungsplan: Vorziehen in Fehlstellen
* Vertretungsplan: ein Lehrer, der zum Zeitpunkt der Vertretung Zusatzunterricht hat, wird als "Indirekter Vertreter"  mit der Art "Übernehmen" angeboten.
* Vertretungsplan: Vertretungsplan|Vertretungen: Bei Wechsel auf einen andere möglichen Vertreterslehrer in der Liste, werden die entsprechenden Stundenpläne der Vertreter synchron angezeigt
* Vertretungsplan: Mitteilungen lt. Vertretungsregelung werden auch in Schülerplänen angezeigt
* Look: Raum-Ressourcen: zugewiesene Ressource kann in Liste der Ressourcenliste entfernt werden
* Look: Raum-Ressource: Zugewiesene Ressource ist ggf. als (nicht) verfügbar gekennzeichnet
* KALENDER: Aufruf neues ganztägiges Ereignis: Haken bei ganztägig ist gesetzt
* KALENDER: Löschen einer Veranstaltung, die im Kalender angelegt wurde, korrigiert
* Ressourcenplan: Beim Neuanlegen von Exemplaren unter Stammdaten|Ressourcen wird die Bezeichnung übernommen.
* Kursplan: "Plandatei aufräumen" korrigiert, es wurden bisher Kurszuweisungen teilweise gelöscht
* Kursplan: Filterung nach Spaltenköpfen im Bereich "Kursplan|Kurse" bleibt erhalten
* Kursplan: RLP-FW-APO-BGY-2010 und RLP-FW-APO-2010 korrigiert Wahl Sozialkunde, Geschichte oder Erdkunde als LK richtige Kombination mit den GK wird geprüft
* Ausdruck: Einzelplan Lehrer| Uhrzeit bei Aufsichten wird mit ausgegeben
* Ausdruck: für Lehrerpläne wird mit der Option !Seite|Nächster Plan auf neuer Seite" ein Seitenumbruch eingefügt
* Ausdruck: Klassenvertretungen: bei gleichzeitig fehlendem Lehrer und Klasse werden die Positionen nicht ausgegeben
* Ausdruck: Tagesvertretung nach Klassen, Sortierung der Klassen beachtet die angegebene Reihenfolge in den Stammdaten
* Ausdruck: Tagesvertretungen in der Spalte V-Lehrer wird der V-Lehrer ausgegeben
* Ausdruck: Gesamtplan Räume|Originaltermine bei Änderungen nicht anzeigen korrigiert 
* HTML Export: Blättern in Klassen-, Lehrer-, Raumplänen möglich
* HTML Export: Klassenpläne können beim Export in einen gesonderten Unterordner abgelegt werden
* HTML Export: Titel einer Veranstaltung wird mit ausgegeben
* HTML Export: Sortierung Tagesvertretung nach Lehrern Positionen mit Zusatzunterricht werden nach Lehrer Kürzel mitsortiert
* HTML Export: einmalige Sperrungen im HTML EXPORT werden in der betreffenden Kalenderwoche ausgegeben
* HTML Export: im Dialogfenster werden die Werte "Von" und "Bis" nach dem Schließen des Dialogfensters  gespeichert 
* HTML Export: Beim Export der Raumpläne kann die Überschrift "Kürzel und Bezeichnung" gewählt werden
* Stammdaten: Leerzeichen vor zum Beispiel Klassenkürzeln werden mitgespeichert. Die Sortierung im Druck oder HTML-Export erfolgt jetzt aufgrund der Stammdatensortierung.
* Stammdaten: Stammdatenfenster - Sortierung auch nach Bezeichnung
* Allgemein: Bei einigen Dateien wurde eine Zugriffsverletzung beim Aufräumen des Planes gezeigt, dieses Problem wurde behoben.

## Pre-Release 6.0.193 (23.04.2015) Dateiformat 6.0.133
 
### Neue Funktionen

* Vertretungsplan: Unter Vertretungen|Fehlzeiten können Sie in der Ansicht "Liste" mehrere Fehlzeiten markieren und über Befehle im Kontextmenü (Rechtsklick) gleichzeitig auf "öffentliche Fehlzeit" oder "nicht öffentliche Fehlzeit" setzen.

### Fehlerkorrektur
 
* Ausdruck: Die Reihenfolge der Inhalte der "Veranstaltungslister Lehrer, Klassen, Fächer, Räume" richtet sich nach der Sortierung der Stammdaten und der Sortierung der Veranstaltungsliste über die Schaltfläche "Sortieren"
* HTML-Export: ganztägigen Mitteilungen werden nur über der Liste ausgegeben (Beispiel Tagesvertretungen nach Klassen/Stunden/Lehrern)
* Vertretungsplan: Mehrfachauflistung von Vertretern (direkt oder indirekt) korrigiert
* Vertretungsplan: Nicht öffentliche Änderungen (nicht öffentliche Fehlzeit) sind in der Änderungsliste sichtbar

## Pre-Release 6.0.192 (22.04.2015) Dateiformat 6.0.133
 
> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* ALLGEMEIN: Plan>Eigenschaften>Stundenplan>Wochen immer anzeigen --> über diese Einstellung können Sie im Planfenster das Periodenkürzel mit Kalenderwochen oder nur das Periodenkürzel ausgegeben lassen, dies ist eine planspezifische und nicht benutzerspezifische Einstellung
* ALLGEMEIN: Höhe der Titelzelle im Planfenster kann verändert werden --> unter Optionen|Termine|Padding-Wert, dieser bestimmt die Höhe der Titelzelle (somit kann Datumsanzeige im Vertretungsplan wieder angezeigt werden. wenn eine Aufsicht vor der 1.Stunde liegt )
* Server: unter Optionen|Einstellungen für daVinci und für Look können Sie wählen, ob die Trennung vom Server bestätigt werden soll
* Stundenplan: Stundenplan|Aufsichtsplan: Entfernen eines Aufsichtlehrers über Backspace Taste
* Stundenplan: Plan fixieren für mehrere Pläne
* Stundenplan: Wenn einer Veranstaltung ein Lehrer über "passende Lehrer" zugewiesen wird, ist "Hinzufügen" und "Zuweisen" aktiv, gibt es bereits einen Lehrer, wird nur noch die Schaltfläche "Hinzufügen" aktiv

### Fehlerkorrektur

* ALLGEMEIN: in Look und DaVinci können Pläne wie folgt geöffnet werden: F6=Klassenplan, F7=Lehrerplan, F8=Raumplan
* Ausdruck: Druckformat Lehrer-Zeitkonto -> es kann der Langname des Lehrers als Überschrift gewählt werden
* Stundenplan: Termin teilen bei Stunden die über eine Pause gehen, Dauer korrigiert
* Stundenplan: Stundenplan|Übersichten|Veranstaltungen Alle Veranstaltungen löschen Fehlermeldung korrigiert
* Stundenplan: Veranstaltungsbefristung aufheben
* Stundenplan: Verplanung zurücksetzen
* Stundenplan: Zeitrahmen -> farbige Trennlinien werden bei unterteilten "Einheiten je Position" im Planfenster korrekt angezeigt
* Stundenplan: Anzeige "einmaliger" Sperrungen in Planansicht korrigiert
* Stundenplan: Konferenzlisten -> Filterung korrigiert 
* Vertretungsplan: Fehlzeiteneintrag über den Kalender beim Anlegen von Ereignissen   
* Vertretungsplan: Vertretungsplan|Fehlzeiten Ansicht "Liste"; Button Neue Fehlzeit aktiv
* Vertretungsplan: Termine Vertauschen korrigiert
* Vertretungsplan: Anzeige einer Kurs-Fehlzeit, die ganztägig erfasst wurde, korrigiert
* Vertretungsplan: "Raum/Lehrer vertauschen" korrigiert
* Kursplan: Blockungsautomatik korrigiert
* Ausdruck: Uhrzeit "am" und "pm" beachtet
* InfoServer: Aktualisierung kann über das InfoServer-Control in der Systemsteuerung erfolgen
* KALENDER: Beim Anlegen eines neuen Ereignis wird nun das "Endet"-Datum automatisch auf "Beginnt"-Datum hochgesetzt 
* KALENDER: Teilnehmer eines Ereignisses entfernen| Zeile löschen aktiviert 

## Version 6.0.191 (31.03.2015) Dateiformat 6.0.132

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Allgemein: Konferenzlisten gibt es auch aus Klassensicht
* KALENDER: Wird ein unterrichtsfreier Tag im Kalender erfasst für den bereits Vertretungsinformationen existieren, werden die Konflikte im Ereignisfenster gezeigt.
* Vertretungsplan: Für Zusatzunterricht kann jetzt auch eine "Info" erfasst werden
* Stundenplan: Beim Aufruf von "zwei Pläne" oder "zwei Listen" werden immer die zuvor gewählte Pläne angezeigt (z.B. Klasse und Lehrer usw.)
* Stundenplan: unter Stundenplan|Stammdaten|Klassen, Lehrer, Räume....|Bearbeiten|Zeitpräferenzen löschen können jetzt mehrere oder alle Zeitpräferenzen in einem Arbeitsgang gelöscht werden
* Stundenplan: Automatik|Verplanung zurücksetzen kann jetzt auch teamweise eingesetzt werden

### Fehlerkorrektur

* Export: Beim Export im xml Format sind jetzt wieder mit die Filter verfügbar.
* Server: Speicheroptimierung und Geschwindigkeitsverbesserung im Enterprise-Betrieb
* Allgemein: "Eigenschaft|Bemerkung" kann im lokalen oder im Server-Betrieb beim Öffnen der Datei gezeigt werden
* KALENDER: Meldung für "Mein Kalender" korrigiert (Stammdaten|Lehrer|Benutzername)
* Vertretungsplan: Beim Eintrag von Fehlzeiten im Zeitstrahl kann die F2-Taste verwendet werden
* Vertretungsplan: Filterung nach dem Team bleibt auf den Karten indirekte Vertreter/direkter Vertreter gespeichert
* Vertretungsplan: Beim Einsatz von Vertretungen werden auch nicht ganzzahlige Anrechenstunden korrekt berücksichtigt
* Vertretungsplan: Aufsicht entfallen lassen auch ohne "Vertretungsentfallgrund" möglich
* Vertretungsplan: Vertretungslehrer für eine Aufsicht fehlt => Aufsicht wird wieder als offen angezeigt
* Vertretungsplan: beim Vorziehen von Unterricht, wird beim Ersatzraum auch eine eventuelle Raumfehlzeit abgeprüft
* Stundenplan: in einigen Dateien gab es Abweichungen unter Stundenplan|Veranstaltungslist in der Spalte Ist/W. Die Aktion Extras|Plan aufräumen korrigiert die Anzeige.
* Stundenplan: Anzeige periodischer Veranstaltungen in der Ansicht alle Wochen
* Stundenplan: Wochenmittel bei der faktorbezogenen Verrechnungsart 
* Ausdruck: Druckformat Einzelplan Lehrer schmal 3 zeilig lässt sich wieder dublizieren
* Ausdruck: Bezeichnung des fehlenden Lehrers in den Druckformaten Tagesvertretungen

## Version 6.0.190 (26.03.2015) Dateiformat 6.0.131

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Wenn unter "Plan|Eigenschaften|Bemerkung" die Option "Bemerkung beim Öffnen der Datei anzeigen" markiert ist, wird diese Bemerkung nun auch entsprechend angezeigt.
* Server: Speicheroptimierung und Geschwindigkeitsverbesserung im Enterprise-Betrieb
* Stundenplan: Verplanung zurücksetzen neue Funktion: Aufsichtslehrer verplanen zurücksetzen
* Explorer: Beim Anlegen von neuen Planordnern kann ein Mandant hinzugefügt werden
* KALENDER: Neue Kalenderdateien mit den Schulferien und Feiertagen für 2015/2016 hinterlegt

### Fehlerkorrektur

* Korrekturen beim der HTML-Ausgabe (Layout für local-HTML-Vorlagen Schriftart, Schriftgröße, Schriftschnitt)
* Stundenplan: Perioden löschen korrigiert
* Stundenplan: Planaktion|Plan fixieren nur für bereits gesetzte Termine 
* Stundenplan: Räume in Blockungen ersetzen
* Stundenplan: Jahresverteilung: Summe geplant/J
* Vertretungsplan: Fehlgrund ändern bei bestehender Fehlzeit; Übernehmen Schaltfläche wieder aktiv
* Vertretungsplan: Vertretung entfällt korrigiert
* Vertretungsplan: Statistik negative Anrechenstunden korrigiert
* Vertretungsplan: Schaltfläche „Neue Fehlzeit“ (in der Fehlzeiten Ansicht: Liste und Zeitplan, Zeitplan und Liste) wieder aktiv
* Look: Farbe der Fehlgründe wird auch in Look angezeigt
* Look: Sammlung Bearbeiten korrigiert
* Look: Anzeige Lehrer/Klassen jetzt Schriftgröße; Fettanzeige; Spaltenanzahl können eingestellt werden
* Look: Vertretungsplan|Höhe der Betroffenenzeile passt sich automatisch beim Vergrößern der Schrift an
* Look: Wenn die Optionen durch ein Passwort geschützt sind, wird das Passwort auch über die Ansicht Beginn|daVinciOptionen abgefragt
* Look: Eingabe in den Dateieigenschaften „Alle Fehlgründe als abwesend anzeigen“ gilt nur für Fehlgründe in Look 
* Look: Filterung nach Teams in Look korrigiert
* Look: Die Info "geändert von" wird auch in Look angezeigt 
* Look: Wechsel von Lehrer (oder Klassen) jetzt in einen Lehrerplan | Wechsel Kalenderwoche (Auswahl der KW bleibt erhalten)    
* Look: das Programm kann auf einem Rechner mehrmals geöffnet werden
* Look: Akualisierungsproblem | Räume jetzt oder Klassen jetzt 
* Look: Akualisierungsproblem | Anzeige gebuchter Ressourcen
* Explorer: Mehrfachmarkierung von Benutzern möglich
* Ausdruck: Termine|Blockungen zusammenfassen Darstellung korrigiert
* Ausdruck: Ausdruck Lehrer Zeitkonto Bezeichnung Verplan in IST umbenannt wie im daVinci Lehrer Zeitkonto
* Ausdruck: Druckformat Tagesvertretungen: Überschrift|fehlende Lehrer mit Langnamen anzeigen entfällt; benutzen Sie bitte Seite|Bezeichnung Lehrer in Überschriften oder Zellen

## Pre-Release 6.0.189 (17.03.2015) Dateiformat 6.0.131

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Allgemein: in der Paths-Datei kann mit dem Eintrag "daVinciServerListFile" für daVinci und daVinciLook auf die daVinci.servers (Serververbindung und Startdatei) verwiesen werden, bitte beachten Sie dazu die Hinweise im Handbuch.
* Stundenplan: Bei Setzen von Terminen per Drag&Drop werden für die aktuell fokussierte Position im Stundenplan im Unverplant-Zusatzfenster ggf. die Terminkonflikte für diese Position angezeigt.
* Kursplan: Neuer Befehl zum Sortieren der Kurse in der Ansicht "Kursplan|Kurse".
* Kursplan: Kursschnittmengenmatrix wie in daVinci 5

### Verbesserte bzw. geänderte Funktion

* Allgemein: Die Schraffuren für Sperrungen wurden für bessere Lesbarkeit durch reine Farben ersetzt. Dazu wird das Farbschema in diesem Update einmalig auf die Standardwerte zurückgesetzt.

### Fehlerkorrektur

* Stundenplan: Stundenplanansicht|Schwarz/Weiß-Schaltfläche
* Stundenplan: im Zeitkonflikte-Fenster als Überschneidungen verkehrt erkannte Termine korrigiert
* Stundenplan: Problem im Zeitkonflikte-Fenster behoben (kollidierende Termin entfernen->Ja/Nein )
* Stundenplan: Klassenfaktor bei im Wertfaktor geänderten Veranstaltungen korrigiert
* Vertretungsplan: farbliche Darstellung der Lehrerfehlgründe korrigiert
* Vertretungsplan: Ersatzräume für eine Vertretung werden wieder korrekt als belegt/nicht belegt angezeigt
* Vertretungsplan: Termine tauschen: Änderung des Textes beim Vertauschen, mit angehakte Objekte werden ignoriert beim Termintausch
* Vertretungsplan: Anrechenstunden beim einem Fach ohne Anrechenstunden werden nun mit 0 gerechnet 
* Vertretungsplan: Termin verschieben mit Ersatzraum korrigiert
* Vertretungsplan: Wenn Sie in den Änderungen nach Lehrern gruppieren, können Sie über "alle expandieren" die Summen pro Lehrer einblenden
* Vertretungsplan: bei beim Vorziehen von Veranstaltungen wird für Fehlstellen nicht mehr die Klasse als fehlend gezeigt
* Vertretungsplan: löscht man eine Änderung in der Änderungsliste, bleibt die Fehlzeit, die Vertretung usw. erhalten, aber in das Element taucht nicht mehr in der Vertretungserstellung auf. Falls das Änderung-Löschen versehentlich passiert ist, können Sie Unter  Vertretung|Fehlzeiten|Extras|Weitere Aktionen mit "Vertretungselemente neu erzeugen" wieder Vertretungselemente erstellen lassen.
* Server: Fehler beim Ändern von Fehlzeiten im Serverbetrieb behoben.
* InfoServer: beim Aufruf content=xml kann die Ausgabe noch unterteilt werden in type=class, type=teacher oder type=subject
* Ausdruck: Nicht öffentliche Fehlzeit taucht nicht mehr auf

## Version 6.0.188 (06.03.2015) Dateiformat 6.0.130

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Stundenplan: Stammdaten|Klassen - Feld "Stufe" wurde erweitert, Eintrag bis max. 99 möglich 
* Stundenplan: Unter Stundenplan|Start|Automatik ist unter "Verplanung zurücksetzen" auch die Planweise(zb. pro Klassenplan) Rücksetzung der Raum- und Lehrerplanung möglich
* ÜBERSICHTEN: "Unterricht": zeigt Unterricht für Lehrer/Klassen/Fächer/Räume aus Fachsicht pro Stunde. Es kann nach Zeitraum und Team gefiltert werden. Es wird zwischen geplanten und stattfindenen Stunden unterschieden.
* ÜBERSICHTEN: "Unterrichtsstatistik" (nur für Modul Analytics): zeigt Unterricht für Lehrer/Klassen pro Tag. Es kann nach dem Zeitraum, Team, Lehrer, Klasse und Fach gefiltert werden. Es wird zwischen geplanten und stattfindenen Stunden unterschieden.
* Vertretungsplan: neuer Status Ungültig zurücksetzen
* VERTRRETUNGSPLAN: Bei Raum-Fehlzeiten kann jetzt mit Option "Nicht mehr verfübar" festgelegt werden, ob der Raum für weitere Vertretungen verfügbar ist oder nicht.
* Kursplan: Weist man einem Schüler Fächer ohne Zuweisung der Untterichtsart zu, werden im Bereich "Kursplan|Schüler" im Zusatzfenster unter "passende Kurse" alle eingerichteten Kurses des Faches angezeigt. Bitte achten Sie bei Zuweisung in den Kurs darauf, dass Sie unter "Fachwahlen" dem Schüler für das Fach die Unterrichtsart noch nachtragen.
* Kursplan: Ansicht "Schüler", im Zusatzfenster "passende Kurse" werden Konflikte bei Kurszuweisung des Schülers durch einen gelben Blitz vor dem Kurs gekenntzeichnet
* Kursplan: Ansicht "Blöcke", Register "Blöcke" - einzelne Kurse können über "strg+entf" aus dem Block entfernt werden
* KURPSLAN: Ansicht "Schüler" - neue Spalte "Hinweise", zeigt gemäß hinterlegtem Fachwahlskript im Stammdatenfenster "Klassen" (Spalte "Skript") Hinweis zu fehlenden Fachwahlbelegungen des Schülers
* Kursplan: Ansicht "Blöcke" - mit Anklicken eines Kurses im Blockfenster erhalten Sie im unteren Bereich des Fensters weitere Informationen zum Kurs wie Dauer und Lehrer
* Kursplan: neue Kursschnittmengenmatrix unter Kursplan in allen Ansichten über die Schaltfläche "Schnittmenge" aufrufbar
* Look: für Feueralarm können die Klassen/Lehrer/Räume zum aktuellen Zeitpunkt ausgegeben und exportiert werden: Unter "Klassen Jetzt"|Listen gibt es neu den Punkt "Situation zum Zeitpunkt"
* Look: Eingeben von Zusatzunterricht klappt wieder korrekt.
* Ausdruck: "Schülerplan" - optional kann nun auch der Tutor ausgegeben werden (Druckvorschau|Design, Register "Seite", Haken setzen vor "Zusatzinformationen drucken")

### Fehlerkorrektur

* Stundenplan/Vertretungsplan: Irrtümlich Anzeige der Bemerkung einer Vertretung im Stundenplan des Lehrers behoben
* Stundenplan: Publizieren|"Kalender synchronisieren" nach Google an neue Google-Schnittstelle angepasst
* Stundenplan: die Raum- und Lehrerzuordnung lässt sich getrennt von der Setzautomatik einsetzen
* Stundenplan: bei der faktorbezogenen Verrechnungsart wird der Wochenfaktor verwendet
* Stundenplan: Stammdaten|Perioden - Löschen korrigiert
* Vertretungsplan: Vertretungsregelung für verschobenen Unterricht korrigiert
* Vertretungsplan: Synchronisationsfehler bei verschobenem Unterricht korrigiert, an der Ursprungsposition wird nun korrekt der Unterricht als verschoben angezeigt
* Vertretungsplan: Lehrerfehlzeit wird durch Vorziehen vertreten – wird nicht mehr als fehlend ausgegeben
* Vertretungsplan: mehrere Vertretungselemente können markiert in einem Arbeitsgang mit "entfällt" markiert werden
* Vertretungsplan: nachträgliches Ändern eines  Raumes für ein Vertretungselement, wird nicht mehr in der Spalte "Fehlt" mit gezeigt, damit ist die Sortierung nur nach fehlendem Lehrer
* Kursplan: Blockungsautomatik - wenn der Haken beim Start der Blockungsautomatik gesetzt ist "Aktzeptiere Blockkonflikte", werden nun alle Schüler trotz möglicher Konflikte auf die Kurse verteilt
* Kursplan: Druck Kursliste korrigiert
* Kursplan: Konfliktanzeige bei Kurszuweisung
* Look: Anzeige von verschobenen Doppelstunden in der Ansicht Vertretungsplan korrigiert
* Look: Publizieren|"Kalender synchronisieren" nach Google an neue Google-Schnittstelle angepasst
* Schuldatentransferformat: beim Importieren von Kursen werden die zugeordneten Blöcke mit übernommen
* Ausdruck: "geänderte-Pläne ab" korrigiert
* HTML-Export: für Tagesvertretungen nach Klassen/Lehrer/Stunden wird für Mitteilungen der Text ausgegeben, statt des Titels

## Version 6.0.187 (17.02.2015)  Dateiformat 6.0.129

### Fehlerkorrektur

* Stundenplan: Export von SDTF-Dateien korrigiert

## Version 6.0.186 (16.02.2015)  Dateiformat 6.0.129

### Neue Funktionen

* Export: Der Export als im Format xml und json wurde jeweils um Informationen über Perioden erweitert.
* KALENDER: Neue Kalenderdateien mit den Schulferien für 2015/2016 hinterlegt
* KALENDER: Import von Kalenderdateien, Importformat UTF8 und UTF8 OHNE BOM
* Allgemein: Unter Extras|Optionen im Dialog „Bezeichnungen“ kann die Anzeige der Bezeichnungen bei Kürzeln Unterrichtsart usw. aus/eingeschaltet werden, standardmässig ist „Nur Kürzel“ an.

### Fehlerkorrektur

* Allgemein: "Plan|Importieren und Exportieren|Upload nach WebWeaver" korrigiert.
* Stundenplan: Rechte-Problem beim Bearbeiten der Stammdaten behoben
* Stundenplan: Ruft man aus den Stammdaten per F9 einen Plan auf, wird die zuletzt gewählte Plan-Ansicht gezeigt
* Stundenplan: Summenwerte aus mit wochenbezogener Berechnung korrigiert
* Stundenplan: Automatische Blockerzeugung in der Veranstaltungsliste über "#" klappt wieder
* Stundenplan: Neue Veranstaltung eingeben im Plan klappt wieder 
* Vertretungsplan: Unter Vertretungsplan|Änderungen wurde die Zählung der Vertretungen im Block korrigiert
* Vertretungsplan: Anzeige der Fehlzeiten im Fehlzeitenfenster korrigiert (Schraffur)
* Vertretungsplan: Frei gestellte und wieder eingesetzte Lehrer werden als indirekte Vertreter zum Übernehmen angeboten
* ÜBERSICHTEN: Unter Vertretungen wurde die Berechnung korrigiert
* Import: Import der Daten aus WinLD nach DaVinci (STDFACH.TXT, STDLEHR.TXT und STDKLASS.TXT) korrigiert. 

## Version 6.0.184 (23.01.2015)

### Verbesserte bzw. geänderte Funktion

* Allgemein: JSON-Export gemäß Spezifikation (siehe http://doc.stueber.de/ontimejs-json/introduction) 
* DaVinci Look: Neues "Benutzerhandbuch" unter http://doc.davinci6.stueber.de/course-plan/index.html

### Fehlerkorrektur

* Kursplan: Bereich "Schüler" Kurswahl-Zuweisung der Fachwahlen/Kurse im Serverbetrieb wieder möglich
* Allgemein: "Plan|Importieren" und "Exportieren|JSON-Daten exportieren" bzw. "Upload nach WebWeaver" korrigiert

## Version 6.0.183 (21.01.2015) Dateiformat 6.0.127

> Bitte DaVinci, DaVinci Look, DaVinci InfoServer und DaVinci Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* Stundenplan: Für den Übertrag des Lehrerunterrichts nach Magellan gibt es im Stundenplanbereich unter Extras|Weitere Aktionen eine neue Funktion "Vorgabelehrer bei Veranstaltungen anpassen". Hintergrund: für den Übertrag nach Magellan wird der Vorgabelehrer den Schülern der Klasse zugeordnet. Ändern Sie den Lehrer in der Terminliste, wird nicht der Vorgabelehrer geändert. Damit kann ein verkehrte Lehrer als Lehrerunterricht nach Magellan übertragen werden. Bitte führen Sie in diesem Fall diese neue Option aus, dann wird der erste Lehrer der Terminliste auch als Vorgabelehrer eingetragen und nach Magellan übertragen.
* Stundenplan: unter Extras|Weitere Aktionen gibt es eine neue Funktion zum Zurücksetzen des UNGÜLTIG Status von Änderungen
* Stundenplan: „Benutzername“ für Stammdaten|Klassen, damit man einen Benutzer „Klasse 8a“ im Explorer anlegen kann und dann den Schülern keine Einzelkennung geben muss.
* Stundenplan: „Soll 4“ als 4. Spalte in Stundentafeln (falls eine 3-jährige Klasse im Schulhalbjahr beginnt
* Allgemein: Unter Extras|Optionen gibt es eine neue Registerkarte UPLOAD für automatischen FTP Upload von JSON-Dateien, derzeit nur benutzt für UPLOAD nach WebWeaver (siehe PLAN > IMPORTIEREN UND EXPORTIEREN)

### Fehlerkorrektur

* Allgemein: Bezeichnung im Dialogfeld Plandatei aufräumen korrigiert 
* Stundenplan: in Veranstaltungsliste und Stundentafel ist bei den bei Fachattributen auch die Bezeichnung sichtbar
* Stundenplan: Teamfilter bei der Auswahl der Fächer in der Veranstungsliste und im Dialogfenster "Neue Veranstaltung" korrigiert
* Stundenplan: Ansicht, öffnet man weiteres Planfenster, bleiben alle als nicht-korrespondierende Pläne markiert auch so erhalten  
* Stundenplan: Plan-Eigenschaften|Statistik, "Mit Wertfaktoren (aus Stundentafel, Fach, Klasse, Veranstaltung)" korrigiert
* Stundenplan: "+"-Zeichen nach Fachkürzel bei der Datenübernahme 5 nach 6 korrigiert (wenn man einen daVinci 5 Plan mit daVinci 6 öffnet) 
* Stundenplan: Auswahlfenster Suche nach Kürzel korrigiert
* Vertretungsplan: Lehrer mit Zusatzunterricht werden wieder als indirekte Vertreter angezeigt
* Vertretungsplan: Fehlermeldung bei der Auswahl eines direkten Vertreters | wählt man V-Lehrer mit Art "Übernehmen" korrigiert
* Vertretungsplan: Folgende Termine analog vertreten" bei geblockten Kursen korrigiert  
* Vertretungsplan: Übersichten|Änderungen: in der Ausfallstatistik: Mitbetreuungen werden korrekt gezählt 
* Vertretungsplan: Vertretungsplan|Ansicht Stundenplan: "drei Pläne" entfernt
* Vertretungsplan: Raumänderung bei getauschten Elementen korrigiert
* Vertretungsplan: Lehrer-/ Raumfehlzeit korrigiert
* Vertretungsplan: Problem beim nachträglichen Änderungen im Stundenplan für bereits vertretene Veranstaltungen korrigiert, bitte führen Sie nach der Änderung den Punkt "Plan aufräumen" durch. Bei bereits erfolgten Änderungen, die als ungültig in der Vertretungserstellung angezeigt werden, wählen Sie bitte Rechtsklick|"Ungültig" zurücksetzen.
* Vertretungsplan: Vorziehen in Fehlstellen wieder möglich
* Vertretungsplan: Probleme mit Vertretungen von geblockten Stunden in der Anzeige des Vertretungslehrers gelöst 
* Vertretungsplan: Sortierung im Stammdatenfenster nach Klassen hat Auswirkung auf Sortierung im Ausdruck 
* Vertretungsplan: Lehrer fehlt/ Raum fehlt korrigiert; Änderung wird nun mit dem Status "Offen" in der Liste der offenen Vertretungen dargestellt
* Kursplan: Zeitrahmen (nicht Hauptzeitrahmen) einer Klasse hat wieder  Auswirkung auf Modul "Kursplan|Stundenplan"
* Kursplan: Bereich "Fachwahlen", trägt man in der Fachwahl eines Schülers ein neues Fach ein, wird dieses als "markiert" (gewählt) gekenntzeichnet 
* Ausdruck: "Originaltermine bei Änderungen nicht anzeigen" klappt wieder in Gesamtplänen
* Ausdruck: "Nur geänderte Pläne ab" - Filterung für Stundenplanänderung korrigiert 
* Ausdruck: "Originaltermine bei Änderungen nicht anzeigen" bei freigestellten Räumen korrigiert 
* Ausdruck: Sortierung in Stammdatenfenster wird auch im Ausdruck und HTML-Export übernommen
* Look: Suchfunktion korrigiert
* Übersichten: LEHRER-SOLL-IST –Übersicht, Ausgabe der Werte in den Spalten Ist/W und Ist/J korrigiert

## Version 6.0.182 (06.01.2015) Dateiformat 6.0.127

> Bitte daVinci, daVinci Look, daVinci InfoServer und daVinci-Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* HTML-EXPORT: Die daVinci.hfm hat sich geändert, wenn Sie mit unseren Originalvorgaben arbeiten möchten, aktualisieren Sie bitte in daVinci unter Publizieren|HTML-Pläne exportieren|HTML-Exportformate|Schaltfläche "Aktualisieren"
* InfoServer: daVinci.hfm -> Öffnen Sie die daVinci-Installation, mit der Sie die Ansichtseinstellungen für den InfoServer vornehmen und führen die Aktion Publizieren|HTML-Pläne exportieren|HTML-Exportformate|Schaltfläche "Aktualisieren" aus. Sollte die bearbeitete daVinci.hfm dieser Installation nicht identisch mit der von Ihrem daVinci-Server sein, übertragen Sie sie bitte von Hand. Den jeweiligen Pfad finden Sie hier:
* InfoServer: css-Dateien -> Wenn Sie die HTML-Vorlagen nutzen, die mit "local" benannt sind, werden css-Dateien genutzt, die auf Ihrem Server liegen. Wenn Sie mit den geänderten Vorlagen arbeiten möchten,  kopieren Sie in diesem Fall aus dem Verzeichnis "C:\ProgramData\Stueber Systems\daVinci 6\HTML\CSS" die erneuten Dateien und legen Sie in Ihr Sandbox-Verzeichnis. Für den InternetInformationServer zum Beispiel unter C:\inetpub\wwwroot\Sandbox.
* Entfernt bei daVinci: daVinci|Hilfe|Systeminfomationen|Dateien|daVinciHtmlExportformatFile
* Entfernt bei InfoServer: Rechern mit daVinciEnterpriseServer|Start|Systemsteuerung|daVinci-Server(32-Bit)|Unterkarte InfoServer|HTML-Exportformate-Datei

### Fehlerkorrektur

* Stundenplan: Automatik verbessert.  
* Stundenplan: Automatik beachtet jetzt korrekt die negative und positive Fachfolge von Veranstaltungen innerhalb einer Klasse. 
* Stundenplan: Neuer Befehl "Automatik | Veranstaltungen verplanen" verplant per Automatik eine oder mehrere in der Veranstaltungsliste ausgewählte Veranstaltungen. 
* Stundenplan: Ansicht Stundenplan: Schaltfläche "Plan hinzufügen" wieder für mehrere Pläne aktiv
* Stundenplan: Ausgabe von IST-Werten für Lehrer im Zeitkonto/Übersicht "Lehrer Soll-Ist" an die Auswahl unter Optionen|Ansicht (Ist-Stunden = geplante oder verplante Stunden) angepasst
* Kursplan: Kursplan|Schüler - Schülerkurse anzeigen: Anzeigereihenfolge der Kurse im Dialogfenster "Kurse" entspricht jetzt der Anzeige der Fachwahlen in der Übersicht.
* Vertretungsplan: Änderungen der Zeitverplanung von Terminen im Bereich Stundenplan (z.B. durch das Versetzen eines Termins von Montag auf Mittwoch) führen dazu, dass in der Spalte "Status" die betreffenden Änderungen auf "Ungültig" gesetzt werden, so dass Sie erkennen können, welche Änderungen neu bestimmt werden müssen. Dazu gibt es eine neue Farbe. Setzen Sie dazu im Dialog "Optionen" per "Standardvorgaben wiederherstellen" das Farbschema auf die Standardwerte zurück. 
* Vertretungsplan: Setzen Sie dazu im Dialog "Optionen" per "Standardvorgaben wiederherstellen" das Farbschema auf die Standardwerte zurück, wenn Sie das neue Standardfarbschema nutzen wollen. 
* Vertretungsplan: Dialog "Anrechnen" zeigt jetzt bei "Folgetermine analog vertreten" nur noch die Folgetermine, die vom Vertreter auch wirklich vertreten werden können. Somit werden Irrtümer bei Folgeterminen ausgeschlossen.
* Vertretungsplan: Lehrer-Anrechenstunden aufgrund einer Klassenfehlzeit werden wieder korrekt ausgegeben
* Vertretungsplan: Folgetermin für verschobenen Termin wird zum Vorziehen angeboten
* Vertretungsplan: Problem beim Vorziehen von geblockten Veranstaltungen behoben
* Vertretungsplan: Folgetermin analog vertreten für geblockte Termin mit Raumfehlzeit korrigiert
* Vertretungsplan: "Wie Woche zuvor" korrigiert
* Vertretungsplan: Im Dialogfenster "Änderungen mitteilen" kann jetzt zusätzlich auch eine personalisierte E-Mail Nachricht mit angegeben werden (siehe Schaltflächen rechts vom jeweiligen Eingabefeld).
* Stundenplan: Im Dialogfenster "Gruppen benachrichtigen" kann die E-Mail ebenfalls personalisiert werden (siehe Schaltflächen rechts vom jeweiligen Eingabefeld).
* Look: In den Dialogfenstern "Mitteilung senden" und "Gruppen benachrichtigen" kann jetzt zusätzlich auch eine personalisierte E-Mail Nachricht angegeben werden (siehe Schaltflächen rechts vom jeweiligen Eingabefeld).
* Stundenplan und Look: Neues Dialogfenster "Raum ändern" für einfaches Zuweisen bzw. Ändern von Räumen durch Kollegen. Das bisherige Dialogfenster "Ressourcen zuordnen" dient jetzt ausschließlich dazu Resourcen zuzuordnen. 
* Look: Neue Befehle zum Eingeben, Löschen, Editieren von Zusatzunterricht durch Kollegen. Jeder Kollege mit entsprechenden Rechten kann selbst Zusatzunterricht eingeben.
* Look: Neue Befehle zum Eingeben, Löschen, Editieren von Lehrerfehlzeiten in Lehrer-Stundenplänen. Jeder Kollege mit entsprechenden Rechten kann selbst seine Fehlzeit eintragen.
* Look: Bitte beachten Sie die neuen Benutzerrechte im DaVinci Explorer für "Räume zuweisen", "Ressourcen zuweisen" und "Zusatzunterricht bearbeiten".  
* Look: Export von Klassenlehrerliste und Konferenzliste korrigiert
* InfoServer: Übergabe von Daten vom DaVinci Server an den InfoServer korrigiert
* Optionen: Darstellung der Passwortangaben für E-Mail und SMS geändert
