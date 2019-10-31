# Voraussichtliche Änderungen

!!! info "Hinweis"

    Sie erhalten hier einen Überblick über die voraussichtlichen Änderungen und Korrekturen für das nächste Serviceupdate.

## LEGENDE

| Abkürzung | Bedeutung |
| --- | --- |
| FIX | Korrektur bestehender Funktionalität |
| NEW | Neue Funktionalität |
| CHANGE | Änderung des Ablaufs, Verarbeitung oder Bedienung |

## DAVINCI WEBBOX Version 1.10.5 \[unveröffentlicht\]

[**UPDATE-ANLEITUNG**](https://doc.davinci6.stueber.de/09.infoserver/update-internet-publication/infoserver-und-webbox-aktualisieren/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

## DAVINCI Version 6.5.61

### SERVER

### INFOSERVER

### STUNDENPLAN

* NEW: Auswahlfenster - Shortcut `Strg + F`für Auswahlfenster Fächer
* NEW: Blockelemente im Plan: über STRG + linke Maustaste auf das Blockelemnet klicken, können Sie die weiteren geblockten ELmente sichtbar machen, wenn Sie nun ein elment anklicken, wird dieses oben und damit auch als erstes in der Planansicht dargestellt
* NEW:  Stellt man einen Wochenbezug ohne Zuweisung einer vorab im Stammdatenfenster definierten Periode, sondern über die Zuweisung bestimmter Kalenderwoche her, wird nun in der Plananzeige neben der Ausgabe der Kalenderwochen auch der Zusatz "KW" ausgegeben.
![Zeitvorgaben in den Veranstaltungsdetails](/assets/images/liesmich/6.5.61.04.png)
![Anzeige im Stundenplan](/assets/images/liesmich/6.5.61.05.png)

* FIX: Hinzufügen einers 2. Raumes über das Zusatzfenster `Passende Räume` in der Liste der  Veransatltungen in der Terminzeile
* FIX: Kernzeiten werden nicht mehr wie Sperrzeiten interpretiert
* FIX: `Plan-Eigenschaften > Planeinträge > Farben` Streifen mit Farbverlauf
* FIX: `Plan-Eigenschaften > Stundenplan` aktivierte Einstellung der Anzeige `Immer Uhrzeiten anzeigen` klappt wieder
* FIX: Stundenplan-Zeitkonto  Operator `A` - Berechnung klappt wieder korrekt für die Fächer, die in der Ansicht `Stammdaten > Fächer` in der Spalte „Zeitkonto“ für ein Fach einen Lehrer-Soll-Schlüssel mit dem Operator `A` als Zeitkonto zugewiesen bekommen haben.
* FIX: `Start > Automatik > Planungsstand` Springstundenzählung für Klassen und Lehrer*
* FIX: Summen für periodische Veranstatlungen, deren Periode unter `Start > Veranstaltung > Veranstaltung bearbeiten` definiert wurde korrigiert
* FIX: `Start > Automatik` Automatikroutine verbessert
* FIX: `Stammdaten > Ressourcen` Spalte Rücklaufzeit kann editiert werden
* FIX: `Stundenplan > Ansicht > Anordnung > Filter laden` Access Violation nach Aufruf von Filter laden behoben
* FIX: `Stammdaten > Lehrer` - Sortierung nach "Name" klappt  
* FIX:`Stundenplan > Start > Automatik` Kernzeiten im Klassenplan werden beachtet
* FIX: `Status` geeigneter Aufsichtslehrer optimiert, es werden mögliche Lehrer nur noch mit dem Status "ausgezeichnet" versehen, wenn diese vor/nach einer Pausenaufsicht Unterricht im Plan haben
* FIX: `Start > Automatik` Automatikvorgaben für Lehrer - max. Aufsichtsdauer je Woche
* FIX: Ansicht `Plan und Liste` und zwei weitere Pläne - Korrespondenz der Pläne sehr verbessert

### VERTRETUNGSPLAN

* NEW: Bereich `Änderungsliste` > In der Änderungsliste sind die Zellen "Datum" und "Tag" aktuell vertikal miteinander verbunden. Neuer Rechte-Maustaste Befehl in der Änderungsliste `Datumzellen zusammenfassen`. Wenn dies markiert ist, werden die Datumszellen zusammengefasst, sonst nicht.
  
![Änderungsliste `Datumzellen zusammenfassen` aktiviert](/assets/images/liesmich/6.5.61.02.png)

![Änderungsliste `Datumzellen zusammenfassen` nicht aktiviert](/assets/images/liesmich/6.5.61.03.png)
  
* FIX: frei gewordener Raum (z.B. durch Klassenfehlzeit) wird als freier Raum zur Vertretungserstellung angeboten
* FIX: Lehrer übernimmt Vertretung und wird dann selbst krank, Termine tauchen wieder zur Vertretung in der Liste der offenen Vertretungen auf
* FIX: Fehlzeit Lehrers wurde bereits vertreten, dann wird eine Raumfehlzeit erzeugt, die ursprüngliche Lehrerfehlzeit wird nun wieder mit dem Status "Offen" in der Liste der offenen Vertretungen angezeigt
* FIX:  indirekte Vertretungen mit zuvor erfasster Raumänderung - "Lehrer freistellen" wird angeboten
* FIX: `Èxtras > Plandatei aufräumen` bwawitigt Restfragmente in der Ansicht `Vertretungsplan > Vertretungen` wenn man Perioden nach Eintrag von Fehlzeiten geändert im Stammdatenfenster geändert hat, werden in der Liste der offenen Vertretungen Elemente angezeigt, die es so aber nicht mehr im Planfenster gibt

### KURSPLAN

* FIX: `Kursplan > Fachwahlen` Alle Fachwahlen markieren
* FIX: fälschlichwerweise angezeigt Konflikt werden über `Extras > Plandatei aufräumen` gelöscht
* FIX: `Kursplan > Fachwahlen` alle Fachwahlen markieren wieder möglich
* FIX: `Kursplan > Fachwahlen` Löschen einer Fachwahlzeile

### LOOK

* FIX: ein über DAVINCI LOOK gebuchte Ressourcen wird in der Ansicht der Ressource gezeigt
* FIX: Lehrersuche über Suchfeld korrigiert (Wechsel von Lehrer zu Raum und dann wieder zu Lehrerplan führte zu Wechsel in falschen Lehrerplan)
  
### DRUCK

* NEW: Druckformat "Kurslisten" > Erweiterung der Ausgabe um Schülergeschlecht, Summen werden nun stets in der Überschrift angegeben
* NEW: Druckformat "Kurslisten" > Erweiterung der Ausgabe um Schülergeschlecht
 ![Druckformat "Kurslisten"](/assets/images/liesmich/6.5.61.01.png)

* FIX: Ausdruck > Kursliste - Designänderungen werden  übernommen
* FIX: Ausdruck von Vertetungen bei unterschiedlichen Zeitrahmen korrigiert
  
### HTML Export

### Sonstiges

* FIX: Übersicht "Ausfallstatistik" > Bitte einmalig über `Extras > Plandatei aufräumen` ausführen, damit werden fehlerhafte Änderungselemente gelöscht.
  