# Was ist neu

Dieses Kapitel gibt ihnen einen Überblick über aktuelle Änderungen in DAVINCI 6 und in der DAVINCI WEBBOX.

* Den Änderungsverlauf aus den vergangenen Jahren finden Sie hier: [2021](changelog-2021.md)[2020](changelog-2020.md), [2019](changelog-2019.md), [2018](changelog-2018.md), [2017](changelog-2017.md),  [2016](changelog-2016.md), [2015](changelog-2015.md), [2014 und früher](changelog-archive.md).

## Wichtige Hinweise

!!! danger "Achtung"

    **OpenSSL-Schwachstelle**: In unseren Softwareprodukten setzen wir kein OpenSSL ein.

    **Log4Shell-Schwachstelle**: Unsere Software-Produkte ENBREA, DAVINCI, MAGELLAN, CONFIRE SHOWTIME und CONFIRE SHERLOCK sind alle nicht von der Log4Shell-Schwachstelle betroffen, da keines dieser Produkte Java verwendet oder von einer externen Java-Anwendung abhängig ist. Auch unsere öffentlich zugänglichen Dienste (z.B. Ticketsystem, Webseiten) nutzen alle kein Java. Bitte lesen Sie auch unseren [Blogeintrag](https://blog.stueber.de/posts/log4j-desaster).

## LEGENDE

Abkürzung  |  Bedeutung
---------- | ----------
FIX |  Korrektur bestehender Funktionalität
NEW |  Neue Funktionalität  
CHANGE|  Änderung des Ablaufs, Verarbeitung oder Bedienung

---
## DAVINCI Version 6.5.90 (unveröffentlicht)

### Allgemein

## DAVINCI Version 6.5.89 (10.04.2024)

### Allgemein

* NEW: Neue Dateien für Schulferien und Feiertage für alle Bundesländer. Sie können die Kalenderdateien auch bereits vorab [hier](https://my.hidrive.com/share/63dd-bod4u) herunterladen, müssten nach dem Import in ältere Ausgaben (vor 6.5.89) bitte unter `Kalender > Ereignisse` bitte jeweils das Häkchen für `unterrichtsfrei` aktivieren.
* FIX: Für den Übertrag nach ENBREA Änderungen beim `Vertretungsplan > Zusatzunterricht` 

### Stundenplan

* CHANGE: interne Änderung für den Einleseprozess für die Importdateien Schulferien und Feiertage

### Vertretungsplan

* FIX: Bei der Funktion "Wie Woche zuvor" werden auch die Werte aus den Feldern `Info` und `Mitteilung` übernommen

## DAVINCI Version 6.5.88 (04.03.2024)

### Vertretungsplan

* NEW: In der Anicht `Vertretungen > Vertretungen` steht zum Ändern der Fächer im Vertretungseinsatz ein Teamfilter zur Verfügung. Dieser basiert auf den Eintragungen unter `Stammdaten > Fächer > Teams`
* FIX: `Vertretungen > Stundenplan > Fach ändern` der Teamfilter beim Ändern des Faches wird berücksichtigt
* FIX: Vorziehoptionen vom gleichen Tag (Tag der Eintragung) als direkte Vertretung

## DAVINCI Version 6.5.87 (22.02.2024)

### DAVINCI SERVER

* FIX: Sicherheitslücke in Kombination mit DAVINCI WEBBOX und DAVINCI MOBILE in DAVINCI-Server geschlossen. Bei Einsatz des DAVINCI INFOSERVERs bitte unbedingt den DAVINCI SERVER aktualisieren!

## DAVINCI WEBBOX Version 1.10.7 (22.02.2024)

[**Update-Anleitung**](https://doc.davinci6.stueber.de/09.infoserver/update/) <br/>
[**Download**](https://davinci-webbox.stueber.de/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Sicherheitslücke in Kombination mit DAVINCI WEBBOX und DAVINCI MOBILE in DAVINCI-Server geschlossen. Bei Einsatz des DAVINCI INFOSERVERs bitte unbedingt den DAVINCI SERVER aktualisieren!

## DAVINCI WEBBOX Version 1.10.6 (18.10.2023)

[**Update-Anleitung**](https://doc.davinci6.stueber.de/09.infoserver/update/) <br/>
[**Download**](https://davinci-webbox.stueber.de/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Der Parameter `substitutionShowExtra` wurde korrigiert
* NEW: Die Bezeichnung des Klassenfehlgrunds wird am oberen Rand des Terminfensters hinter der Info "Klassen fehlt" eingeblendet. Ein Beispiel: "Klasse fehlt: Distanzunterricht"

## DAVINCI Version 6.5.86 (24.01.2024)

### Allgemein

* FIX: `Importieren > Exportieren > Export für Schulportal Hessen` 
* CHANGE: Abgleich mit MAGELLAN 11 wurde ermöglicht

### Vertretungsplan

* FIX: Vorziehoptionen vom gleichen Tag als direkte Vertretung