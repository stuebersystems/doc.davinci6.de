# Schulportal HESSEN

Mit DaVinci ist ein manueller Upload der Stunden- und Aufsichtplandaten sowie der Vertretungsplandaten in das Schulportal HESSEN möglich. Das Schulportal HESSEN ist ein Service, der von der _Hessischen Lehrkräfteakademie_ den Schulen zur Verfügung gestellt wird.

Bitte schauen Sie auch [hier](https://support.schulportal.hessen.de/knowledgebase.php?category=76) direkt auf der Seite des Schulportal Hessen und infomrieren sich zu den aktuellen Möglichkeiten.

## Stunden- und Aufsichtspläne

## JSON Export

!!! warning Wichtig
    Vor dem Start des Imports in LANIS wird dort die Dateiendung überprüft. Hier kann es zu Problemen kommen, wenn Sie im Dateinamen Punkte verwendet haben, zum Beispiel Plan 11.11.2021.json.

Über den JSON Export werden Stunden- und Aufsichtspläne wochenweise übergeben und enthalten somit Informationen über periodisch stattfindende Veranstaltungen.

Generell gilt für den Export für einen Zeitraum:

Wenn Option "Alle Wochen" in DaVinci gewählt wurde, dann enthält die JSON.Datei keine Terminangaben für die Stunde, sondern nur die Nummer des Wochentags (weekday). Somit darf beim Import ins Schulportal auch nicht die Option "Datei enthält Datumsangaben" gewählt werden.

Wenn ein Zeitraum für den Export gewählt wurde, enthält die JSON.Datei für die Stunde ein Array von Datumsangaben (dates), aber nicht das Feld Weekday. Dann kann beim Import die Option für mehrere Wochen gewählt werden. Zudem muss beim Export die Option "Termine" ausgewählt sein.

#### DaVinci JSON-Daten exportieren

Doku in Bearbeitung

1. Wählen Sie über `Plan > Importieren und Exportieren > Exportieren > DaVinci JSON-Daten exportieren` aus und klicken Sie auf `Weiter`.

2. Geben Sie im Bereich `Datei` über das Eingabefeld die Datei an, in die Sie die Daten exportieren wollen. Im Bereich `Zeitraum` wählen Sie `alle Wochen` aus. Klicken Sie auf `Weiter`.

### XML Export (bitte zukünftig nicht mehr verwenden)

Im Schulprotal HESSEN kann die Datei des XML-Exports aus DaVinci ausgewertet werden. Der XML-Export enthält den Stunden- und Aufsichtsplan aus DaVinci. Um die Daten im Schulportal HESSEN anzeigen zu lassen, muss der Export der XML-Datei aus Sicht aller Wochen erfolgen. Hier werden jedoch aktuell keine Informationen über die Perioden übergeben.

#### DaVinci XML-Daten exportieren

1. Wählen Sie über `Plan > Importieren und Exportieren > Exportieren > DaVinci XML-Daten exportieren` aus und klicken Sie auf `Weiter`.

2. Geben Sie im Bereich `Datei` über das Eingabefeld die Datei an, in die Sie die Daten exportieren wollen. Im Bereich `Zeitraum` wählen Sie entweder `Alle Wochen` oder `Nur Wochen` und geben ein `Von` und `Bis`-Datum ein. Letzteres ermöglicht einen Export von wochenbezogenen Veranstaltungen. Bitte beachten Sie in diesem Falle unbedingt darauf, dass Sie unter `Auswahl` den Haken vor `Termine` gesetzt haben. Klicken Sie auf `Weiter`.
3. Die Daten werden exportiert. Klicken Sie im Dialogfenster auf `OK`. 

Diese DaVinci JSON-Export Datei müssen Sie nun noch in das Schulprotal HESSEN hochladen.

## Export der Vertretungspläne für das Schulportal HESSEN

Um Vertretungsplaninformationen aus DaVinci in das Schulportal HESSEN zu übergeben, nutzen Sie bitte die dafür eingebaute Exportfunktion in DaVinci.

### So gehen Sie vor

1. Wählen Sie über `Plan > Importieren und Exportieren > Exportieren > Export für Schulportal Hessen` aus und klicken Sie auf `Weiter`.

2. Geben Sie nun über das Eingabefeld `Export Zielordner` den Zielordner an, in dem Datei gespeichert werden soll. Klicken Sie auf `Weiter`, um den Export zu starten.

3. Geben Sie beim Zeitraum bitte den zu exportierenden Zeitraum für die Vertretungsdaten an.

![Import/Export-Assistent, Schulportal Hessen](/assets/images/regionales/sshot11.png)

4. Das Ergebnis ist eine Datei mit dem Namen **vertretungsplan.csv**.

5. Diese Datei enthält folgende Informationen:

Spalte | Inhalt
-|-
Tag| Datum der Fehlzeit bzw. Vertretungsinfomration
Lehrer| Originallehrer
Stunde|Stunde laut Zeitrahmen
Klasse| betroffene Klasse
Art | Art der Änderung (Änderung, Aufsicht, Klasse fehlt; Mitteilung)
Vertreter| Vertretungslehrer
Fach|Vertretungsfach
Raum| Vertretungsraum
Hinweis Raum_alt| Originalraum
Fach_alt |Originalfach
Klasse_alt| betroffene Klasse
Hinweis2|Textfeld einer Mitteilung
Lerngruppe|

Diese Export Datei (vertretungsplan.csv) müssen Sie nun noch ins Schulportal HESSEN hochladen.

## Weitere Hinweise

Im Zeitrahmen der Stunden und Aufsichten sind nur ganze Zahlenwerte erlaubt, d.h. dass die Eingabe von Werten wie z.B. 1/2 als Stunden- oder Aufsichtsbezeichnungen und Positionen nicht möglich sind.