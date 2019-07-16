# Was ist neu

Dieses Kapitel gibt ihnen einen Überblick über aktuelle Änderungen in DAVINCI 6 und in der DAVINCI WEBBOX.

* Den Änderungsverlauf aus den vergangenen Jahren finden Sie hier: [2018](changelog-2018.md), [2017](changelog-2017.md),  [2016](changelog-2016.md), [2015](changelog-2015.md), [2014 und früher](changelog-archive.md).

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

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/substitution-plan/veroeffentlichung/veroeffentlichung/)

## DAVINCI Version 6.5.57

Veröffentlichung: 20.06.2019
Dateiformat: 6.0.171

### STUNDENPLAN

* FIX: Problem beim Öffnen einiger Dateien nach Update auf 6.5.56 behoben

## DAVINCI Version 6.5.56

Veröffentlichung: 18.06.2019
Dateiformat: 6.0.171

### SERVER

CHANGE: Ein Benutzer, der einem Mandanten zugeordnet ist und als Admin gekennzeichnet ist hat folgende Rechte:

1. Alle Benutzer seines Mandanten bearbeiten und löschen. Allerdings kann nicht die Mandantenzugehörigkeit geändert werden.
2. Alle Benutzer seines Mandanten exportieren.
3. Neue Benutzer importieren, die dann alle automatisch seinem Mandanten zugeordnet werden

### INFOSERVER

### STUNDENPLAN

* FIX: Kalenderdatei für Sachsen für das SJ 2019/2020 (SAC_Schulferien_2019-2020.ical)

### VERTRETUNGSPLAN

* FIX: `Vertretungen > Fehlzeiten` Lehrerfehlzeit wird über eine geplante Vertretung des fehlenden Lehrers verlängert, Vertretung wird nicht zurückgesetzt
* FIX: `Vertretungen > Vertretungen` Vertreten von Fehlstellen durch Vorziehen wieder möglich
* FIX: `Vertretungen > Vertretungen` Lehrerfehlzeit nach Raumänderung - Raumänderung wird nur rückgängig gemacht, wenn beim Eintrag der Lehrerfehlzeit der Haken bei "Diese Änderungen zurücksetzen gesetzt" wurde
* FIX: ``Vertretungen > Fehlzeiten` Fehlzeit  bis zum letzten Tag des Planungszeitraumes kann wieder eingetragen werden
* FIX: `Vertretungen > Vertretungen` setzen des Fokus bei der Planauswahl und in der Liste der offenen Vertretungen korrigiert
* FIX: `Vertretungen > Vertretungen` durch Vertretungen verplanter Raum wird nicht mehr als frei dargestellt

### KURSPLAN

* FIX: `Kursplan > Blöcke` und `Kursplan > Kurse` farbige Markierung der Schüler für markierte Alterntativkurse wieder vorhanden
* FIX: `Kursplan > Schüler > Passende Kurse` Zuweisung von Kursen funktioniert wieder
* FIX: `Kursplan > Schüler` Löschen eines Kurse beim Schüler, löscht den Schüler auch aus Duplikaten des Kurses
* FIX: `Kursplan > Kurse > neue Veranstaltung` Löschen eines manuell angelegten Kurses wieder möglich
* FIX: `Kursplan > Schüler > Passende Kurse` bei der Zuweisung zu einem manuell angelegten Kurs wird die Kursnummer korrekt angezeigt

### LOOK

* FIX:  fehlende Anzeige von Zusatzunterricht im lokalen Betrieb kann über `Extras > Plandatei aufräumen` in DAVINCI angezeigt werden

### Sonstiges

* FIX: LANIS Export - ``Weiter``-Button wieder aktiv
![``Plan > Importieren/Eportieren`` Assistent](/assets/images/5.5.56_Bild1.png)

## DAVINCI Version 6.5.55

Veröffentlichung: 27.02.2019
Dateiformat: 6.0.171

### Server

* FIX: Problem beim Anzeigen von Zusatzunterricht mit Fehlzeiten für WEBBOX und App für Schüler und Klassen behoben
* FIX: Problem beim Anzeigen von ganztägigen Mitteilungen behoben

### INFOSERVER

* FIX: Problem bei aktivierter Komprimierung und 64-Bit DAVINCIIS.dll behoben
* NEW: Optimierungen zur Geschwindigkeitessteigerung

### STUNDENPLAN

* CHANGE: Mitteilungsfenster überarbeitet: Anordnung, zusätzliche Prüfung bei der Eingabe der Zeiten

## DAVINCI Version 6.5.53 und 6.5.54

Veröffentlichung: 20.02.2019
Dateiformat: 6.0.171

### KALENDER

* NEW: Neue Kalender für 2019/2020 verfügbar.

### Sonstiges

* FIX: Lanis Export UTF 8 Format
