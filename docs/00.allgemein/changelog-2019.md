# Was ist neu


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

## DAVINCI Version 6.5.61

### STUNDENPLAN

* NEW: Auswahlfenster - Shortcut `Strg + F` für Auswahlfenster Fächer
* NEW: Blockelemente im Plan: über `Strg + linke Maustaste` auf das Blockelemnet klicken, können Sie die weiteren geblockten Elemente sichtbar machen, wenn Sie nun ein Element anklicken, wird dieses oben und damit auch als erstes in der Planansicht dargestellt
* NEW:  Stellt man einen Wochenbezug ohne Zuweisung einer vorab im Stammdatenfenster definierten Periode, sondern über die Zuweisung bestimmter Kalenderwoche her, wird nun in der Plananzeige neben der Ausgabe der Kalenderwochen auch der Zusatz "KW" ausgegeben.
![Zeitvorgaben in den Veranstaltungsdetails](/assets/images/liesmich/6.5.61.04.png)
![Anzeige im Stundenplan](/assets/images/liesmich/6.5.61.05.png)

* FIX: Hinzufügen eines 2. Raumes über das Zusatzfenster `Passende Räume` in der Liste der  Veranstaltungen in der Terminzeile
* FIX: Kernzeiten werden nicht mehr wie Sperrzeiten interpretiert
* FIX: `Plan-Eigenschaften > Planeinträge > Farben` Streifen mit Farbverlauf
* FIX: `Plan-Eigenschaften > Stundenplan` aktivierte Einstellung der Anzeige `Immer Uhrzeiten anzeigen` klappt wieder
* FIX: Stundenplan-Zeitkonto  Operator `A` - Berechnung klappt wieder korrekt für die Fächer, die in der Ansicht `Stammdaten > Fächer` in der Spalte „Zeitkonto“ für ein Fach einen Lehrer-Soll-Schlüssel mit dem Operator `A` als Zeitkonto zugewiesen bekommen haben.
* FIX: `Start > Automatik > Planungsstand` Springstundenzählung für Klassen und Lehrer
* FIX: `Start > Automatik` Automatische Verplanung berücksichtigt Wegzeiten, die über die Zuordnung verschiedener Gebäude zu den Räumen `Stammdaten > Gebäude` entstehen
* FIX: Summen für periodische Veranstaltungen, deren Periode unter `Start > Veranstaltung > Veranstaltung bearbeiten` definiert wurde korrigiert
* FIX: `Start > Automatik` Automatikroutine verbessert
* FIX: `Stammdaten > Ressourcen` Spalte Rücklaufzeit kann editiert werden
* FIX: `Stundenplan > Ansicht > Anordnung > Filter laden` Access Violation nach Aufruf von Filter laden behoben
* FIX: `Stammdaten > Lehrer` - Sortierung nach "Name" klappt  
* FIX:`Stundenplan > Start > Automatik` Kernzeiten im Klassenplan werden beachtet
* FIX: `Status` geeigneter Aufsichtslehrer optimiert, es werden mögliche Lehrer nur noch mit dem Status "ausgezeichnet" versehen, wenn diese vor/nach einer Pausenaufsicht Unterricht im Plan haben
* FIX: `Start > Automatik` Automatikvorgaben für Lehrer - max. Aufsichtsdauer je Woche
* FIX: Ansicht `Plan und Liste` und zwei weitere Pläne - Korrespondenz der Pläne sehr verbessert
* CHANGE: `Stundenplan > Veranstaltung > Neue Veranstaltung` Beim Anlegen einer neuen Veranstaltung in der Veranstaltungsliste ist die Dauer automatisch mit "1" vorbelegt (vormals "0")

### VERTRETUNGSPLAN

* NEW: Bereich `Änderungsliste` > In der Änderungsliste sind die Zellen "Datum" und "Tag" aktuell vertikal miteinander verbunden. Neuer Rechte-Maustaste Befehl in der Änderungsliste `Datumzellen zusammenfassen`. Wenn dies markiert ist, werden die Datumszellen zusammengefasst, sonst nicht.
  
![Änderungsliste `Datumzellen zusammenfassen` aktiviert](/assets/images/liesmich/6.5.61.02.png)

![Änderungsliste `Datumzellen zusammenfassen` nicht aktiviert](/assets/images/liesmich/6.5.61.03.png)
  
* FIX: frei gewordener Raum (z.B. durch Klassenfehlzeit) wird als freier Raum zur Vertretungserstellung angeboten
* FIX: Lehrer übernimmt Vertretung und wird dann selbst krank, Termine tauchen wieder zur Vertretung in der Liste der offenen Vertretungen auf
* FIX: Fehlzeit eines Lehrers wurde bereits vertreten, nun wird eine Raumfehlzeit erzeugt, die ursprüngliche Lehrerfehlzeit wird dann wieder mit dem Status "Offen" in der Liste der offenen Vertretungen angezeigt
* FIX:  indirekte Vertretungen mit zuvor erfasster Raumänderung - "Lehrer freistellen" wird angeboten
* FIX: `Extras > Plandatei aufräumen` beseitigt Restfragmente in der Ansicht `Vertretungsplan > Vertretungen` wenn man Perioden nach Eintrag von Fehlzeiten im Stammdatenfenster geändert hat, werden in der Liste der offenen Vertretungen Elemente angezeigt, die es so aber nicht mehr im Planfenster gibt
* FIX: Es ist wieder möglich, aus der Liste der direkte Vertreter Lehrer einzusetzen, wenn für diese eine Sperrung (Kategorie 2-4) im Stundenplan erfasst wurde.
* FIX: Fehlt ein Lehrer über einen längeren Zeitraum, werden im Vertretungserstellen-Fenster wieder Folgetermine angezeigt, die analog vertreten werden sollen:
![Folgende Fehltermine analog vertreten](/assets/images/liesmich/6.5.61.06.png)

