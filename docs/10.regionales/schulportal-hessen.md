# Schulportal HESSEN

In DAVINCI ist ein manueller Upload der Stunden- und Aufsichtplandaten sowie der Vertretungsdaten ins Schulportal HESSEN integriert. Das Schulportal HESSEN ist ein Service, der von der _Hessischen Lehrkräfteakademie_ den Schulen zur Verfügung gestellt wird.

## Export der Stunden- und Aufsichtspläne für das Schulportal Hessen 

Im Schulprotal HESSEN kann die Datei des XML-Exports aus DAVINCI ausgewertet werden. Der XML-Export enthält den Stunden- und Aufsichtsplan aus DAVINCI. Um die Daten im Schulportal HESSEN anzeigen zu lassen, muss der Export der XML-Datei aus Sicht aller Wochen erfolgen. Hier werden jedoch aktuell keine Informationen über die Perioden übergeben.

Da die Funktion des Exportes der DAVINCI Daten in eine XML-Datei zukünftig nicht mehr unterstützt wird, ist das Einlesen einer JSON Datei (über den Export aus DAINCI) ins Schulportal HESSEN geplant. Über den JSON Export werden die Daten wochenweise übergeben und enthalten somit Informationen über periodisch stattfindende Veranstaltungen.

### DAVINCI XML-Daten exportieren

1. Wählen Sie über `Plan > Importieren und Exportieren > Exportieren > DAVINCI XML-Daten exportieren` aus und klicken Sie auf `Weiter`.

2. Geben Sie im Bereich `Datei` über das Eingabefeld die Datei an, in die Sie die Daten exportieren wollen. Im Bereich `Zeitraum` wählen Sie `alle Wochen` aus. Klicken Sie auf `Weiter`.

![Import/Export-Assistent, DAVINCI XML-Daten exportieren](/assets/images/regionales/sshot12.png)

Diese DAVINCI XML-Export Datei müssen Sie nun noch in das Schulprotal HESSEN hochladen.

## Export der Vertretungspläne für das Schulportal HESSEN

Um Vertretungsplaninformationen aus DAVINCI in das Schulportal HESSEN zu übergeben, nutzen Sie bitte die dafür eingebaute Exportfunktion in DAVINCI.

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