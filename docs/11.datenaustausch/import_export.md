# Datenaustausch

## Importieren

### Vom externen Kalender synchronsisieren

Der Ablauf ist hier beschrieben:
[Nach externen Kalender synchronsisieren](/01.stundenplan/kalender/#termine-mit-outlookgoogle-synchronisieren)

### Von Magellan importieren

Der Ablauf ist hier beschrieben:
[Datenaustausch mit Magellan](/11.datenaustausch/magellan/)

### DaVinci Änderungen für den Planwechsel importieren

![DaVinci Änderungen für den Planwechsel importieren](/assets/images/Datenaustausch/export12.png)

* Importdatei: Geben Sie hier die Datei an, aus der Sie die Daten importieren möchten. Importiert werden Vertretungsplaninformatione. Dazu gehören Lehrer-Fehlzeiten und Anrechnungen.

### DaVinci Schuldatentransferdatei importieren

Der Ablauf ist hier beschrieben:

[Schuldatentransferformat](/11.datenaustausch/sdtf/)

### DaVinci Schlüsseldatei importieren

![DaVinci Schlüsseldatei importieren](/assets/images/Datenaustausch/export13.png)

Hier können Sie Schlüsseldateien für DaVinci importieren. Sie können dabei entscheiden, ob Einträge mit identischen Ürzel oder Schlüssel ersetzt werden.

### Hessen LUSD importieren

Der Ablauf ist hier beschrieben:
[Statistik Hessen](/10.regionales/hes-lusd/)

### Bayern ASV importieren

Der Ablauf ist hier beschrieben:
[Statistik Bayern](/10.regionales/bayern/)

### Bayern WinLD importieren

Der Ablauf ist hier beschrieben:
[Statistik Bayern](/10.regionales/bayern/)

### Sachsen Fachdaten importieren

Das Vorgehen ist hier beschrieben:
[Sachsen Fachdaten importieren](/10.regionales/sac-ausfallstatistik/)

### ASC Timetable XML 2012 importieren

Der Ablauf ist hier beschrieben:
![ASC Timetable XML 2012 importieren](/assets/images/Datenaustausch/export14.png)

### Meinen externen Kalender synchronisieren

Über diesen Aufruf können Sie Ihreeingetragenen unterrichtstermine in eine externen Kalender übertragen:
![Meinen externen Kalender synchronisieren](/assets/images/Datenaustausch/synchronisieren.png)

Wählen Sie Ihr Kürzel aus und den entsprechenden Kalenderdienst.

## Exportieren

### Nach externen Kalender synchronsisieren

Der Ablauf ist hier beschrieben:
[Nach externen Kalender synchronsisieren](/01.stundenplan/kalender/#termine-mit-outlookgoogle-synchronisieren)

### Nach Magellan exportieren

Der Ablauf ist hier beschrieben:
[Datenaustausch mit Magellan](/11.datenaustausch/magellan/)

### Statistikdaten exportieren

![Statistikdaten exportieren](/assets/images/Datenaustausch/export11.png)

Das Ergebnis ist eine Textdatei (.txt), die dem Schuldatentransferformat entspricht.

#### Allgemeines Statistikformat exportieren

![Allgemeines Statistikformat exportieren](/assets/images/Datenaustausch/export11.png)

#### Statistik Bremen Unterrichtsausfall exportieren

Der Ablauf ist hier beschrieben:
[Statistik Bremen](/10.regionales/bremen/)

#### Statistik Bayern (ASV) exportieren

Der Ablauf ist hier beschrieben:
[Statistik Bayern](/10.regionales/bayern/)

Der Ablauf ist hier beschrieben:
#### Statistik Bayern (WinLD) exportieren

Der Ablauf ist hier beschrieben:
[Statistik Bayern](/10.regionales/bayern/)

#### Statistik Hessen (LUSD) exportieren

Der Ablauf ist hier beschrieben:
[Statistik Hessen](/10.regionales/hes-lusd/)

#### Statistik Niedersachsen BBS exportieren

Der Ablauf ist hier beschrieben:
[Statistik Niedersachsen](/10.regionales/niedersachsen/)

#### Statistik Nordrhein-Westfalen ABS (Extern.dat) exportieren

Der Ablauf ist hier beschrieben:
[Statistik Nordrhein-Westfalen](/10.regionales/nordrhein-westfalen/)

#### Statistik Nordrhein-Westfalen BBS (Extern.dat) exportieren

Der Ablauf ist hier beschrieben:
[Statistik Nordrhein-Westfalen](/10.regionales/nordrhein-westfalen/)

#### Statistik Nordrhein-Westfalen GPC exportieren

Der Ablauf ist hier beschrieben:
[Statistik Nordrhein-Westfalen](/10.regionales/nordrhein-westfalen/)

#### Statistik Rheinland Pfalz (auch edoo.sys) exportieren

Der Ablauf ist hier beschrieben:
[Statistik Rheinland Pfalz (auch edoo.sys)](/10.regionales/rlp-edoosys/)

#### Statistik Schleswig Holstein

Der Ablauf ist hier beschrieben:
[Statistik Schleswig Holstein](/10.regionales/schleswig-holstein/)

### DaVinci Schuldatentransferdatei exportieren

![DaVinci Schuldatentransferdatei exportieren](/assets/images/Datenaustausch/export9.png)

Der Ablauf ist hier beschrieben:

 [Schuldatentransferformat](/11.datenaustausch/sdtf/)

### DaVinci XML-Daten exportieren

!!! info "Hinweis"

    Diese Funktion wird zukunftig nicht mehr unterstützt. Verwenden Sie bittestattdessen `DaVinci JSON-Daten exportieren`.

![DaVinci XML-Daten exportieren](/assets/images/Datenaustausch/export8.png)

* Datei: Geben Sie die Datei an, in die Sie Daten exportieren wollen: Das Ergebis ist hier eine Datei mit der Endung .xml

* Zieladresse: in den DaVinci Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatische beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

* Zeitraum: Auswahl des zu exportierenden Zeitraumes

* Auswahl: Wählen Sie, ob Sie Alle Daten oder Klasse, Lehrer, Schüler exportieren möchten. Sie können zusätzlich wählen ob Termine, Änderungen, Fehlzeiten, Kalendereinträge, Schülernamen und Vertretungsinformationen mitexportiert werden sollen.

### DaVinci JSON-Daten exportieren

![DaVinci JSON-Daten exportieren](/assets/images/Datenaustausch/export1.png)

* Geben Sie die Datei an, in die Sie Daten exportieren wollen: Das Ergebis ist hier eine Datei mit der Endung .json

* Zieladresse: in den DaVinci Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatische beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

* Zeitraum: Auswahl des zu exportierenden Zeitraumes

* Auswahl: Wählen Sie, ob Sie Alle Daten oder Klasse, Lehrer, Schüler exportieren möchten. Sie können zusätzlich wählen ob Termine, Änderungen, Fehlzeiten, Kalendereinträge, Schülernamen mitexportiert werden sollen.

### DaVinci Benutzerdaten exportieren

![DaVinci Benutzerdaten exportieren](/assets/images/Datenaustausch/export7.png)

Dieser Export benötigen Sie zur Einrichtung der Benutzerrechte im DaVinci Explorer. Die in DaVinci erzeugten Benutzernamen für Schüler, Klassen oder Lehrer können exportiert und im DaVinci-Explorer wieder importiert werden.

* Datei: Geben Sue due Datei an, in die Sie die Daten exportieren wollen. Geben Sie hier Namen und Speichertort einer Textdatei (.txt) an.
  
* Auswahl: Wahlweise können die Benutzerdaten für Klassen, Lehrer und/oder Schüler in eine Textdatei exportiert werden.

### Upload allgemein

![Upload allgemein](/assets/images/Datenaustausch/export6.png)

Geben Sie hier bitte die Zieladresse für den Upload nach Webweaver ein. Klicken Sie dazu auf `Verbindungsdetails` und Sie gelangen in die DaVinci Optionen.

In den DaVinci Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatisch beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

### Upload nach Webweaver

![Upload nach Webweaver](/assets/images/Datenaustausch/export2.png)

Geben Sie hier bitte die Zieladresse für den Upload nach Webweaver ein. Klicken Sie dazu auf `Verbindungsdetails` und Sie gelangen in die DaVinci Optionen.

In den DaVinci Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatisch beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/Datenaustausch/export2.png)

### Export für Schulportal Hessen

Die Informationen zum Upload nach LANiS finden Sie hier:

[Export für Schulportal Hessen](/10.regionales/schulportal-hessen/)
