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

* FIX: Darstellung von Fehlzeiten in der Vertretungsansicht bei vorherigem Feiertag
* FIX: Anzeige von Wochentagen in der Vertretungsliste (davinci-substitutions.html) korrigiert
* NEW: Neuer Parameter (+ Wert) "substSort=key". Dieser Parameter arbeitet gemeinsam mit dem Parameter "substKey".
  Beispiele:
  * Gruppiert und sortiert nach Lehrer: .../davinci-substitutions.html?substKey=teacher&substSort=key
  * Gruppiert und sortiert nach Lehrer: .../davinci-substitutions.html?substKey=class&substSort=key
* FIX: Anzeige von Kalendereignissen und damit verbundenen Unterrichtsstunden
* FIX: Anzahl der Klassen in der Anzeige "Alle Klassen" erhöht

## DAVINCI Version 6.5.66

### Allgemein

* NEW: 

### STUNDENPLAN

* CHANGE: Aufruf `Plan > Importieren und Exportieren > Exportieren | Aufruf "Export f. LANiS`  umbenannt in `Plan > Importieren und Exportieren > Exportieren | Export für Schulportal Hessen`

### VERTRETUNGSPLAN

* FIX:  `Vertretzbgsplan > Vertretungen` Beim Zurücksetzen von geblockten Vertretungen wir nur die gewählte Veranstaltung zurückgesetzt nicht alle Vertretungen im Block

### SERVER

FIX: Datenübergabe an Webbox

### LOOK

* FIX:

### KURSPLAN

* FIX: `Kursplan > Blöcke > Start > Kurse und Blöcke bearbeiten > Blockbezeichnungen anpassen`
* FIX: Fehlermeldung beim Ansichtenwechsel Wechsel der Ansicht aus `Kursplan > Fachwahlen` in die Ansicht `Kursplan > Schüler` mit anschließendem Wechsel der Klasse

### DRUCK

* FIX:
  
### HTML Export

* FIX:

### Sonstiges

* FIX: 

### Webbox

* FIX: 
