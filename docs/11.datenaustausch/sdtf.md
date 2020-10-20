# Datenaustausch

DAVINCI speichert die Daten im XML-Format ab. Auf diese Daten können Sie mit jedem Text- oder XML-Editor zugreifen. DAVINCI bietet darüber hinaus verschiedene integrierte Möglichkeiten, Daten für den Austausch mit anderen Programmen zu importieren und zu exportieren. Lesen Sie dazu das Kapitel [Regionales](https://doc.davinci6.stueber.de/10.regionales/allgemeines/).

Sie können Plandaten mit DAVINCI über das Schuldatentransferformat austauschen. Dateien im Schuldatentransferformat sind Textdateien, mit denen Sie Daten einerseits nach DAVINCI importieren und andererseits aus DAVINCI exportieren können. Das Schuldatentransferformat bildet z.B. die Grundlage für den Datenabgleich mit MAGELLAN, wird aber auch von anderen Softwareanbietern aus dem Bereich Schulverwaltung und Stundenplanung unterstützt.

Die Beschreibung des Schuldatentransferformats finden Sie [hier](https://doc.sdtf.stueber.de/).

## Schuldatentransferdatei exportieren

Um eine Schuldatentransferdatei aus DAVINCI zu exportieren, gehen Sie bitte folgendermaßen vor:

1. Klicken Sie im Menüband des Programmfensters auf die Schaltfläche `Plan` und wählen Sie im Planmenü den Befehl `Importieren und Exportieren`: der Assistent `Import/ Export-Assistent` wird geöffnet.

![Import/Export-Assistent](/assets/images/datenaustausch/datenaustausch1.png)
2. Markieren Sie auf der ersten Assistentenseite im Bereich `Exportieren` den Eintrag `DAVINCI Schuldatentransferdatei exportieren` und bestätigen Sie Ihre Auswahl mit `Weiter`.
3. Klicken Sie im Bereich `Datei` der nächsten Assistentenseite auf die Schaltfläche `Datei auswählen`. Wählen Sie im Explorerfenster `Öffnen` das Zielverzeichnis der Exportdatei aus und geben Sie den gewünschten Dateinamen ein. Bestätigen Sie Ihre Angaben im Explorerfenster Öffnen mit `Öffnen`: der Dateipfadname der Exportdatei wird nun im Bereich `Datei` der Assistentenseite `daVinci-Schuldatentransferdatei exportieren` hinterlegt
4. Aktivieren Sie im Bereich `Weitere Angaben` die gewünschten Optionen für den Export der DAVINCI-Daten in die Exportdatei:
   * `Veranstaltungen und Blöcke exportieren`: Mit dieser Option werden die Veranstaltungs- und Termindaten in die Schuldatentransferdatei übertragen.
   * `Stammdaten exportieren`: Mit dieser Option werden die Daten aus den Stammdatenlisten in die Schuldatentransferdatei übertragen
   * `Schüler exportieren`: Mit dieser Option werden die Schüler der Oberstufe einschließlich der bei diesen hinterlegten Fach- bzw. Kurswahlen in die Exportdatei übertragen. Diese Option ist nur relevant, wenn Sie mit DAVINCI KURSPLAN arbeiten.
5. Setzen Sie optional den Haken bei `Schulnummer beachten` und tragen Sie im neben stehenden Eingabefeld die gewünschte Schulnummer ein, um die exportierten Daten, auf Klassen der zugehörigen Schulnummer einzuschränken. Bestätigen Sie Ihre Angaben mit `Weiter`.

Die Exportdatei wird nun entsprechend der vorgenommenen Einstellungen erzeugt. Den Fortschritt des Datenexports können Sie anhand des grünen Fortschrittsbalkens im Dialogfenster `Exportieren` erkennen.

## Schuldatentransferdatei importieren

Um eine Schuldatentransferdatei aus DAVINCI zu exportieren, gehen Sie bitte folgendermaßen vor:

1. Klicken Sie im Menüband des Programmfensters auf die Schaltfläche `Plan` und wählen Sie im Planmenü den Befehl `Importieren und Exportieren`: der Assistent `Import/ Export-Assistent` wird geöffnet.
2. Markieren Sie auf der ersten Assistentenseite im Bereich `Importieren` den Eintrag `DAVINCI-Schuldatentransferdatei importieren`, bestätigen Sie Ihre Auswahl mit `Weiter`.
3. Klicken Sie im Bereich `Datei` der nächsten Assistentenseite auf die Schaltfläche `Datei auswählen`. Wählen Sie im Explorerfenster `Öffnen` die gewünschte Importdatei aus. Bestätigen Sie Ihre Auswahl im Explorerfenster `Öffnen` mit Öffnen: der Dateipfadname der Importdatei wird nun im Bereich `Datei` der Assistentenseite `DAVINCI-Schuldatentransferdatei importieren` hinterlegt
4. Aktivieren Sie im Bereich `Weitere Angaben` die gewünschten Optionen für den Import der DAVINCI-Daten in die Exportdatei:
   
|Auswahl | Bedeutung|
|---|---|
|`Veranstaltungen und Blöcke importieren`|Veranstaltungen und Blöcke importieren: Mit dieser Option werden die Veranstaltungs- und Termindaten aus der Schuldatentransferdatei in die daVinci-Datei übertragen.|
|`Stammdaten importieren` | Mit dieser Option werden die Stammdaten aus der Schuldaten-transferdatei in die DAVINDA-Datei übertragen.|
|`Schülerdaten importieren`| Mit dieser Option werden die Schülerdaten der Oberstufe einschließlich der bei diesen hinterlegten Fach- bzw. Kurswahlen in die DAVINCI-Datei übertragen. Diese Option ist nur relevant, wenn Sie mit DAVINCI KURSPLAN arbeiten.|
|`In gleiche Blockbezeichner importieren` | Um anzugeben, das die Veranstaltungs- und Ter-mindaten aus der Schuldatentransferdatei mit den dort hinterlegten Blockkürzeln in die da-Vinci-Datei übertragen werden. Falls dieser Haken nicht gesetzt ist, wird für die in der Schul-datentransferdatei angelegten Blockkürzel beim Einspielen in daVinci ein neues Blockkürzel vergeben.|
|`Sperrungen importieren` | Mit dieser Option werden die in der Schuldatentransferdatei angelegten Sperrungen in die DAVINCI-Datei übertragen.
4. Wählen Sie im unteren Bereich über das entsprechende Aufklappemenü aus folgenden Optionen aus:
   
|Auswahl | Bedeutung|
|---|---|
|`Alle Feldinhalte (auch leere) importieren` ODER `Leere Feldinhalte ignorieren, gefüllte ersetzen` | |
|`Datensatz über Kürzel identifizieren` ODER `Datensatz über ID identifizieren` ODER `Datensatz über ID identifizieren, Kürzel nicht überschreiben`||

![Importieren und Exportieren-Assistent](/assets/images/KP/datenabgleich2.png)

5. Bestätigen Sie Ihre Angaben mit `Weiter`. Die Daten werden nun entsprechend der vorgenommenen Einstellungen in die DAVINCI-Datei übertragen. Den Fortschritt des Datenimports können Sie anhand des grünen Fortschrittsbalkens im Dialogfenster `Importieren` erkennen.

!!! warning "Wichtig"

    Falls beim Importieren der Termindaten aus der Schuldatentransferdatei Überschneidungen mit bereits existierenden Terminen in der DAVINCI-Datei auftreten, so werden die betroffenen Termindaten nicht in die DAVINCI-Datei eingelesen. Die nicht eingelesenen Termine werden mit Klassen- und Fachkürzel im Dialogfenster „Importieren“ angezeigt.
