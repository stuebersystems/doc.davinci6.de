# Was ist neu

Dieses Kapitel gibt ihnen einen Überblick über aktuelle Änderungen in DAVINCI 6 und in der DAVINCI WEBBOX.

* Den Änderungsverlauf aus den vergangenen Jahren finden Sie hier: [2019](changelog-2019.md), [2018](changelog-2018.md), [2017](changelog-2017.md),  [2016](changelog-2016.md), [2015](changelog-2015.md), [2014 und früher](changelog-archive.md).

* Was wir für die nächste Ausgabe planen, sehen Sie im Kapitel [Voraussichtliche Änderungen](changelog-next.md).

## LEGENDE

Abkürzung  |  Bedeutung
---------- | ----------
FIX |  Korrektur bestehender Funktionalität
NEW |  Neue Funktionalität  
CHANGE|  Änderung des Ablaufs, Verarbeitung oder Bedienung

---

## Aktueller Hinweis

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

## DAVINCI MOBILE APP

* NEW: Testfunktion für die Serververbindung
* NEW: Im Detailfenster einer Veranstaltung (Klick aufs Terminfeld) werden für Vertretungen auch die Vertretungsinformation und die Vertretungsmitteilung gezeigt (beide Informationen werden in DAVINCI Vertretungsplan in der Vertretungsliste in den gleichnamigen Spalten erfasst)
* NEW: Die Bezeichnung des Klassenfehlgrunds wird beim Klick auf ein Terminfeld im Detailfenster zusätzlich zur Information "Klasse fehlt" gezeigt. 

## DAVINCI WEBBOX Version 1.10.5 

[**UPDATE-ANLEITUNG**](https://doc.davinci6.stueber.de/09.infoserver/infoserver-und-webbox-aktualisieren/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Darstellung von Fehlzeiten in der Vertretungsansicht bei vorherigem Feiertag
* FIX: Anzeige von Wochentagen in der Vertretungsliste (davinci-substitutions.html) korrigiert
* NEW: Neuer Parameter (+ Wert) "substSort=key". Dieser Parameter arbeitet gemeinsam mit dem Parameter "substKey".
  Beispiele:

1. Gruppiert und sortiert nach Lehrer: .../davinci-substitutions.html?substKey=teacher&substSort=key
2. Gruppiert und sortiert nach KLasse: .../davinci-substitutions.html?substKey=class&substSort=key
* FIX: Anzeige von Kalendereignissen und damit verbundenen Unterrichtsstunden
* FIX: Anzahl der Klassen in der Anzeige "Alle Klassen" erhöht

## DAVINCI Version 6.5.71 (07.06.2021)

### Allgemein

* FIX: Korrekturen zum Abgleich DAVINCI Vertretungsplan mit dem ENBREA Klassenbuch bezüglich der Darstellung der Vertretungsplaninformationen

## DAVINCI Version 6.5.70 (20.05.2021)

### Allgemein

* NEW: Abgleich DAVINCI - MAGELLAN 8

### VERTRETUNGSPLAN

* FIX: `Vertretungsplan > Anrechnen` Anrechenstunden können manuell hinzugefügt werden mit Auswahl des Lehrers
* FIX: `Vertretungsplan > Vertretungen` fehlende Vorziehoptionen werden angezeigt

### SERVER

* FIX: Doppelte Ausgabe von Mitteilungen für die Webbox korrigiert

### LOOK

* FIX: DAVINCI LOOK liest die Pathsdatei daVinciLook.paths statt der daVinci.paths 


## DAVINCI Version 6.5.69 (25.03.2021)

### STUNDENPLAN

* FIX: mehrtägige Ereignisse werden wieder korrekt im Zusatzkalender gespeichert/angezeigt
* FIX: Ereignisse (von-bis Zeit) werden wieder korrekt im Zusatzkalender gespeichert/angezeigt
* NEW: Kalenderdateien Ferien 2021/2022
* FIX: Aufsichtsplan: Lehrer, die bereits einem Aufsichtsbereich zugewiesen sind, stehen in anderen Bereichen zur selben Zeit wieder zur Auswahl

### VERTRETUNGSPLAN

* FIX: V-Lehrer für Aufsichten - eine Lehrkraft kann nun wieder mehrere Bereiche vertreten, d.h. sobald eine Lehrkraft einem Aufsichtsbereich zugewiesen ist, steht diese wieder als möglicher Vertreter zur Auswahl (mit der "Bemerkung" - bereits Aufsicht zu dieser Zeit).
* FIX: bei gleichzeitiger Lehrer- und Klassenfehlzeit in einer Blockung, lassen sich die verbliebenen Teile der Blockung wieder vertreten
* FIX: Befristungen von Veranstaltungen im Stundenplanbereich löschen im Vertretungsplanbereich nur die Veranstaltungen/Vertretungen, die von der Befristung betroffen sind

### KURSPLAN

* FIX: `Kursplan > Fachwahlen` Fachschwerpunkt auswählbar
  
### DRUCK

* FIX: `Design > Liste> Klassenfehlzeitermine anzeigen`reguläre Stunden ohne V-Planänderungen werden nicht mehr ausgegeben
* FIX: `Kursliste` bei Kursduplikaten mit zwei unterschiedlichen Lehrern werden beide Kurse zum Druck angeboten
  
### HTML Export

* FIX: HTML-Main-Vorlagen: Buttons werden wieder korrekt dargestellt

### Analytics

* FIX: Ausfallstatistik - Ausgabe der Werte `Zeitraum > Verplant` bei der Auswahl mehrerer Tage

## DAVINCI Version 6.5.68 (29.10.2020)

### STUNDENPLAN

* CHANGE: beim Anlegen einer neuen Veranstatltung ist im Fenster `Veranstaltung bearbeiten` der Haken für **Dauer unabhängig vom Block** standardmäßig nicht gesetzt

### VERTRETUNGSPLAN

* FIX: `Vertretungen > Vorziehen`fehlende Vorziehoptionen korrigiert

### KURSPLAN

* FIX: `Kursplan > Fachwahl` Schüler verschwinden im Fenster Schüler
* FIX: `Kursplan > Fachwahlen` Aktualisierungsproblem beim Wechseln in einen anderen Kurs
* FIX_ `Kursplan > Fachwahl > Fachwahl erzeugen` Übergabe der Sollstundenzahl
* FIX: `Kursplan > Kurse` Löschen eines manuell angelegten Kurses 

