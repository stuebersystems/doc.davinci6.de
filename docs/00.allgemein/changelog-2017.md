# Änderungen 2017

## DAVINCI Version 6.5.37 - WEBBOX Version 1.9.12

Veröffentlichung: 21.12.2017  
Dateiformat: 6.0.170

* VERTRETUNGSPLAN: Vertretungsregelung "Entfällt" wieder bei geblockten Klassen möglich
* VERTRETUNGSPLAN: Aktualisierungsproblem behoben \| Änderungen werden in geöffneten Plänen angezeigt
* VERTRETUNGSPLAN: Fehlzeiten-Erfassen-Fenster, beim Eintragen einer neuen Fehlzeit ist die Bemerkungszeile (Eintrag im Feld "Bemerkung") standardmäßig wieder leer
* VERTRETUNGSPLAN: Löschen von Fehlstellen über "Änderungen löschen" im Planfenster wieder möglich
* VERTRETUNGSPLAN: Fehlstellen, die in der Liste der offenen Vertretungen auf "Geschlossen" gesetzt werden, werden in Spalte "Art" weiterhin als Fehlstelle angezeigt, allerdings nicht mehr gelb hervorgehoben

![Anzeige einer &quot;Geschlossenes&quot; Fehlstelle](/assets/images/6.5.37.01.png)

* VERTRETUNGSPLAN: Beim Vorziehen von Doppelstunden wird im Ausdruck wieder richtig in Spalte "Art" die Positionsnummer der vorgezogenen Veranstaltung angezeigt. Bsp. 8.-9. Std. soll auf die 1.-2. Stunde vorgezogen werden, beim Asudruck wurde sonst immer in der ersten Zeile in Spalte "Art" die Meldung angezeigt, dass die 8-9 Std. verschoben wurde. Nun steht hier richtig, dass die 8. Std. verschoben wurde.
* DRUCK:  Klassenvertretungen\|Vertretungsliste nach Klassen: bei Klassenfehlzeit wurde auch unveränderter Unterricht gezeigt
* MOBILE: Konfigurationsdaten in Android werden dauerhaft gespeichert.
* MOBILE: Rotationproblem in iOS 11 gelöst

## DAVINCI Version 6.5.36

Veröffentlichung: 04.11.2017  
Dateiformat: 6.0.170

* VERTRETUNGSPLAN: Raumänderungen werden wieder "+ neuer Raum (alter Raum)" dargestellt und für den Druck übergeben.
* WEBBOX: Der DAVINCI Server liefert für Lehrerpläne (Lehrerrechte) geänderte und unveränderte Planelemente.

## DAVINCI Version 6.5.35

Veröffentlichung: 27.10.2017  
Dateiformat: 6.0.170

* STUNDENPLAN: Verschieben von Stunden wieder möglich
* KURSPLAN: Kurszuweisung beim Ändern der Unterrichtsart bleibt erhalten
* VERTRETUNGSPLAN: Bei der Vertretung von Aufsichten werden wieder Lehrer zur Auswahl angezeigt, die bereits eine Aufsicht zur gleichen Zeit haben

## DAVINCI Version 6.5.34  WEBBOX Version 1.9.12

Veröffentlichung: 16.10.2017  
Dateiformat: 6.0.170

* STUNDENPLAN: Anzeige "Passende Räume" korrigiert
* VERTRETUNGSPLAN: Fehler bei der Anzeige direkter Vertreter mit einer Freistunde behoben.
* VERTRETUNGSPLAN: Arbeiten mit unterschiedlichen Zeitrahmen - zukünftig werden Kollegen, die aufgrund Ihres Zeitrahmens nur einen Teil der zu vertretenden Stunde frei haben, als indirekte Vertreter angezeigt.
* VERTRETUNGSPLAN: mögliche direkte Vertreter, die als "Zusätzlich" in die Vertretungsregelung hätten einfließen können, werden nun wieder zur Auswahl gestellt
* HTML-Export: doppelte Anzeige von Aufsichten, die noch eine nullte Stunde vor sich haben, korrigiert

* WEBBOX: ein fehlender Raum bei Veranstaltungen mit zwei Räumen wird korrekt in der WEBBOX angezeigt

* WEBBOX: Mitteilungen, die über den Vertretungsplan eingetragen wurden, werden nun auch in die WEBBOX übergeben  
  ![Anzeige Mitteilung im V-Plan](/assets/images/6.5.33.01.png)

