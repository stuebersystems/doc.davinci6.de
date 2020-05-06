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

## DAVINCI Version 6.5.65

### Allgemein

* NEW: Die DAVINCI-Mailschnittstelle kann für 32 Bit- und 64 Bit-Mailclients verwendet werden

### STUNDENPLAN

* NEW: Die MAGDAVINCI-Mailschnittstelle kann für 32 Bit- und 64 Bit-Mailclients verwendet werden. Sollte nicht der von Ihnen erwartete Mailclient aufgerufen werden, schauen Sie bitte folgenden Artikel an [Welcher Mailclient wird aufgerufen?](https://doc.kb.stueber.de/sonstiges/mapi2.html).
* FIX: Eintragung `Stammdaten > Schüler > Stufe`; wenn keine Klasse zugeordnet ist, ist eine Klasse zugeordnet, wird die Stufe der Klasse in der Spalte Stufe angezeigt
* FIX: `Stammdaten > Klassen > Klassen löschen` und `Plan > Neu > Daten übernehmen`beim Löschen der Klasse incl. deren Veranstaltungen wurden Veranstaltungsverweise im Kalender (Veranstaltungen bzw. Kurse können einem Kalendereintrag zugewiesen) nicht gelöscht
* FIX: manuelle Verplanung von Räume in Berücksichtigung der Vorgaben bei `Planansicht > Verplanen > Räume`

### VERTRETUNGSPLAN

* FIX: 

### SERVER

<<<<<<< HEAD
FIX: Datenübergabe an die Webbox Übergabe von Zusatzunterricht bei Klassen mit Fehlzeit
=======
CHANGE: Zusatzunterricht für als fehlend gekennzeichnete Klassen wird auch für Nutzer mit dem Profil Klasse in der Webbox und in der Mobile App gezeigt
>>>>>>> c4029258467cce6132875e1d3512780cf70af159

### LOOK

* FIX:

### KURSPLAN

* FIX:

### DRUCK

* FIX:
  
### HTML Export

* FIX:

### Sonstiges

* FIX: 

### Webbox

* FIX: 
