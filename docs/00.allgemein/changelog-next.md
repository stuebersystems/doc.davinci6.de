# Voraussichtliche Änderungen

!!! info "Hinweis"

    Sie erhalten hier einen Überblick über die voraussichtlichen Änderungen und Korrekturen für das nächste Serviceupdate.

## LEGENDE

| Abkürzung | Bedeutung |
| --- | --- |
| FIX | Korrektur bestehender Funktionalität |
| NEW | Neue Funktionalität |
| CHANGE | Änderung des Ablaufs, Verarbeitung oder Bedienung |

## DAVINCI MOBILE APP [unveröffentlicht]

* NEW: Testfunktion für die Serververbindung
* NEW: Im Detailfenster einer Veranstaltung (Klick aufs Terminfeld) werden für Vertretungen auch die Vertretungsinformation und die Vertretungsmitteilung gezeigt (beide Informationen werden in DAVINCI Vertretungsplan in der Vertretungsliste in den gleichnamigen Spalten erfasst)
* NEW: Die Bezeichnung des Klassenfehlgrunds wird beim Klick auf ein Terminfeld im Detailfenster zusätzlich zur Information "Klasse fehlt" gezeigt. 

## DAVINCI WEBBOX Version 1.10.6 \[unveröffentlicht\]

[**UPDATE-ANLEITUNG**](https://doc.davinci6.stueber.de/09.infoserver/infoserver-und-webbox-aktualisieren/)

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DAVINCI LOOK und der DAVINCI WEBBOX: [Welche Vertretungsinformationen werden für LOOK oder die WEBBOX publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

* FIX: Der Parameter `substitutionShowExtra` wurde korrigiert
* NEW: Die Bezeichnung des Klassenfehlgrunds wird am oberen Rand des Terminfensters hinter der Info "Klassen fehlt" eingeblendet. Ein Beispiel: "Klasse fehlt: Distanzunterricht"

## DAVINCI Version 6.5.69

### Allgemein

* NEW: 

### STUNDENPLAN

* FIX: mehrtägige Ereignisse werden wieder korrekt im Zusatzkalender gespeichert/angezeigt
* FIX: Ereignisse (von-bis Zeit) werden wieder korrekt im Zusatzkalender gespeichert/angezeigt
* NEW: Kalenderdateien Ferien 2021/2022
  
!!! info "Hinweis"

    Vorab können Sie die Kalenderdateien [hier](https://my.hidrive.com/share/63dd-bod4u) herunterladen

* FIX: Aufsichtsplan: Lehrer, die bereits einem Aufsichtsbereich zugewiesen sind, stehen in anderen Bereichen zur selben Zeit wieder zur Auswahl
  ![Aufsichtsplan](/assets/images/liesmich/6.5.69.01.png)

### VERTRETUNGSPLAN

* FIX: V-Lehrer für Aufsichten - eine Lehrkraft kann nun wieder mehrere Bereiche vertreten, d.h. sobald eine Lehrkraft einem Aufsichtsbereich zugewiesen ist, steht diese wieder als möglicher Vertreter zur Auswahl (mit der "Bemerkung" - bereits Aufsicht zu dieser Zeit). 

### SERVER

* FIX: 

### LOOK

* FIX:

### KURSPLAN

* FIX: `Kursplan > Fachwahlen` Fachschwerpunkt auswählbar
  
### DRUCK

* FIX: `Design > Liste> Klassenfehlzeitermine anzeigen`reguläre Stunden ohne V-Planänderungen werden nicht mehr ausgegeben
  
### HTML Export

* FIX: HTML-Main-Vorlagen: Buttons werden wieder korrekt dargestellt

### Sonstiges

* FIX: 

### Webbox

* FIX: 

### Analytics

* FIX: Ausfallstatistik - Ausgabe der Werte `Zeitraum > Verplant` bei der Auswahl mehrerer Tage
