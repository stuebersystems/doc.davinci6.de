# Datenaustausch

## Importieren

### Vom externen Kalender synchronsisieren

[Nach externen Kalender synchronsisieren](/01.stundenplan/kalender/#termine-mit-outlookgoogle-synchronisieren)

### Von MAGELLAN importieren

[Datenaustausch mit MAGELLAN](/10.regionales/11.datenaustausch/magellan/)

### DAVINCI Änderungen für den Planwechsel importieren

![DAVINCI Änderungen für den Planwechsel importieren](/assets/images/Datenaustausch/export12.png)

* Importdatei: Geben Sie hier die Datei an, aus der Sie die Daten importieren möchten. Importiert werden Vertretungsplaninformatione. Dazu gehören Lehrer-Fehlzeiten und Anrechnungen.

### DAVINCI Schuldatentransferdatei importieren

Der Ablauf ist hier beschrieben:

[Schuldatentransferformat](/11.datenaustausch/sdtf/)

### DAVINCI Schlüsseldatei importieren

![DAVINCI Schlüsseldatei importieren](/assets/images/Datenaustausch/export13.png)

Hier können Sie Schlüsseldateien für DAVINCI importieren. Sie können dabei entscheiden, ob Einträge mit identischen Ürzel oder Schlüssel ersetzt werden.

### Hessen LUSD importieren

[Statistik Hessen](/10.regionales/hes-lusd/)

### Bayern ASV importieren

[Statistik Bayern](/10.regionales/bayern/)

### Bayern WinLD importieren

[Statistik Bayern](/10.regionales/bayern/)

### Sachsen Fachdaten importieren

Das Vorgehen ist hier beschrieben:

[Sachsen Fachdaten importieren](/10.regionales/sachsen/)

### ASC Timetable XML 2012 importieren

![ASC Timetable XML 2012 importieren](/assets/images/Datenaustausch/export14.png)

### Meinen externen Kalender synchronisiseren

## Exportieren

### Nach externen Kalender synchronsisieren

Der Ablauf ist hier beschrieben:

[Nach externen Kalender synchronsisieren](/01.stundenplan/kalender/#termine-mit-outlookgoogle-synchronisieren)

### Nach MAGELLAN exportieren

Der Ablauf ist hier beschrieben:

[Datenaustausch mit MAGELLAN](/10.regionales/11.datenaustausch/magellan/)

### Statistikdaten exportieren

![Statistikdaten exportieren](/assets/images/Datenaustausch/export11.png)

Das Ergebnis ist eine Textdatei (.txt), die dem Schuldatentransferformat entspricht.

#### Allgemeines Statistikformat exportieren

![Allgemeines Statistikformat exportieren](/assets/images/Datenaustausch/export11.png)

#### Statistik Bremen Unterrichtsausfall exportieren

[Statistik Bremen](/10.regionales/bremen/)

#### Statistik Bayern (ASV) exportieren

[Statistik Bayern](/10.regionales/bayern/)

#### Statistik Bayern (WinLD) exportieren

[Statistik Bayern](/10.regionales/bayern/)

#### Statistik Hessen (LUSD) exportieren

[Statistik Hessen](/10.regionales/hes-lusd/)

#### Statistik Niedersachsen BBS exportieren

[Statistik Niedersachsen](/10.regionales/niedersachsen/)

#### Statistik Nordrhein-Westfalen ABS (Extern.dat) exportieren

[Statistik Nordrhein-Westfalen](/10.regionales/nordrhein-westfalens/)

#### Statistik Nordrhein-Westfalen BBS (Extern.dat) exportieren

[Statistik Nordrhein-Westfalen](/10.regionales/nordrhein-westfalen/)

#### Statistik Nordrhein-Westfalen GPC exportieren

[Statistik Nordrhein-Westfalen](/10.regionales/nordrhein-westfalen/)

#### Statistik Rheinland Pfalz (auch edoo.sys) exportieren

[Statistik Rheinland Pfalz (auch edoo.sys)](/10.regionales/rlp-edoosys/)

#### Statistik Schleswig Holstein

Der Ablauf ist hier beschrieben:

 [Statistik Schleswig Holstein](/10.regionales/schleswig-holstein/)

### DAVINCI Schuldatentransferdatei exportieren

![DAVINCI Schuldatentransferdatei exportieren](/assets/images/Datenaustausch/export9.png)

Der Ablauf ist hier beschrieben:

 [Schuldatentransferformat](/11.datenaustausch/sdtf/)

### DAVINCI XML-Daten exportieren

!!! info "Hinweis"

    Diese Funktion wird zukunftig nicht mehr unterstützt. Verweden Sie stattdessen `DAVINCI JSON-Daten exportieren`.

![DAVINCI XML-Daten exportieren](/assets/images/Datenaustausch/export8.png)

* Datei: Geben Sie die Datei an, in die Sie Daten exportieren wollen: Das Ergebis ist hier eine Datei mit der Endung .xml

* Zieladresse: in den DAVINCI Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatische beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

* Zeitraum: Auswahl des zu exportierenden Zeitraumes

* Auswahl: Wählen Sie, ob Sie Alle Daten oder Klasse, Lehrer, Schüler exportieren möchten. Sie können zusätzlich wählen ob Termine, Änderungen, Fehlzeiten, Kalendereinträge, Schülernamen und Vertretungsinformationen mitexportiert werden sollen.

### DAVINCI JSON-Daten exportieren

![DAVINCI JSON-Daten exportieren](/assets/images/Datenaustausch/export1.png)

* Geben Sie die Datei an, in die Sie Daten exportieren wollen: Das Ergebis ist hier eine Datei mit der Endung .json

* Zieladresse: in den DAVINCI Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatische beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

* Zeitraum: Auswahl des zu exportierenden Zeitraumes

* Auswahl: Wählen Sie, ob Sie Alle Daten oder Klasse, Lehrer, Schüler exportieren möchten. Sie können zusätzlich wählen ob Termine, Änderungen, Fehlzeiten, Kalendereinträge, Schülernamen mitexportiert werden sollen.

### DAVINCI Benutzerdaten exportieren

![DAVINCI Benutzerdaten exportieren](/assets/images/Datenaustausch/export7.png)

Dieser Export benötigen Sie zur Einrichtung der benutzerrechte im DAVINCI Explorer. Die in DAVINCI erzeugten Benutzernamen für Schüler, Klassen oder Lehrer können exportiert und im DAVINCI-EXPLORER wieder importiert werden.

* Datei: Geben Sue due Datei an, in die Sie die Daten exportieren wollen. Geben Sie hier Namen und Speichertort einer Textdatei (.txt) an.
  
* Auswahl: Wahlweise können die Benutzerdaten für Klassen, Lehrer und/oder Schüler in eine Textdatei exportiert werden.

### Upload allgemein

![Upload allgemein](/assets/images/Datenaustausch/export6.png)

Geben Sie hier bitte die Zieladresse für den Upload nach Webweaver ein. Kleicken Sie dazu auf `Verbindungsdetails` und Sie gelangen in die DAVINCI Optionen.

In den DAVINCI Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatische beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

### Upload nach Webweaver

![Upload nach Webweaver](/assets/images/Datenaustausch/export2.png)

Geben Sie hier bitte die Zieladresse für den Upload nach Webweaver ein. Kleicken Sie dazu auf `Verbindungsdetails` und Sie gelangen in die DAVINCI Optionen.

In den DAVINCI Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatische beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

### Export für Schulportal Hessen

Die Informationen zum Upload nach LANiS finden Sie hier:

[Export für Schulportal Hessen](/11.regionales/schulportal-hessen.md/)
