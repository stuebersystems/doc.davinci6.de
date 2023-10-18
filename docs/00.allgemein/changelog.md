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
## DAVINCI WEBBOX Version 1.10.6 (unveröffentlicht)

[**Update-Anleitung**](https://doc.davinci6.stueber.de/09.infoserver/update/) <br/>
[**Download**](https://davinci-webbox.stueber.de/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Der Parameter `substitutionShowExtra` wurde korrigiert
* NEW: Die Bezeichnung des Klassenfehlgrunds wird am oberen Rand des Terminfensters hinter der Info "Klassen fehlt" eingeblendet. Ein Beispiel: "Klasse fehlt: Distanzunterricht"

## DAVINCI Version 6.5.86 (unveröffentlicht)

### Allgemein

## DAVINCI Version 6.5.85 (16.10.2023)

### Allgemein

* FIX: `Importieren > Exportieren > Export für Schulportal Hessen` Export Informationen bei Freistellungen von Lehrkräften

### Vertretungsplan

* CHANGE: Freistellen von Lehrkräften ganztägig oder über mehrere Position möglich, optional können die freigestellten Stunden angerechnet werden `Start > Änderungen > Freistellen` und `Vertretungsplan > Anrechnungen`
* FIX: Anrechenstunden für freigestellte Lehrkräfte korrigiert `Vertretungsplan > Anrechnungen`und `Start > Änderungen > Freistellen`

### Druck

* FIX: Für Kurslisten wird die ID der Schüler mit ausgegeben.

## DAVINCI Version 6.5.84 (28.08.2023)

### Allgemein

* NEW: `13_RLP_Lehrer-Soll-Schluessel.keys`
* NEW: aktualisierte Beispieldateien
* FIX: Druckdarstellung korrigiert (Darstellung mit ... in einzelnen Spalten)
  
## DAVINCI Version 6.5.83 (17.07.2023)

### Allgemein

* FIX: `Extras > Plandatei aufräumen`löscht nicht mehr manuelle Zuordnung von Schülern als Teilnehmer einer Veranstaltung `Veranstaltung bearbeiten > Teilnehmer Veranstaltung > Schüler` hat ein Schüler keine passende Kurswahl wurde er aus der Veranstaltung entfernt
* FIX: Übersicht `Extras > Jetzt` berücksichtigt Vertretungsplaninformationen
* NEW: Lehrer Soll-Ist-Schlüssel NRW, `Extras > Schlüsselverzeichnisse > Lehrer Soll-Ist-Schlüssel > Importieren` 13_NRW_Lehrer-Soll-Schluessel_BK.keys; 13_NRW_Lehrer-Soll-Schluessel_GES.keys

### Stundenplan

* FIX: `Stundenplan > Stundenplan > Zeitkonflikte anzeigen` Schienen X und A 
   
### Kursplan

* FIX: `Kursplan > Fachwahl > Sortieren` Darstellungsfehler behoben

## DAVINCI Version 6.5.82 (25.04.2023)

### Allgemein

FIX: Skalierungsfehler in Fenstern/ Ansichten gelöst

## DAVINCI Version 6.5.81 (29.03.2023)

### Allgemein

* CHANGE: Ergänzen der Registrypfade, die für den Abgleich zwischen DAVINCI und MAGELLAN10 genutzt werden
* NEW: Kalenderdateien 2023-2024

### Vertretungsplan

* FIX:Fehlstellen ohne Datumsangabe werden nicht in das ECF-Format ausgegeben 

## DAVINCI Version 6.5.80 (06.01.2023)

### Allgemein

* FIX: `Extras > Plandatei aufräumen` Augräumroutine `Veranstaltung bearbeiten > Teilnehmer Veranstaltung > Schüler`hat ein Schüler keine zur Veranstaltung passende Kurswahl, wird er als Teilnehmer der Veranstaltung gelöscht deaktiviert 
* FIX: `Dateieigenschaften > Datenschutz> Änderungen publizieren` Samstag/Sonntag werden bei der Auswahl der Tage nicht als Unterrichtstage angenommen
* FIX: Stammdaten `Extras > Weitere Aktionen > Stammdaten IDs löschen`

### Kursplan

* FIX: Synchronisationsproblem bei der Eingabe auf `Kursplan > Fachwahlen`gelöst
* 


