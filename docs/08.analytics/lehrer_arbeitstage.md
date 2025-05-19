# Übersicht "Lehrer Arbeitstage"

**Filterangaben:**

* Von-Bis: Auswahl des auszuwertenden Zeitraumes
* Fehlgrund: Auswahl des Fehlgrundes für die Anzeige in der Spalte Fehlzeit/Tage; Fehlzeit/Stunden (greift zurück auf das Schlüsselverzeichnis "Lehrerfehlgründe")
* Lehrerart: Auswahl der Lehrerart (greift zurück auf das Schlüsselverzeichnis "Lehrerarten") unterscheidet Lehrer von anderen für die Ausgabe der Summen in den Spalten
* Team: filtert nach Teamzugehörigkeit (greift zurück auf die Eintragungen in den Stammdaten)

!!! info "Hinweis"

     Für die Auswertung der Altersangaben ist die Eintragung des Geburtsdatums in `Stammdaten|Lehrer` notwendig.

## Ansicht "Übersicht"

![Ansicht Übersicht](/assets/images/Lehrerarbeitstage1.png)

## Bereich Merkmale

Spalte | Erläuterungen
--------|-------------------------------------------
Merkmal| fest definiertes Merkmal zur Aufsummierung 
Anzahl|Anzahl der auf das Merkmal bezogenen Lehrer im ausgewählten Zeitraum
Arbeitstage|Anzahl der auf das Merkmal bezogenen Arbeitstage der Lehrer im ausgewählten Zeitraum

## Bereich Fehltage

Spalte | Erläuterungen
--------|-------------------------------------------
Tage |Gesamtfehltage der Lehrer im ausgewählten Zeitraum unabhängig von der Dauer der Fehlzeit
Quote|
Lehrer|Anzahl der fehlenden Lehrer im ausgewählten Zeitraum unabhängig von der Dauer der Fehlzeit

## Bereich 1-3 Fehltage

Spalte | Erläuterungen
--------|-------------------------------------------
Tage |Gesamtfehltage der Lehrer im ausgewählten Zeitraum, Dauer der Fehlzeit 1-3 Fehltage
Quote|
Lehrer|Anzahl der fehlenden Lehrer im ausgewählten Zeitraum, Dauer der Fehlzeit 1-3 Fehltage

## Ansicht "Lehrer"

[![Ansicht Lehrer][1]][1] 

### Bereich Lehrer

Spalte | Erläuterungen
--------|-------------------------------------------
Kürzel | Kürzel Lehrer laut `Stammdaten>Lehrer`
Titel |laut `Stammdaten>Lehrer`
Nachname|Nachname Lehrer laut `Stammdaten>Lehrer`
Vorname|Vorname laut `Stammdaten>Lehrer`
Mittelname|Mittelname Lehrer laut `Stammdaten>Lehrer`
Geschlecht|Geschlecht Lehrer laut `Stammdaten>Lehrer`
Team|Team Lehrer laut `Stammdaten>Lehrer`

### Bereich geplant

Spalte | Erläuterungen
--------|-------------------------------------------
Tage|geplante Unterrichtstage im Auswahlzeitraum
Stunden |geplante Unterrichtsstunden im Auswahlzeitraum

### Bereich Fehlzeit

Spalte | Erläuterungen
--------|-------------------------------------------
Tage| Fehlzeittage auf Grund des ausgewählten Fehlgrundes
Stunden |Fehlzeitstunden auf Grund des ausgewählten Fehlgrundes

[1]:/assets/images/analytics/Lehrerarbeitstage.png