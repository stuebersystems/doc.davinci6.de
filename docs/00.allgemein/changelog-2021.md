# Änderungen 2021

## LEGENDE

Abkürzung  |  Bedeutung
---------- | ----------
FIX |  Korrektur bestehender Funktionalität
NEW |  Neue Funktionalität  
CHANGE|  Änderung des Ablaufs, Verarbeitung oder Bedienung

## DaVinci Version 6.5.75 (22.11.2021)

### Allgemein

* FIX: Abgleich DaVinci - Enbrea Klassenbuch (Alpha)

## DaVinci Version 6.5.74 (18.10.2021)

### Allgemein

* FIX: Kalenderdatei 2021/2022 für SHL korrigiert
* FIX: SDUI Upload korrigiert

## DaVinci Mobile App

* NEW: Testfunktion für die Serververbindung
* NEW: Im Detailfenster einer Veranstaltung (Klick aufs Terminfeld) werden für Vertretungen auch die Vertretungsinformation und die Vertretungsmitteilung gezeigt (beide Informationen werden in DaVinci Vertretungsplan in der Vertretungsliste in den gleichnamigen Spalten erfasst)
* NEW: Die Bezeichnung des Klassenfehlgrunds wird beim Klick auf ein Terminfeld im Detailfenster zusätzlich zur Information "Klasse fehlt" gezeigt. 

## DaVinci WebBox Version 1.10.5 

[**UPDATE-ANLEITUNG**](https://doc.davinci6.stueber.de/09.infoserver/update/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DaVinci Look und der DaVinci WebBox: [Welche Vertretungsinformationen werden für Look oder die WebBox publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Darstellung von Fehlzeiten in der Vertretungsansicht bei vorherigem Feiertag
* FIX: Anzeige von Wochentagen in der Vertretungsliste (davinci-substitutions.html) korrigiert
* NEW: Neuer Parameter (+ Wert) "substSort=key". Dieser Parameter arbeitet gemeinsam mit dem Parameter "substKey".
  **Beispiele:**
Gruppiert und sortiert nach Lehrer: .../davinci-substitutions.html?substKey=teacher&substSort=key
Gruppiert und sortiert nach KLasse: .../davinci-substitutions.html?substKey=class&substSort=key
* FIX: Anzeige von Kalendereignissen und damit verbundenen Unterrichtsstunden
* FIX: Anzahl der Klassen in der Anzeige "Alle Klassen" erhöht

## DaVinci Version 6.5.73 (07.10.2021)

### Stundenplan

* FIX: `Stundenplan > Jahresverteilung`geplant Summen 

### Vertretungsplan

* FIX: `Übersichten > Ausfallstatistik` Export 
* FIX: Verlängerung einer Lehrerfehlzeit hat bei vorgezogenen Stunden zu Leereinträgen in der Änderungsliste geführt, dieses Problem ist gelöst. Achtung, bestehende Leereinträge werden durch das Update nicht bereinigt, müssen also manuell aus der Änderungsliste entfernt werden.

### Kursplan

* FIX: automatisches Anlegen von Kursen bei mehreren Klassen einer Jahrgangsstufe

## DaVinci Version 6.5.72 (24.06.2021)

### Server

* FIX: Zusatzunterrichte wurden als offene Vertretungen kategorisiert, als Ergebnis konnte es zur falschen bzw. unvollständigen JSON-Ausgabe (WebBox, App) führen 

## DaVinci Version 6.5.71 (07.06.2021)

### Allgemein

* FIX: Korrekturen zum Abgleich DaVinci Vertretungsplan mit dem Enbrea Klassenbuch bezüglich der Darstellung der Vertretungsplaninformationen

## DaVinci Version 6.5.70 (20.05.2021)

### Allgemein

* NEW: Abgleich DaVinci - Magellan 8

### Vertretungsplan

* FIX: `Vertretungsplan > Anrechnen` Anrechenstunden können manuell hinzugefügt werden mit Auswahl des Lehrers
* FIX: `Vertretungsplan > Vertretungen` fehlende Vorziehoptionen werden angezeigt

### Server

* FIX: Doppelte Ausgabe von Mitteilungen für die WebBox korrigiert

### Look

* FIX: DaVinci Look liest die Pathsdatei daVinciLook.paths statt der daVinci.paths 


## DaVinci Version 6.5.69 (25.03.2021)

### Stundenplan

* FIX: mehrtägige Ereignisse werden wieder korrekt im Zusatzkalender gespeichert/angezeigt
* FIX: Ereignisse (von-bis Zeit) werden wieder korrekt im Zusatzkalender gespeichert/angezeigt
* NEW: Kalenderdateien Ferien 2021/2022
* FIX: Aufsichtsplan: Lehrer, die bereits einem Aufsichtsbereich zugewiesen sind, stehen in anderen Bereichen zur selben Zeit wieder zur Auswahl

### Vertretungsplan

* FIX: V-Lehrer für Aufsichten - eine Lehrkraft kann nun wieder mehrere Bereiche vertreten, d.h. sobald eine Lehrkraft einem Aufsichtsbereich zugewiesen ist, steht diese wieder als möglicher Vertreter zur Auswahl (mit der "Bemerkung" - bereits Aufsicht zu dieser Zeit).
* FIX: bei gleichzeitiger Lehrer- und Klassenfehlzeit in einer Blockung, lassen sich die verbliebenen Teile der Blockung wieder vertreten
* FIX: Befristungen von Veranstaltungen im Stundenplanbereich löschen im Vertretungsplanbereich nur die Veranstaltungen/Vertretungen, die von der Befristung betroffen sind

### Kursplan

* FIX: `Kursplan > Fachwahlen` Fachschwerpunkt auswählbar
  
### DRUCK

* FIX: `Design > Liste> Klassenfehlzeitermine anzeigen`reguläre Stunden ohne V-Planänderungen werden nicht mehr ausgegeben
* FIX: `Kursliste` bei Kursduplikaten mit zwei unterschiedlichen Lehrern werden beide Kurse zum Druck angeboten
  
### HTML Export

* FIX: HTML-Main-Vorlagen: Buttons werden wieder korrekt dargestellt

### Analytics

* FIX: Ausfallstatistik - Ausgabe der Werte `Zeitraum > Verplant` bei der Auswahl mehrerer Tage

## DaVinci Version 6.5.68 (29.10.2020)

### Stundenplan

* CHANGE: beim Anlegen einer neuen Veranstatltung ist im Fenster `Veranstaltung bearbeiten` der Haken für **Dauer unabhängig vom Block** standardmäßig nicht gesetzt

### Vertretungsplan

* FIX: `Vertretungen > Vorziehen`fehlende Vorziehoptionen korrigiert

### Kursplan

* FIX: `Kursplan > Fachwahl` Schüler verschwinden im Fenster Schüler
* FIX: `Kursplan > Fachwahlen` Aktualisierungsproblem beim Wechseln in einen anderen Kurs
* FIX_ `Kursplan > Fachwahl > Fachwahl erzeugen` Übergabe der Sollstundenzahl
* FIX: `Kursplan > Kurse` Löschen eines manuell angelegten Kurses 