![Anzeige Mitteilung in WEBBOX](/assets/images/6.5.33.02.png)

## DAVINCI Version 6.5.33

Veröffentlichung: 02.10.2017  
Dateiformat: 6.0.170

* STUNDENPLAN: `Extras > Optionen > Stundenplan`: Einstellungen unter `Was soll ein Doppelklick auf einen Termin im Stundenplan bewirken` wird wieder berücksichtigt.
* STUNDENPLAN: Anzeige der Positionskonflikte beim Setzten korrigiert
* STUNDENPLAN: Schienen werden wieder angezeigt
* VERTRETUNGSPLAN: `Vertretungsplan > Fehlzeiten`: Korrektur des Eintrags der Fehlzeiten im Zeitplan durch Markieren mit der Maus.
* VERTRETUNGSPLAN: Tab-Taste innerhalb Eingabemasken beim Zusatzuntericht springt in alle Felder
* VERTRETUNGSPLAN: Aufsichtsbereiche - für fehlende Aufsichten werden keine bereits verplanten Aufsichtslehrer mehr angezeigt
* VERTRETUNGSPLAN: `Vertretungsplan > Vertretungen` trägt man im Planfenster rechts z.B. eine Raumfehlzeit ein, springt der Plan rechts nicht mehr zum Lehrerplan des in der Liste der offenen Vertretungen markierten Lehrer
* VERTRETUNGSPLAN: `Einstellungen > Eignungsfaktoren` "Präsenz" Wert wir auch nach dem Schließen der Datei gespeichert
* VERTRETUNGSPLAN: Zusatzunterricht taucht in der Liste der offenen Vertertungen auf, wenn der Lehrer fehlend ist
* VERTRETUNGSPLAN: gibt man im Planfenster in der Ansicht `Vertretungen > Vertretungen` eine Fehlzeit ein, wird diese sofort angezeigt
* VERTRETUNGSPLAN: Markierung beim Eintrag einer Fehlzeit wird korrekt übernommen
* KURSPLAN:  `Kursplan > Stundenplan` in der Planansicht links Pos. und Uhrzeit wieder eingeblendet
* HTML EXPORT:  HTML Export "Tagesvertretungen nach Klassen"; Mitteilungen werden wieder mit ausgegeben, wenn eine Teamfilterung eingestellt ist:
* HTML-EXPORT: Auswahl "Gesamtplan" funktioniert wieder
* LOOK: im Vollbildmodus wird die Uhr ausgeblendet, wenn in den Optionen eingestellt
* LOOK: eine Raumbuchung mit der rechten Maustaste "neue Raumbuchung" wird sofort angezeigt
* KURSPLAN: `Kursplan > Blöcke`- Kurse können wieder verschoben werden
* KURSPLAN: `Kursplan > Stundenplan`- Fehler beim Aufruf des Stundenplans behoben

## DAVINCI Version 6.5.31

Veröffentlichung: 21.09.2017  
Dateiformat: 6.0.170

* SDTF: D6-Zeile Lehrer Ist wird wieder ausgegeben
* STUNDENPLAN:  Wenn Sie in den Klassenstundentafeln die Spalte Kategorie \[Veranstaltungskategorie\] gefüllt haben, wird der Wert wieder geklammert in der Veranstaltungsliste eingeblendet, es sein denn, Sie haben der Veranstaltung direkt eine Kategorie zugewiesen. **WICHTIG:** Wenn Sie die Fachkategorie im Nachhinein in der Veranstaltungsliste ändern wollen, müssen Sie die Änderung in der Stundentafel vornehmen. Die Kategorie wird dann in die Veranstaltungsliste synchronisiert.

## DAVINCI Version 6.5.30

Veröffentlichung: 19.09.2017  
Dateiformat: 6.0.170

