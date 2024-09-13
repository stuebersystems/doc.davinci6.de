# Was ist neu

Dieses Kapitel gibt ihnen einen Überblick über aktuelle Änderungen in DaVinci 6 und in der DaVinci WebBox.

* Den Änderungsverlauf aus den vergangenen Jahren finden Sie hier: [2021](changelog-2021.md)[2020](changelog-2020.md), [2019](changelog-2019.md), [2018](changelog-2018.md), [2017](changelog-2017.md),  [2016](changelog-2016.md), [2015](changelog-2015.md), [2014 und früher](changelog-archive.md).

## Wichtige Hinweise

!!! danger "Achtung"

    **OpenSSL-Schwachstelle**: In unseren Softwareprodukten setzen wir kein OpenSSL ein.

    **Log4Shell-Schwachstelle**: Unsere Software-Produkte Enbrea, DaVinci, Magellan, CONFIRE SHOWTIME und CONFIRE SHERLOCK sind alle nicht von der Log4Shell-Schwachstelle betroffen, da keines dieser Produkte Java verwendet oder von einer externen Java-Anwendung abhängig ist. Auch unsere öffentlich zugänglichen Dienste (z.B. Ticketsystem, Webseiten) nutzen alle kein Java. Bitte lesen Sie auch unseren [Blogeintrag](https://blog.stueber.de/posts/log4j-desaster).

## LEGENDE

Abkürzung  |  Bedeutung
---------- | ----------
FIX |  Korrektur bestehender Funktionalität
NEW |  Neue Funktionalität  
CHANGE|  Änderung des Ablaufs, Verarbeitung oder Bedienung

---
## DaVinci Webbox v1.10.8 (unveröffentlicht)

* NEW: Separate Spalte in der Ansicht "Alle Klassen" zu Anzeige der Mitteilungen für "Alle Klassen/Lehrer" oder "Alle Klassen"

## DaVinci Version 6.5.91 (13.09.2024)

#### DaVinci Konsole

* FIX: Problem beim Übertrag von Plandaten/Vertretungsdaten mit neuem Hauptzeitraum gelöst

### Allgemein

* CHANGE: `13_NRW_Lehrer-Soll-Schlüssel.txt` Schlüsselwerte ergänzt
* FIX: `Stammdaten > Lehrer > Details > Keine Aufsicht` Eintrag kann wieder gelöscht uns gespeichert werden
* CHANGE: `Export > Statistik > Schulportal Hessen` Export der Aufsichten erweitert um den Aufischtsbereich, dieser wir din der Spalte Raum ausgegeben

### Vertretungsplan

* FIX: beim Vorziehen von Veranstaltungen mit Kursnummer wird auch die Kursnummer mit vorgezogen
* FIX: Ausgabe in `Vertretungsplan > Änderungsliste > Fach` korrigiert

### DaVinci Look

* FIX: `Extras > Otionen > Plananzeige > Änderungen` neue Änderungen werden wie gekennzeichnet dargestellt

## DaVinci Version 6.5.90 (25.07.2024)

### Allgemein

* CHANGE: Icons, Symbole und Splashscreens

### Enbrea

* FIX: Datenübertrag nach Enbrea: Export von Vertretungsplaninfos auch über den Planungszeitraum hinaus möglich.

## DaVinci Version 6.5.89 (10.04.2024)

### Allgemein

* NEW: Neue Dateien für Schulferien und Feiertage für alle Bundesländer. Sie können die Kalenderdateien auch bereits vorab [hier](https://my.hidrive.com/share/63dd-bod4u) herunterladen, müssten nach dem Import in ältere Ausgaben (vor 6.5.89) bitte unter `Kalender > Ereignisse` bitte jeweils das Häkchen für `unterrichtsfrei` aktivieren.

### Enbrea

* FIX: Für den Übertrag nach ENBREA Änderungen beim `Vertretungsplan > Zusatzunterricht` 

### Stundenplan

* CHANGE: interne Änderung für den Einleseprozess für die Importdateien Schulferien und Feiertage

### Vertretungsplan

* FIX: Bei der Funktion "Wie Woche zuvor" werden auch die Werte aus den Feldern `Info` und `Mitteilung` übernommen

## DaVinci Version 6.5.88 (04.03.2024)

### Vertretungsplan

* NEW: In der Anicht `Vertretungen > Vertretungen` steht zum Ändern der Fächer im Vertretungseinsatz ein Teamfilter zur Verfügung. Dieser basiert auf den Eintragungen unter `Stammdaten > Fächer > Teams`
* FIX: `Vertretungen > Stundenplan > Fach ändern` der Teamfilter beim Ändern des Faches wird berücksichtigt
* FIX: Vorziehoptionen vom gleichen Tag (Tag der Eintragung) als direkte Vertretung

## DaVinci Version 6.5.87 (22.02.2024)

### DaVinci Server

* FIX: Sicherheitslücke in Kombination mit DaVinci WebBox und DaVinci Mobile in DaVinci-Server geschlossen. Bei Einsatz des DaVinci INFOSERVERs bitte unbedingt den DaVinci Server aktualisieren!

## DaVinci WebBox Version 1.10.7 (22.02.2024)

[**Update-Anleitung**](https://doc.DaVinci6.stueber.de/09.infoserver/update/) <br/>
[**Download**](https://DaVinci-webbox.stueber.de/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DaVinci Look und der DaVinci WebBox: [Welche Vertretungsinformationen werden für Look oder die WebBox publiziert?](https://doc.DaVinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Sicherheitslücke in Kombination mit DaVinci WebBox und DaVinci Mobile in DaVinci-Server geschlossen. Bei Einsatz des DaVinci INFOSERVERs bitte unbedingt den DaVinci Server aktualisieren!

## DaVinci WebBox Version 1.10.6 (18.10.2023)

[**Update-Anleitung**](https://doc.DaVinci6.stueber.de/09.infoserver/update/) <br/>
[**Download**](https://DaVinci-webbox.stueber.de/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DaVinci Look und der DaVinci WebBox: [Welche Vertretungsinformationen werden für Look oder die WebBox publiziert?](https://doc.DaVinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Der Parameter `substitutionShowExtra` wurde korrigiert
* NEW: Die Bezeichnung des Klassenfehlgrunds wird am oberen Rand des Terminfensters hinter der Info "Klassen fehlt" eingeblendet. Ein Beispiel: "Klasse fehlt: Distanzunterricht"

## DaVinci Version 6.5.86 (24.01.2024)

### Allgemein

* FIX: `Importieren > Exportieren > Export für Schulportal Hessen` 
* CHANGE: Abgleich mit Magellan 11 wurde ermöglicht

### Vertretungsplan

* FIX: Vorziehoptionen vom gleichen Tag als direkte Vertretung