# Erste Schritte in DAVINCI

## Programm starten

Durch die [Installation](https://doc.davinci6.stueber.de/00.allgemein/installation/) von DAVINCI wird nicht automatisch eine Verknüpfung auf den Desktop erstellt.  Öffnen Sie DAVINCI daher über `Start > Alle Programme > Stueber Systems`. Sie können mit einem Rechtsklick auf die Symbole im Startmenü selbstständig eine Desktopverknüpfung anlegen, wenn Sie dies wünschen.

## Plan-Eigenschaften

![Plan Eigenschaften](/assets/images/Plan-Eigenschaften.png)

Das Dialogfenster  `Plan > Eigenschaften` gibt Ihnen Informationen zur aktuellen Plandatei und erlaubt einige wichtige Datei-Einstellungen, auf die wir in den entsprechenden Abschnitten näher eingehen werden.

!!! info "Hinweis"

    Die Einstellungen im Dialogfenster `Plan > Eigenschaften` werden in der DAVINCI Datei abgelegt.

!!! info "Hinweis"

    Die Einstellungen im Dialogfenster `Extras > Optionen` werden benutzerspezifisch gespeichert.

## DAVINCI Optionsdateien

DAVINCI  verwendet diverse Optionsdateien. Die Ordner, in denen diese Dateien liegen, sind teilweise spezifisch für die Betriebssystemversion bzw. den Benutzer. Sie werden durch das DAVINCI Installationsprogramm automatisch entsprechend der Betriebssystemkonventionen festgelegt. Die genauen Namen und Pfadangaben dieser Dateien können Sie dem Fenster `Hilfe > System-Informationen` entnehmen.

| Optionsdatei | Beschreibung |
| --- | --- |
| daVinciLogo.png | Kundenlogo zum Einbinden in DAVINCI |
| daVinci.cfg | Aktuelle Login-Daten für DAVINCI |
| daVinci.opt | Optionsdatei für DAVINCI |
| daVinci.hfm | HTML Exportformate |
| daVinci.lic | DAVINCI /DAVINCI Look Lizenzdaten |
| daVinci.pfm | DAVINCI /DAVINCI Look Druckformate |
| daVinci.site | Standortdaten (Schulname, Adresse, etc.) |
| daVinci.sms | SMS-Logbuch |
| daVinci.paths | [DAVINCI  Paths-Datei](https://doc.davinci6.stueber.de/00.allgemein/pathdatei/) |
| daVinciExplorer.opt | daVinci EXPLORER Optionsdatei |
| daVinciLook.cfg | Aktuelle Login-Daten für DAVINCI LOOK |
| daVinciLook.opt | Optionsdatei für DAVINCI LOOK |
| daVinciServer.opt | Optionsdatei |
| daVinciServer.cfg | Server-Konfiguration (Eigene IP-Adresse, etc.) |
| daVinci.servers | Server-Anmeldeinformationen und Serverstartdatei |

## Arbeitsumgebung kennenlernen

![Willkommensfenster](/assets/images/willkommen01.png)

Die Willkommensansicht, mit der DAVINCI beim ersten Programmstart geöffnet wird, vermittelt einen ersten Überblick über die Arbeitsumgebung. DAVINCI gliedert sich in sieben Programmbereiche, die für unterschiedliche Aufgaben zuständig sind. Jeder Programmbereich bietet eine speziell an die eigene Funktion angepasste Benutzeroberfläche.

| Bereich | Beschreibung |
| --- | --- |
| **Stammdaten** | Hier erfassen Sie die zentralen Akteure und Ressourcen, die Sie für die Unterrichtsplanung benötigen. Hier geben Sie z.B. Klassen, Lehrer, Fächer und Räume ein. |
|**Kalender**| Hier tragen Sie Termine in einer Kalenderansicht ein. Sie können hier Ereignisse, die keinen klassischen Unterrichtscharakter haben, hinterlegen. Außerdem können Sie hier Aufgaben eingeben und verwalten, die noch keinen direkten Terminbezug aufweisen.|  
| **Stundenplan**| Hier erstellen und bearbeiten Sie Unterrichtsveranstaltungen und legen die Termine fest, an denen diese Veranstaltungen stattfinden sollen. Mit einem grafischen Planeditor können Sie Veranstaltungen und Termine per Drag & Drop ver- oder entplanen.| 
| **Vertretungsplan**| In dieser Ansicht erstellen Sie die täglichen Planänderungen aufgrund fehlender Lehrer, Räume und Klassen und bestimmen Sie passende Vertreter.|
| **Kursplan**| Hier können Sie die Fachwahlen der Schüler erfassen und aufgrund dessen das Kursangebot erstellen. Anschließend können Sie die Kurse blocken und die Schüler auf die Kurse verteilen.|
| **Übersichten**| In den `Übersichten` erhalten Sie alle Listen und Berechnungen, die Sie hier gefiltert, gruppiert und/oder sortiert drucken oder exportieren können.
| **Ressourcenplan**| In dieser Ansicht können Sie Ihre beweglichen Ressourcen einsehen und an derzeit stattfindende Termine vergeben oder in Räume einbuchen.|

## Plandatei öffnen

Um eine DAVINCI Datei zu öffnen gehen Sie auf Plan und wählen die Datei entweder aus der Liste der bisher geöffneten Dateien aus oder Sie gehen auf `Plan > Öffnen` und wählen die Datei von Ihrem Computer oder einem Netzwerkpfad aus.

!!! info "Hinweis"

    Dateien, die mit der Version DAVINCI 6 erstellt werden, erhalten die Endung `.daVinci`

!!! info "Hinweis"

    Dateien, die Sie mit der Vorgängerversion DAVINCI 5 erstellt haben, tragen die Endung `.dav`. Beide Dateitypen können Sie direkt in DAVINCI 6 öffnen. Eine vorherige Konvertierung von `*.dav`-Dateien ist nicht erforderlich.

Bei der Installation von DAVINCI werden Beispieldateien auf Ihren Computer kopiert, die Sie für Tests nutzen können. Diese Beispieldateien werden standardmäßig unter folgendem Dateipfad auf Ihrem Computer gespeichert:
**Windows 8/10** ```C:\Users\Public\Documents\Stueber Systems\daVinci 6\Beispiele```

Die Beispieldatei können Sie öffnen, indem Sie auf der Willkommensseite die Schnellstart-Schaltfläche Beispiel öffnen betätigen. 

![Willkommensfenster - Beispiel Dateien](/assets/images/Bsp.DAteien.png)

!!! info "Hinweis"

    Sie können festlegen, dass bei jedem Programmstart eine bestimmte DAVINCI-Datei automatisch geöffnet wird. Klicken Sie dazu auf `Plan > DAVINCI Optionen` oder auf  `Extras > Optionen`, um das Dialogfenster ``Optionen`` und dort die Registerkarte Plandatei aufzurufen. Aktivieren Sie im Bereich ``Startdatei`` der Eingabeseite ``Plandatei`` die gewünschte Option:

| Auswahl | Beschreibung |
| --- |  --- |
|Immer ohne Plandatei starten | Mit dieser Option legen Sie fest, dass DAVINCI beim Programmstart ohne Datei geöffnet wird.|
|Immer mit Serveranmeldung starten | Wenn Sie DAVINCI ENTERPRISE nutzen, ist es nützlich DAVINCI direkt beim Start automatisch mit dem Server zu verbinden. Geben Sie in dem Dialogfenster bei ``Kennung und Kennwort``Ihre Anmeldedaten an, damit sich DAVINCI auch automatisch beim Programmstart am Server anmeldet.|
| Immer mit zuletzt geöffneter Plandatei starten | Mit dieser Option startet DAVINCI jeweils mit der Plandatei, die zuletzt auf dem Rechner zur Bearbeitung geöffnet war.|
| Immer mit der folgenden Plandatei starten | Geben Sie den Pfad zur gewünschten Plandatei im Textfeld an oder wählen Sie ihn unter Plandatei auswählen direkt aus.|

![Optionen](/assets/images/DAV.Optionen.PLandatei.png)

## Neue Plandatei anlegen

Für das Anlegen einer neuen Plandatei steht Ihnen in DAVINCI 6 ein eigener Programmassistent zur Verfügung. Den Planvorbereitungsassistenten können Sie aufrufen, indem Sie auf `Plan > Neu` klicken.

![Planvorbereitungsassistent](/assets/images/Planvorbereitungsassistent01.png)

Folgende Optionen werden Ihnen angeboten:

| Auswahl | Beschreibung |
| --- |  --- |
| Neuen leeren Plan erstellen | Sie können eine neue leere Plandatei anlegen, die keine Daten enthält. |
| Neuen Plan erstellen und Daten übernehmen | Sie können eine neue Plandatei anlegen und die Stamm-, Unterrichts- und Rahmendaten aus einer anderen DAVINCI-Datei übernehmen, zum Beispiel bei einem Schuljahreswechsel. Bei dieser Option wird Ihnen im folgenden Dialog angeboten,die Klassennummerierungen um eins zu erhöhen (z.B.: „8a“ wird zu „9a“).
| Neuen leeren Plan erstellen, aber aktuellen Planrahmen übernehmen | Sie können eine neue Plandatei anlegen, die nur die Rahmendaten der aktuell geöffneten DAVINCI-Datei enthält. Dabei werden alle Daten bis auf Fächer, Schlüsselverzeichnisse, Zeitrahmen und der Kalender gelöscht|

### Neuen Plan erstellen und Daten übernehmen (Schuljahreswechsel)

Markieren Sie ``Neuen Plan erstellen und Daten übernehmen`` wenn Sie auf eine Vorjahresplandatei zurückgreifen und Daten übernehmen möchten. Geben Sie an, aus welchem Plan Sie die Daten übernehmen möchten und klicken Sie auf ``Weiter``.

![Neuen Plan erstellen und Daten übernehmen](/assets/images/Neuen.Plan.erstellen.Daten.übernehmen.png)

Wählen Sie zwischen ``Neues Schuljahr`` oder ``Planwechsel innerhalb des Schuljahres`` und klicken Sie auf ``Weiter``. 

![Planvorbereitungsassistent "Neues Schuljahr"](/assets/images/Neuen.Plan.Neues.SJ.png)

Wählen Sie zwischen ``Unterrichtsverteilung und Aufsichten löschen`` oder ``Alles übernehmen`` und klicken Sie auf ``Weiter``. 

![Wählen Sie hier, ob Sie alle Daten übernehmen möchten oder nur eine Teilmenge](/assets/images/Neuen.Plan.Neues.SJ.Löschen.Übernehmen.png)

Anschließend gelangen Sie zu den wesentlichen Schritten der Planneuerstellung.

![Schritte der Planneuerstellung](/assets/images/Planvorbereitungsassistent03.png)

#### Schritt 1 - Zeitraum eingeben

Geben Sie den Zeitraum an, für den Ihr Plan gelten soll.

![Plan-Eigenschaften, Registerkarte "Zeitraum"](/assets/images/Plan-Eigenschaften01.png)

Registerkarte „Statistik“

* _Zeitdauerangaben_: Tragen Sie die zur Berechnung der Stundenangaben für die Statistik entsprechende Zeitdauer ein.
* _Wochenbezogene Summen_: Hier können Sie die Kalenderwochen kennzeichnen, in denen kein Unterricht stattfindet. Entfernen Sie im unteren Fenster den Haken bei den Wochen, in denen kein Unterricht stattfindet. Bitte den Haken nur vor ganzen Ferienwochen entfernen! Wichtig ist diese Angabe insbesondere, wenn Sie mit Perioden arbeiten oder eine wochenbezogene Berechnung der Unterrichtsstunden wünschen.
* _Verrechnungsart_: Wenn man im Zeitrahmen den Haken vor ``Termin-Ende beim Verplanen automatisch an Zeitrahmen anpassen`` gesetzt hat, kann man über die Option ``Mit Minuten pro Einheit`` laut Zeitrahmen anstatt realer Dauer laut Plan rechnen“ entscheiden, ob in der Summenbildung die Unterrichtsstunde als 45 min gewertet werden soll, oder die Dauer lt. Positionen (die ja abweichen, 40 min, 45 min) einfließen sollen.
* Die Option _Mit Wertfaktoren (aus Stundentafel, Fach, Klasse, Veranstaltung) _benötigen Sie, wenn Sie mit dem Hamburger Lehrerarbeitszeitmodell rechnen wollen. Nachträglich gelangen Sie über ``Plan > Eigenschaften > Statistik`` in dieses Menü.

![Plan-Eigenschaften, Registerkarte "Statistik"](/assets/images/Plan-Eigenschaften02.png)

#### Schritt 2 - Kalenderdaten importieren...

Laden Sie den Kalender für Ihr Bundesland, um die Ferien- und Feiertage zu importieren.

`…:\Users\Public\Documents\Stueber Systems\daVinci 6\Kalender`

![Kalender importieren](/assets/images/Kalender.Importieren.png)

#### Schritt 3 - Zeitrahmen einstellen

Registerkarte "Allgemein"

* Hier können Sie vorgeben, aus wie viel Positionen Ihr Tag besteht und welche Dauer eine Position hat.

![Zeitrahmen, Register "Allgemein"](/assets/images/Zeitrahmen.Allgemein01.png)

Registerkarte "Positionen":

* Bezeichnung: Standardmäßig so voreingestellt, können auch gerändert werden
* Beginn/Ende: geben Sie hier Beginn und Ende der einzelnen Stunden an
* Differenz: Wert errechnet sich automatisch aufgrund der eingetragenen Uhrzeiten bei „Beginn“ und „Ende“
* Trennlinie: zwischen den einzelnen Positionen können Sie Trennlinien einfügen, diese können auch im Ausdruck verwendet werden
* Doppelstunde: gesetzter Haken heißt für die Automatik, wann eine Doppelstunde beginnen darf, also von der Automatik verplant werden soll

![Zeitrahmen, Register "Positionen" , Register "Positionen" ](/assets/images/Zeitrahmen.Positionen01.png)

##### Aufsichten-Zeitrahmen

Registerkarte "Allgemein"

* Geben Sie im Feld "Positionen" die Anzahl der zu beaufsichtigenden Pausenzeiten ein.

Registerkarte "Positionen"

* Tragen Sie Beginn- und Endzeiten der zu beaufsichtigenden Pausen ein

![Aufsichten-Zeitrahmen](/assets/images/Zeitrahmen.Aufsichten.png)

!!! info "Hinweis"

    Das Zeitrahmen-Fenster können Sie jederzeit über den Menüpunkt ``Extras>Zeitrahmen`` öffnen. Bitte beachten Sie, den Zeitrahmen am gesetzten Plan nicht mehr zu verändern. 

### Neuen leeren Plan erstellen (für Neueinsteiger)

Um eine neue Plandatei mit DAVINCI 6 zu erstellen, rufen Sie den Planvorbereitungsassistenten über `Plan > Neu` auf.

Gehen Sie hier wie folgt vor:

* Markieren Sie ``Neuen leeren Plan`` da Sie zum ersten Mal Ihre Stundenplanung mit DAVINCI vornehmen.

![Planvorbereitunsassistent - Neuen leeren Plan erstellen](/assets/images/Neuen.leeren.Plan.png)

* Klicken Sie auf ``Weiter``.
* Bereiten Sie die Planerstellung für das neue Schuljahr mit Hilfe dieser Liste vor.
  
![Schritte der Planneuerstellung](/assets/images/Planvorbereitungsassistent02.png)

1. Zeitraum eingeben
2. Kalenderdaten importieren
3. Zeitrahmen einstellen
4. Stammdaten befüllen

## Datei speichern (im lokalen Betrieb)

### Sicherungskopie erstellen/wiederherstellen

Um bei jedem Speichern eine Sicherungskopie Ihrer Datei zu erstellen, öffnen Sie die Programm Optionen unter  `Plan > DAVINCI-Optionen` oder `Extras > Optionen` im Reiter `Plandatei`.

![DAVINCI Optionen - Backup](/assets/images/opt.sicherung.png)

Wählen Sie im unteren Drittel die Option ``Sicherungskopie (.Backup-Datei) der Datei anlegen`` wenn Sie im lokalen Betrieb (ohne den Einsatz von DAVINCI ENTERPRISE arbeiten). Nun wird bei jedem Speichern von Ihrer Datei eine Sicherungskopie angelegt, welche als Dateierweiterung das Datum und die Endung ``.BACKUP`` trägt.

!!! info "Hinweis"

    Ihre Sicherungskopie enthält den Namen Ihrer ursprünglichen Datei, das aktuelle Jahr, die Nummer des Tages im Jahr und die Endung ``.BACKUP``. (z.B. Beispiel.2018-04-20-00.backup)
    Um eine Sicherungskopie wieder herzustellen müssen Sie Ihre Datei im Windows-Explorer in eine ``*.daVinci`` Datei umbenennen. Löschen Sie dazu den Punkt, die Zahl und die .BACKUP-Endung.

Generell sollten Sie in regelmäßigen Abständen, mindestens täglich, externe Sicherungskopien Ihrer Daten erstellen. Dazu sollten Sie folgende Daten sichern:

Datei| Inhalt
 --- | ---
Ihre aktuelle .daVinci | Datei Ihr Stundenplan
daVinci.hfm | Exportformate Datei
daVinci.pfm | Druckformate Datei
daVinci.opt | Ihre persönlichen Einstellungen für Farben, Ansichten, Dialogfenster

Das Erstellen der externen Sicherungskopien sollte in die Cloud (das Internet), auf Bandlaufwerke oder auf USB-Sticks erfolgen.

!!! info "Hinweis"

    Sorgen Sie unbedingt dafür, dass mindestens einmal täglich Sicherungskopien Ihrer
Daten auf externe Datenträger erstellt  werden. Andernfalls können Sie z.B. in Folge eines Hardwarefehlers Ihre gesamten Daten verlieren.

### Datei automatisch speichern (im lokalen Betrieb)

Sie können festlegen, dass Ihre DAVINCI-Datei in einem bestimmten Zeitintervall automatisch gespeichert wird. Auch beim automatischen Speichern wird jedes Mal eine Sicherungskopie angelegt. Öffnen Sie die DAVINCI Optionen unter `Plan > DAVINCI-Optionen` oder `Extras > Optionen` im Reiter ``Plandatei`` und wählen die Option ``Automatische Sicherung der Daten nach X Minuten`` und tragen Sie ein, wie viele Minuten zwischen den Sicherungen liegen sollen.

![DAVINCI Optionen - Backup](/assets/images/opt.sicherung.png)

### Plandatei speichern

Um eine Plandatei in dem gewünschten Zielverzeichnis auf Ihrem Rechner zu speichern, klicken Sie auf  `Plan > Speichern unter` und wählen Sie DAVINCI-Datei. Sie haben darüber hinaus die Möglichkeit, eine DAVINCI-Datei in komprimierter Form, also mit deutlich reduzierter Dateigröße zu speichern. Dies bietet sich z.B. an, wenn Sie Ihre Datei per E-Mail versenden möchten. Wenn Sie diese Option wählen, wird Ihre DAVINCI-Datei mit der Endung ``.daVinci.zip`` als gezippte Datei gespeichert.
Eine ``*.daVinci.zip``-Datei kann mit DAVINCI geöffnet werden, ohne dass diese vorher mit einem externen Programm entpackt werden muss. Die gezippte Plandatei wird beim Öffnen mit DAVINCI automatisch entpackt und im Standardformat ``.daVinci`` geladen.

## Datei speichern (im Serverbetrieb)

Genauere Informationen dazu finden Sie im Teil [DAVINCI SERVER](https://doc.davinci6.stueber.de/06.enterprise/00.allgemeines/).