* SDTF: D6-Zeile wird auch für Unterricht ohne Lehrerzuweisung erzeugt
* STUNDENPLAN: "Veranstaltung bearbeiten"  Eintrag unter "Kategorie" kann wieder dauerhaft mit Entf gelöscht werden
* STUNDENPLAN: Ist in den Plan-Eigenschaften (Plan\|Eigenschaften) in der Registerkarte "Zeitraum" das Wochenende bis Sa definiert, wird im Planfenster die Wochenansicht fest von Mo-Sa angezeigt. Ein scrollen zum Wochentag Samstag ist nicht mehr erforderlich.
* EXPLORER: Eine für Benutzer erfasste Bemerkung wird korrekt gespeichert
* VERTRETUNGSPLAN: Aktualisierungsproblem beim Erfassen von Lehrerfehlzeiten und Mitteilungen gelöst - Fehlzeiteneinträge sind wieder automatisch in den Planfenstern sichtbar
* VERTRETUNGSPLAN: Vertauschen von geblockten Stunden - es werden wieder richtig alle Elemente des Blockes verschoben, wenn im "Termine Vertauschen"-Fenster die Option `Gesamten Block (alle Termine des Blocks) verschieben` aktiviert ist 
* VERTRETUNGSPLAN: Aktualisierungsproblem im Bereich "Fehlzeiten" gelöst, der Zeitplan passt sich entsprechend geöffneten Planfenster (Lehrer, Klassen oder Raumplan) an 
* VERTRETUNGSPLAN: erzeugte Fehlstellen, die durch Vorziehen eines Unterrichtes gefüllt werden, werden nicht mehr als "zusätzlich" im Plan deklariert, da es "vorgezogene" Stunden sind (Kollegen haben durch Vorziehen von Veranstaltungen keinen zusätzlichen Unterricht, der wurd nur verlegt)
* VERTRETUNGSPLAN: Wenn innerhalb einer Klasse Unterricht vorgezogen und danach für diese Klasse eine Fehlzeit erfasst wurde, wurde der vorgezogene Unterricht wieder zurückgesetzt. Dies kann man optional deaktiviert werden. Beim Erfassen der Klassenfehlzeit kann der Haken gesetzt werden vor `Diese Änderungen zurücksetzen` oder nicht.  
  ![Fehlzeiten Erfassen-Fenster](/assets/images/6.5.30.01.png)

* AUSDRUCK: Tagestrennlinien in Gesamtplänen werden zwischen den Wochentagen wieder korrekt angezeigt

* AUSDRUCK: Format "Klassenvertretungen": Ausgabe vom Stundentausch in der Darstellung angepasst (Vergleichbar mit Darstellung in Version 5 von DAVINCI)  
  ![Stundentausch zweier Veranstaltungung](/assets/images/6.5.30.02.png)

* Übersichten: AUSFALLSTATISTIK für Sachsen, Korrekturen vorgenommen

* IMPORT: Import Fächer aus edoo.sys in Stammdaten DAVINCI ist Fachkategorie leer, wird nun keine Fachkategorie in DAVINCI importiert

* KALENDER. korrigierte Ausgabe von unterrichtsfreien Termin im Ausdruck Raum Gesamtplan

* EXPLORER: Korrektur der Benutzerrechte für den Zugriff auf Unterordner im DAVINCI EXPLORER

## DAVINCI Version 6.5.29

Veröffentlichung: 04.08.2017  
Dateiformat: 6.0.170

