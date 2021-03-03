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

