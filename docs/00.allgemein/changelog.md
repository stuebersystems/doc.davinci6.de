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

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/substitution-plan/veroeffentlichung/veroeffentlichung/)

## DAVINCI Version 6.5.63 (18.02.2020)

### VERTRETUNGSPLAN

* FIX: Liste der offenen Vertretungen, wird ein Eintrag gewählt, passt sich das Planfenster rechts entsprechend an. Wechselt man nun auf einen anderen Eintrag in der Liste der offenen Vertretungen mit gleicher Positionierung, passt sich das Planfenster rechts nun auch wieder richtig an.

### Sonstiges

* FIX: Kalenderdateinen für Ferientermine 2020/2021

### Webbox

* FIX: vereinzelt fehlten Termine einer Veranstaltung in der Lehrer und Klassenansicht, dies wurde korrigiert


## DAVINCI Version 6.5.62 (23.01.2020)

### STUNDENPLAN

* NEW: `Stammdaten > Lehrer` Lehrbefähigung in Spalte Fächer kann wieder eingegeben werden
 
### DRUCK

* FIX: Speichern der Ausrichtung Querformat wieder möglich

!!! danger "Achtung"
    Ehemals für das Querfomrat angelegte Druckformate müssen Sie bitte noch einmal neu als Querformat speichern. Bitte gehen Sie in die Druckvorschau `Format > Seite einrichten > Seite` und stellen Sie hier das gewünschte Format ein.
  

## DAVINCI Version 6.5.61 (10.01.2020)

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

* NEW:  Bereich `Änderungsliste` > In der Änderungsliste sind die Zellen "Datum" und "Tag" aktuell vertikal miteinander verbunden. Neuer Rechte-Maustaste Befehl in der Änderungsliste `Datumzellen zusammenfassen`. Wenn dies markiert ist, werden die Datumszellen zusammengefasst, sonst nicht.
  
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
* FIX: erzeugte Vertretung einer Raumfehlzeit wird durch Erfassen einer Lehrerfehlzeit zur selben Zeit nicht mehr zurückgesetzt

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