* INFOSERVER: Zahlreiche sicherheitsrelevante Optimierungen.
* WEBPUBLIKATIONEN: parallel wurden auch neue Ausgaben der [DAVINCI WEBBOX](https://davinci-webbox.stueber.de/) (Anleitung fürs Update [hier](https://doc.davinci6.stueber.de/09.infoserver/update-internet-publication/infoserver-und-webbox-aktualisieren)) und der Mobile APP ( bitte aus dem Android-Play Store oder IOS-App Store laden) veröffentlicht.  
* STUNDENPLAN/VERTRETUNGSPLAN: aktuelles Datum wird im Planfenster (Kopftitel oben) wieder 
  farblich hervorgehoben
* VERTRETUNGSPLAN:  Fächer, die im Stammdatenfenster als nicht vertretbar deklariert sind (Spalte "Vertretung" -&gt; "Keine Vertretung" zugewiesen), tauchen nicht mehr in der Liste der offenen Vertretungen auf
* AUSDRUCK: In Wochenplänen wird bei der Datumsangabe `Kopftitel oben` nun auch die Jahreszahl mit ausgegeben 

![Ausdruck](/assets/images/imagesliesmich/6.5.29.01.png)

* Ausdruck: Lehrerpläne - Lehrerfehlgründe die farbig hinterlegt wurden, werden nun mit ausgedruckt. Hintergrund: Wenn ein Leher an einem Tag z.B.
  keinen Unterricht hat, ist im Lehrerplan der Tag wie "frei" im Ausdruck angezeigt worden, obwohl der Lehrer ganztägig zu einer Prüfung extern ist oder eine Fortbildung hat usw.

![Ausdruck](/assets/images/imagesliesmich/6.5.29.02.png)

* Importieren und Exportieren: Korrektur beim Import einer SDTF (Schuldatentransferdatei)
* KALENDER: erneute Aktualisierung aller Kalenderdateien für das Schuljahr 2017/2018, die im Bereich "Kalender" über den Aufruf `Importieren` eingelesen werden können

## DAVINCI Version 6.5.28

Veröffentlichung:  07.07.2017  
Dateiformat: 6.0.170

* DRUCK: `Publizieren > Pläne drucken > mit Vertretungsplaninformationen`

## DAVINCI Version 6.5.27

Veröffentlichung: 06.07.2017  
Dateiformat: 6.0.170

* STUNDENPLAN: Anzeige geeigneter Aufsichtslehrer korrigiert
* DRUCK:  Tagesvertretungen nach Stunden: Zeilenhöhe korrigiert
* DRUCK:  Teilweise fehlerhafte Ausgabe der Stundenpläne für die letzte Unterrichtswoche korrigiert. 
* DRUCK:  Lehrervertretungen Hinweis in der Überschrift von wann bis wann der Vertretungsplan gilt wieder eingefügt
* ALLGEMEIN: JSON Export korrigiert

* KALENDER:  Excelexport Ereignisse Kalender, Spalte  Beginnt und Endet wird korrekt übergeben

* VERTRETUNGSPLAN: "Extras \| Weitere Aktionen \| Alte Änderungen löschen" löscht nun auch die Anrechenstunden

* VERTRETUNGSPLAN: Die Vertretungsstatistik zeigt wieder alle Monate des Planungszeitraumes an.

![Statistik](/assets/images/imagesliesmich/6.5.27.01.png)WEBBOX: Stunden fehlt bei Klassenrechten, korrigiert

## DAVINCI Version 6.5.26

Veröffentlichung: 16.05.2017  
Dateiformat: 6.0.170

* VERTRETUNGSPLAN: Vorziehoptionen fehlten, wenn Stunden z.B. im Nachmittagsbereich nicht wie alle anderen 45 min lang sondern nur 40 min lang sind - diese Veranstaltungen werden nun auch zum Vorziehen angeboten 
* VERTRETUNGSPLAN: Befehl `DAVINCI > Extras > Plandatei aufräumen` führte zum Löschen von Zusatzunterricht, der ohne Klassenzuordnung angelegt wurde. Dies wurde korrigiert.
* SERVER: Das DAVINCI-Server-Control in der Systemsteuerung Ihres DAVINCI-Serverrechners prüft korrekt auf neue Updates. (`Systemsteuerung > DAVINCI-Server (32-Bit) > Unterkarte "Hilfe" > Schaltfläche "Auf Aktualsierung prüfen"`)
* LOOK: Die Option unter `DAVINCI LOOK > Plan > DAVINCI-Optionen > Einstellungen > Serverbetrieb > Trennung vom Server bestätigen` wurde korrigiert.

![DAVINCI LOOK Optionen ](/assets/images/imagesliesmich/6.5.26.01.png)

* KALENDER: Neue Ereignis im Dialogfenster erstellen und direkt per Email versenden klappt wieder
* Ausdruck: Druckformat "Veranstaltungsliste Lehrer" - es wird wieder richtig gemäß Einstellungen unter `DAVINCI > Extras > Optionen > Ansicht >Lehrer-Ist Werte in Zeitkonten` der Geplant/Verplant-Wert ausgegeben

![DAVINCI Optionen ](/assets/images/imagesliesmich/6.5.26.02.png)

* Ausdruck: VERTRETUNGSPLAN: Ausdruck "Tagesvertretungen nach Klassen" - es erschienen Klassen, für die keine Änderung vorgenommen wurde - dies ist korrigiert
* Ausdruck: Druckformat "Tagesvertretungen nach Klassen" - es wurden Klassen ausgegeben, für die keine Änderung vorgenommen wurden - korrigiert
* Ausdruck:  Druckformat „Lehrervertretungen“ - die Spalten "Zeit" und "Datum" werden wieder ausgedruckt. Spalt "Art" ist wieder gefüllt und Inhalte in Spalte "Info" sind wieder vollständig.
* Ausdruck: In Vertretungsplänen wir unter `Design > Spalten` der aktivierte Haken vor "Text in Zellen umbrechen" wieder im Druckbild berücksichtigt.

![Druckvorschau, Design ](/assets/images/imagesliesmich/6.5.26.03.png)

* Ausdruck: Druckformat "Vertretungslehrerliste" - der unter `Design > Seite` gesetzte Haken vor "Jede Tabelle auf neuer Seite beginnen" wird wieder dauerhaft gespeichert
* Ausdruck: Druckformat "Veranstaltungsliste Lehrer" - der unter `Design > Seite` gesetzte Haken vor "Nächste Liste auf neuer Seite beginnen" wird wieder dauerhaft gespeichert
* XML-Daten exportieren: Der Export von XML Daten zweier aufeinenderfolgender Tage unter `Plan > Importieren und Exportieren > DAVINCI XML-Daten exportieren` ist wieder möglich
* KALENDER: korrigiert Ferienkalender Bayern

## DAVINCI Version 6.5.25

Veröffentlichung: 25.04.2017  
Dateiformat: 6.0.170

* VERTRETUNGSPLAN: In der Vertretungsstatistik werden unter "Negative Anrechenstunden" die korrekten Anrechenstunden ausgewiesen. Sie stimmen nun wieder mit den negativen Anrechenstunden überein, die in der Ansicht "Anrechnungen" pro Lehrer gelistet sind.
* VERTRETUNGSPLAN: Entfällt die Vertretungsregelung für eine Klasse, haben Sie die Möglichkeit zu entscheiden, ob die Teilnehmer frei haben oder nicht. Weiterhin können Sie ggf. den Unterricht der entfällt vertreten lassen - den Lehrer den Sie hier auswählen, bekommt im Lehrerplan einen entsprechenden Hinweis. Bitte beachten Sie, dass das Aufklappmenü alle Lehrer auflistet, unabhängig davon ob Sie Unterricht haben oder nicht.  
  ![Entfällt ](/assets/images/imagesliesmich/6.5.25.03.png)

* KALENDER: Versand von Emails korrigiert (fehlende Trennung der Adressen, Titel des Ereignisses)

* KALENDER: neue Kalenderdateien (Ferien/Feiertagskalender) für das Schuljahr 2017/2018 stehen zur Verfügung

* DRUCK: Der Typ "Klassenvertretungen" zeigt Zusatzunterricht ohne Klassenauswahl nicht mehr mit an

* DRUCK: Der Typ "Klassenvertretungen" zeigt  Ausfallinfos nur noch für betroffene Klassen an

* DRUCK: in den Einstellungen der Druckformate können Sie den Zeilenabstand (positive und negative Werte sind möglich) und die Position innerhalb der Zelle beeinflussen

![Neue Einstellmöglichkeiten für den Zeilenabstand und die Positionierung in der Terminzelle](/assets/images/imagesliesmich/6.5.25.png)

* DRUCK: die Option "Terminzeilen umbrechen" für Druckformate unter `Publizieren > ausgewähltes Druckformat > Termine` wurde korrigiert
* DRUCK: Die Hintergrundfarbe aus dem Stundenplan kann auch im Druck verwendet werden
* KALENDER: erfasste unterrichtsfreie Ereignisse für Teilnehmer, die nur in Teilnehmerplänen sichtbar sein sollen, werden nun im Planfenster korrekt angezeigt.

![Anlegen eines unterrichtsfreien Ereignisses nur für Teilnehmer](/assets/images/imagesliesmich/6.5.25.01.png)

![Anzeige des unterrichtsfreien Ereignisses im Plan des Teilnehmers](/assets/images/imagesliesmich/6.5.25.02.png)

* Übersichten: "Ausfallstatistik" für Sachsen, bitte beachten Sie die aktualisierte Dokumentation für diese \[Ausfallstatistik\] ([https://doc.davinci7.stueber.de/statistik/ausfallstatistik.html](https://doc.davinci7.stueber.de/statistik/ausfallstatistik))

## DAVINCI Version 6.5.24

Veröffentlichung: 28.03.2017  
Dateiformat: 6.0.169

* STUNDENPLAN: Nachkommastellen aus `Einstellungen > Statistik` werden für Ist/W übernommen, ebenfalls in den Ausdrucken (Veranstaltungsliste Lehrer, Lehrer-Zeitkonto)

![Plan-Eigenschaften](/assets/images/imagesliesmich/6.5.23.05.png)

* STUNDENPLAN: das aktuelle Datum wird im Planfenster farblich hervorgehoben

![Planfenster](/assets/images/imagesliesmich/6.5.23.06.png)

* STUNDENPLAN: Anzeige der Lehrer-Ist-Werte in Zeitkonten gibt korrekt den geplant bzw. verplant Wert an. DAVINCI prüft hier Ihre Einstellungen in den DAVINCI Optionen unter "Ansicht" und gibt entweder den Geplant- oder den Verplant-Wert beim Ist aus.

![DAVINCI Optionen, Ansicht](/assets/images/imagesliesmich/6.5.23.08.png)

* VERTRETUNGSPLAN: In den Druckformaten bzw. HTML-Exportformaten für den Vertretungsplan (Tagesvertretungen nach Klassen, - nach Stunden, - nach Lehrern) kann für alle Formate optional "Aufsichten anzeigen" gewählt werden. 
* VERTRETUNGSPLAN: Lehrer, die an Tagen gesperrt sind, an denen es offenen Vertretungen gibt, werden nicht mehr als "Vorziehbare Vertreter" angezeigt

* VERTRETUNGSPLAN: das aktuelle Datum wird im Planfenster farblich hervorgehoben

* VERTRETUNGSPLAN: Zusatzunterricht, der im Planfenster "Lehrer" angelegt wurde, erscheint nun auch wieder im Planfenster des gewählten Faches des Zusatzunterrichtes

* EMAIL/SMS: unter `Publizieren > Änderungen mitteilen` können Sie per Klick die Empfänger  `Alle demarkieren` oder  `Alle markieren`

* EMAIL/SMS: unter `Publizieren > Änderungen mitteilen` können Sie neben dem Datum auch die Uhrzeit einstellen, seit der Änderungen erfolgt sind

* EMAIL/SMS: unter `Publizieren > Änderungen mitteilen` können Sie sich Änderungen eines Tages zwischen "Von" und "Bis"-Uhrzeit anzeigen lassen und gefiltert versenden

![Änderungen mitteilen](/assets/images/imagesliesmich/6.5.23.07.png)

* HTML-Export: Beim Export der Raum- und der Klassenpläne wird in den Plänen die Anpassung aus dem Design unter `Seite > Bezeichnungen` ausgegeben.
* HTML-Export: Beim Export der "Tagesvertretungen nach Klassen" werden Mitteilungen wieder korrekt ausgegeben.

## DAVINCI Version 6.5.23

Veröffentlichung: 10.03.2017

* SERVER und WEBBOX:

  * Die Anzeige von Änderungen in Klassen- und Lehrerplänen für Webbox und die App wurde für folgende Situation korrigiert: Klasse fährt zur Klassenfahrt, Lehrer begleiten (Korrektur am DAVINCI Server, nicht an der Webbox/App)
  * Die Anzeige der fehlenden Lehrer und Klassen über der Vertretungsliste wurde für folgende Situation korrigiert: Klasse fährt zur Klassenfahrt, Lehrer begleiten (Korrektur am DAVINCI Server und der [WEBBOX 1.9.10 (davinci-substitutions.html)](http://davinci-webbox.stueber.de/))

* STUNDENPLAN: `Plan > Neu > Neuen leeren Plan erstellen, aber aktuellen Planrahmen übernehmen` korrigiert

* STUNDENPLAN: Bei der Lehrerzuweisung wird der Differenz-Betrag angepasst. Bereits geplante Stunden sind in der Differenz zu sehen.

* STUNDENPLAN: In der Unterrichtsmatrix wurde die Anzeige der gelben Markierung für noch fehlende Elemente in den Veranstaltungen korrigiert.

* STUNDENPLAN: Unterrichtsmatrix, gelbe Markierung erscheint nur, wenn noch keine Lehrerzuweisung erfolgt ist

![Markierung in der Unterrichtsmatrix](/assets/images/imagesliesmich/6.5.23.03.png)

* DRUCK: Mitteilungen für Lehrer werden nicht in das Druckformat Klassenvertretungen mit ausgegeben.
* HTML-Export: Die Optionen "Klasseausfalltermine anzeigen" und "Aufsichten anzeigen" wurden für die Ausgabe der "Tagesvertretungen nach Klassen/Lehrer/Stunden" korrigiert.

![Einstellungen für HTML-Export &quot;Tagesvertretungen nach Klassen/Lehrer/Stunden&quot;](/assets/images/imagesliesmich/6.5.23.04.png)

* VERTRETUNGSPLAN: Die Anzeige der freien Räume wurde korrigiert: Räume die bereits durch Verschiebungen belegt sind, werden als belegt angezeigt.
* VERTRETUNGSPLAN: Wenn die Option "Aber nicht aus der Vergangenheit" unter `Vertretungsplan > Start > Einstellungen > Ansicht` aktiviert ist, werden nur Termine ab heute gezeigt.

![Korrigierte Option](/assets/images/imagesliesmich/6.5.23.02.png)

## DAVINCI Version 6.5.22

Veröffentlichung: 05.03.2017

* DRUCK/HTML-Export: `Tagesvertretungen nach Klassen/Lehrern/Stunden` --&gt; `Klassenausfall Termine anzeigen` kann optional wieder ausgewählt werden
* DRUCK/HTML-Export: `Lehrervertretungen`/`Vertretungslehrerliste` --&gt; `Aufsichten anzeigen` kann optional wieder ausgewählt werden
* DRUCK/HTML-Export: Fachänderungen (über Befehl `Fach ändern`) erscheinen wieder im Ausdruck und HTML Export

* VERTRETUNGSPLAN: fehlende Klassen wurden fälschlicherweise in der Liste der offenen Vertretungen angezeigt, diese tauchen nun nicht mehr auf

* VERTRETUNGSPLAN: Vertretungsregelung `Wie Woche zuvor`nun wieder möglich, wenn man in der Woche zuvor die Vertretung auf `Entfällt` gesetzt hatte

* Übersichten: Ausfallstatistik (für Sachsen) - eine Raumänderung (über Befehl `Raum ändern`) wird in der Ausfallstatistik nicht mehr als Vertretung ausgewiesen. Es handelt sich um einen Raumtausch, gleiches Fach, für die Schüler und den Lehrer fällt also nichts aus.

* Übersichten: Ausfallstatistik (für Sachsen) - Zeitraumfilter korrigiert

## DAVINCI Version 6.5.21

Veröffentlichung: 28.02.2017

* STUNDENPLAN: Planfenster - Register unter Plan passen sich entsprechend der markierten Position im Plan an (Reiter aktualisieren wieder)
* STUNDENPLAN: Automatiklauf korrigiert, Stunden werden wieder über die gesamte Woche verplant
* STUNDENPLAN: JAHRESVERTEILUNG, Listenansicht Verplant je Woche korrigiert. Es wurden fäschlicherweise Pausenzeiten bei Doppelstunden, die über eine Pause verplant wurden, in die Berechnung mit einbezogen.
* STUNDENPLAN: Bei der Umplanung von Stunden kam es zum Programmabsturz, dies wurde korrigiert
* STUNDENPLAN: Veranstaltungsliste Lehrer - hier "IST" , Zeitkonto Lehrer und Summe\|Wochenschnitt --&gt; Verplant Wert gibt wieder einheitlich den richtigen Wert aus.
* STUNDENPLAN: Problem beim Entfernen eines Termines aus dem Plan gelöst. Termine können wieder per Drag&Drop aus dem Plan gezogen werden
* STUNDENPLAN: Befristung von Veranstaltungen wird wieder in den Verplant-Wert bei der Wochenbezogenen Verrechnungsart übernommen

* VERTRETUNGSPLAN: Planfenster - Register unter Plan passen sich entsprechend der markierten Position im Plan an (Reiter aktualisieren wieder)

* LOOK: Gebäudefilter für die Vertretungsplananzeige

* HTML EXPORT: "Tagesvertretungen nach Lehrern", Reihenfolge korrigiert

* HTML EXPORT: "Lehrervertretungen" - "Klasse fehlt" kann optional wieder angezeigt werden

* DRUCK: "Tagesvertretungen nach Klassen" - Aufsichtsvertretungen können optional wieder angezeigt werden

* DRUCK: "Lehrervertretungen" - "Klasse fehlt" kann optional wieder angezeit werden

* DRUCK: "Tagesvertretungen nach Klassen" - Vertretungsregelungen für Stunden ohne Klassenzugehörigkeit werden mit aufgeführt (Spalte Klasse bleibt leer)

* WEBBOX: vorgezogener Unterricht erscheint nicht mehr doppelt

* WEBBOX: Mitteilungen erscheinen nun wieder (Achtung: ganztägige Mitteilungen sind aktuell nicht darstellbar)

* SERVER: Bisher wurde die Session eines DAVINCI-Clients mit dem DAVINCI-Servers nach 20 Minuten Inaktivität geschlossen.Bei einer Wiederaufnahme nach der Dauer muss erst der aktuelle Stand vom DAVINCI-Server abgeholt werden. Die Dauer bis zum Inaktivieren der Session zwischen Client und Server wurde auf 120 Minuten erhöht, nach den 120 Minuten erhält man eine entsprechende Meldung, das zuerst die Daten aktualisiert werden.

## DAVINCI Version 6.5.20  WEBBOX Version 1.9.9

Veröffentlichung: 09.02.2017

* WEBBOX: Bitte beachten Sie die aktualisierte Ausgabe der [Webbox (v1.9.9)](http://davinci-webbox.stueber.de/). Das Einfügen der neuen Dateien beschreiben wir im Abschnitt ["Die DAVINCI WEBBOX aktualisieren"](https://doc.davinci6.stueber.de/09.infoserver/setup-webbox/iis-10.html#die-davinci-webbox-aktualisieren).
* STUNDENPLAN: Korrektur im Export von json-Daten
* STUNDENPLAN: Der Wert aus `Stammdaten > Fächer` wird in der Berechnung unter `Übersichten > Lehrer-Soll-Ist` berücksichtigt 
* STUNDENPLAN: Aufrufe unter `Extras > Importieren und Exportieren` korrigiert
* VERTRETUNGSPLAN: Vertreter werden zum Vorziehen von Terminen angeboten
* WEBBOX: Anzeige von Stunden integrierter Klassen
* INFOSERVER: Anzeige von Stunden integrierter Klassen

## DAVINCI Version 6.5.19  WEBBOX Version 1.9.8

Veröffentlichung: 20.01.2017

### Fehlerkorrektur

* VERTRETUNGSPLAN:  beim Erfassen einer Mitteilung ist das Feld "Bis" zum Belegen des Bis-Datums wieder vorhanden 
* VERTRETUNGSPLAN: im Fenster "Vertreter vorziehen" werden Folgetermine wieder angezeigt
* VERTRETUNGSPLAN: fehlender Lehrer wird bei Unterrichtsausfall der Klasse im Ausdruck, HTML-Export und im INFOSERVER nicht mehr in der Spalte "Vertreter" ausgegeben, diese bleibt nun richtig ohne Inhalt
* VERTRETUNGSPLAN: Vorziehen von Doppelstunden, diese werden nun nicht mehr doppelt im Klassenplan angezeigt
* VERTRETUNGSPLAN: Zusatzunterricht wird wieder im Ausdruck/HTML/Webbox ausgegeben
* VERTRETUNGSPLAN: Raumänderung und nachträgliche Lehrerfehlzeit zur selben Zeit wird nun wieder richtig in der Liste der offenen Vertretungen in einer Zeile ausgegeben. Bereits erfasste Raumänderungen werden durch das Erfassen der Lehrerfehlzeit automatisch zurückgesetzt, diese muss nun neu vertreten werden.
* VERTRETUNGSPLAN: Mitteilungen die nur für Lehrer eingegeben wurden, erscheinen nicht mehr im Ausdruck und HTML-Export "Klassenvertretungen"
* VERTRETUNGSPLAN: erfasste Lehrerfehlzeit führt nicht mehr dazu, dass Änderungen die man über das Planfenster `rechte Maustaste > Raum ändern bzw. Fach ändern` vorgenommen hat, aus dem Plan entfernt werden. Diese Fach- bzw. Raumänderungen bleiben bestehen.

* KALENDER: hat man in DAVINCI einen Zusatzkalender (Ablage im Netzwerk) hinzugefügt und später ein Ereignis in diesem Kalender bearbeitet, kam es zu einer Zugriffsverletzung - dieses Problem ist gelöst

* DRUCK:  Mitteilungen für Klassen werden im Druckformat Tagesvertretungen nach Klassen ausgegeben

* WEBBOX/APP: fehlende Stunden in Lehrer- und Klassenstundenplänen werden angezeigt