* FIX: Anrechenstunden, die man einem Lehrer über den Bereich "Anrechnungen" neu hinzugefügt hat (über Befehl `F2` oder grünes Plus in der Registerkarte "Start") werden nun auch in den Bereich "Vertretungen" bei den indirekten/direkten Vertretern in die Spalten +/-AStd/M und +/-AStd/J übergeben
* FIX: Unter `Start > Planansicht` aktivierte Einstellung `Positionskonflikte anzeigen` gibt wieder korrekt farbliche Markierungen im Planfenster aus

### KURSPLAN

* FIX: `Kursplan > Fachwahlen` Alle Fachwahlen markieren
* FIX: fälschlichwerweise angezeigte Konflikte werden über `Extras > Plandatei aufräumen` gelöscht
* FIX: falsche Kurszuweisung nach Kurswechsel werden über `Extras > Plandatei aufräumen` gelöscht
* FIX: `Kursplan > Fachwahlen` alle Fachwahlen markieren wieder möglich
* FIX: `Kursplan > Fachwahlen` Löschen einer Fachwahlzeile wieder möglich

### LOOK

* FIX: ein über DAVINCI LOOK gebuchte Ressourcen wird in der Ansicht der Ressource gezeigt
* FIX: Lehrersuche über Suchfeld korrigiert (Wechsel von Lehrer zu Raum und dann wieder zu Lehrerplan führte zu Wechsel in falschen Lehrerplan)
  
### DRUCK

* NEW: Druckformat "Kurslisten" > Erweiterung der Ausgabe um Schülergeschlecht, Summen werden nun stets in der Überschrift angegeben
* NEW: Druckformat "Kurslisten" > Erweiterung der Ausgabe um Schülergeschlecht
 ![Druckformat "Kurslisten"](/assets/images/liesmich/6.5.61.01.png)

* FIX: Druckformat "Kurslisten" - Designänderungen werden übernommen
* FIX: Ausdruck von Vertetungen bei unterschiedlichen Zeitrahmen korrigiert
* FIX: Ausdruck der Fach-/ Lehrerlegende gibt bei Teamteaching auch den zweiten Lehrer aus
* FIX: Ausdruck von Vertretungsplänen: In Spalte "Art" wird nun aus dem Schlüsselverzeichnis "Vertretungsentfallgründe" das Feld "Bezeichnung" (Langname) und nicht mehr das Feld "Kürzel" in den Druck übergeben
  
### HTML Export

* FIX: Exportformat "Lehrer-Änderungsabrechnung" - Änderungen werden wieder korrekt übergeben

### Sonstiges

* FIX: Übersicht "Ausfallstatistik" > Bitte einmalig über `Extras > Plandatei aufräumen` ausführen, damit werden fehlerhafte Änderungselemente gelöscht.
* FIX: LANIS Export Zeichensatz auf UTF 8 geändert

### Webbox

* FIX: Vertretungen für eine gleichzeitige Raum- und Lehrerfehlzeit werden in allen betroffenen Plänen angezeigt


## DAVINCI Version 6.5.60

Veröffentlichung: 12.09.2019
Dateiformat: 6.0.171

### ALLGEMEIN

* NEW: 13_NRW_Lehrer-Soll-Schluessel.keys

## DAVINCI Version 6.5.59

Veröffentlichung: 04.09.2019
Dateiformat: 6.0.171

### ALLGEMEIN

* NEW: Datenabgleich mit MAGELLAN 7 möglich
* CHANGE: 12_SHL_Lehrer-Soll-Schluessel.keys
* CHANGE: 23_SHL_Unterrichtsarten.keys
* CHANGE: 25_SHL_Veranstaltungskategorien.keys
* CHANGE: 25_SHL_Veranstaltungskategorien.keys

### LOOK

* FIX: Die in DAVINCI LOOK bzw. im VERTRETUNGSPLAN gebuchten Ressourcen werden im entsprechenden Ressourcenplan (über Auswahlfenster "verfügbare Ressourcen" zu öffnen) wieder angezeigt

## DAVINCI Version 6.5.58

Veröffentlichung: 30.07.2019
Dateiformat: 6.0.171

* NEW: Neue Nachrichtenfunktion: Die DAVINCI-Willkommensseite wurde neu gestaltet und enthält jetzt zu den wichtigsten Aufrufen (Dokumentation, Newsletter, Ticketsystem usw.) einen Nachrichtenbereich, über den wir Sie auf dem Laufenden halten werden. Sie erhalten diesen Überblick beim Aufruf von DAVINCI und DAVINCI LOOK.

### DRUCK

* FIX: Kopf- und Fußzeilen in Klassen-, Lehrer- und Vertretungsplänen werden wieder korrekt an den Druckertreiber übergeben

## DAVINCI Version 6.5.57

Veröffentlichung: 20.06.2019
Dateiformat: 6.0.171

### STUNDENPLAN

* FIX: Problem beim Öffnen einiger Dateien nach Update auf 6.5.56 behoben

## DAVINCI Version 6.5.56

Veröffentlichung: 18.06.2019
Dateiformat: 6.0.171

### SERVER

* CHANGE: Ein Benutzer, der einem Mandanten zugeordnet ist und als Admin gekennzeichnet ist hat folgende Rechte:

1. Alle Benutzer seines Mandanten bearbeiten und löschen. Allerdings kann nicht die Mandantenzugehörigkeit geändert werden.
2. Alle Benutzer seines Mandanten exportieren.
3. Neue Benutzer importieren, die dann alle automatisch seinem Mandanten zugeordnet werden

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
