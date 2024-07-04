# Änderungen 2018

## LEGENDE

Abkürzung | Bedeutung
----------|----------
FIX   | Korrektur bestehender Funktionalität
NEW   | Neue Funktionalität
CHANGE| Änderung des Ablaufs, Verarbeitung oder Bedienung

---

## Aktueller Hinweis

!!! warning "Wichtig"

Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DaVinci Look und der DaVinci WebBox: [Welche Vertretungsinformationen werden für Look oder die WebBox publiziert?]


## DaVinci Version 6.5.52

Veröffentlichung: 13.12.2018
Dateiformat: 6.0.171

### Stundenplan

* FIX: eingetragene Kernzeiten werden wieder im Planfenster abgebildet

### Vertretungsplan

* FIX: "Änderungen mitteilen" -  die fehlenden Lehrer in den Zusatzinformationen werden nicht mehr mehrfach angezeigt

![Änderungen mitteilen](/assets/images/6.5.52_01.png)

* FIX:  Doppelte Anrechnung von Vertretungsstd. bei geblockten Unterricht bei INDIREKTEN Vertretern korrigiert. Sie erhalten nun korrekterweise wieder nur eine Anrechnungsstunde.

### Look

FIX: Registerkarten unter Planfenster werden wieder angezeigt und laufen synchron mit dem gewählten Element im Plan.

## DaVinci Version 6.5.51

Veröffentlichung: 29.11.2018
Dateiformat: 6.0.171

### Server

* FIX: Änderungsgründe von Fehlzeiten werden unabhängig von den Einstellungen in DaVinci nicht für die DaVinci WebBox oder DaVinci Mobile übergeben.
* FIX: Offene Fehlzeiten (ohne abgeschlossene Vertretungsregelung) sind in der DaVinci WebBox und in DaVinci Mobile für alle Nutzer außer Nutzer mit Klassen- oder Schülerrechten sichtbar.

### Stundenplan

* FIX: Extern dat, Ausgabe der Stunden bei Unterricht mit 2 Lehrern

### Vertretungsplan

* FIX: Fehlzeit im Kursbereich (Fehlzeit eines Lehrers im Kursbereich mit anschließender Fehlzeit eines anderen Kurses führte zum Verschwinden der zuerst eingetragenen Lehrerfehlzeit)
* FIX: werden Fehlzeiten von Klassen gelöscht, mussten betroffenen offene Vertretungen für Lehrer bisher neu erzeugt werden, dies geschieht nun automatisch
* FIX: Vertretungsregelung "Wie Woche zuvor" ist wieder möglich

### Kursplan

* FIX: Im Bereich "Kursplan > Schüler" sind beim Schüler "Klasse" und "Tutor" verloren gegangen, dies wurde korrigiert.
* FIX: Im Bereich "Kursplan > Fachwahlen" wurden die Stundenwerte der Kurse verändert, diese Werte stimmen nun wieder.

### KALENDER

* FIX: Beim Anlegen neuer Ereignisse wurden Datumsangaben nicht korrekt übernommen, dies wurde korrigiert.

### Look

* FIX: offene Lehrerfehlzeiten werden wieder den Lehrer- und Klassenplänen angezeigt
* FIX: Eintrag von Fehlzeit im Enterprisebetrieb wieder möglich

### DRUCK

NEW: kompakte Wochendarstellung in der Publikation;[48],[50-52] statt [48],[49],[50],[51],[52]

### HTML Export

* FIX: Darstellung fehlender Lehrer und Klassen (nicht ganztags)

### Sonstiges

* NEW: Aktualisierung der LANIS Schnittstelle

## DaVinci WebBox Version 1.10.4 

[**UPDATE-ANLEITUNG**](https://doc.davinci6.stueber.de/09.infoserver/infoserver-und-webbox-aktualisieren/)

* FIX: geblockter Unterricht wird wieder vollständig dargestellt 
* FIX: Unterricht ohne Klassen wird wieder in den Lehrerplänen dargestellt
* FIX: eingetragener Zusatzunterricht ohne Klassen wird wieder in den Lehrerplänen dargestellt

!!! warning "Wichtig"

    Bitte beachten Sie unsere Dokumentation hinsichtlich des Umgangs mit Veröffentlichungen in DaVinci Look und der DaVinci WebBox: [Welche Vertretungsinformationen werden für Look oder die WebBox publiziert?](https://doc.davinci6.stueber.de/02.vertretungsplan/veroeffentlichung/)

## DaVinci Version 6.5.50

Veröffentlichung: 25.10.2018
Dateiformat: 6.0.171

### Stundenplan

* FIX: Die im Stammdatenfenster eingestellten Farben bei "Lehrer, Klassen, Fach, Raum" (und über die Plan-Eigenschaften aktiviert) werden wieder in die Stundenplanansicht und in Look übergeben.

## DaVinci Version 6.5.49

Veröffentlichung: 22.10.2018
Dateiformat: 6.0.171

### Look

* FIX: Nach dem Upate auf DaVinci Look 7.5.48 kam es zu Zugriffsverletztungen über die Suche und beim Öffen von Planfenstern. Dies ist korrigiert.

## DaVinci Version 6.5.48

Veröffentlichung: 19.10.2018
Dateiformat: 6.0.171

### Stundenplan

* FIX: Statistik Nordrhein-Westfalen BBS/ABS - Extern.dat gibt nun richtig die Lehrer-Ist Werte aus 
* FIX: Statistik Nordrhein-Westfalen BBS/ABS - Extern.dat gibt berücksichtigt dreistellige Schülerzahlen 

### Vertretungsplan

* FIX: Fehlzeitenerfassung bei Lehrer - wenn man im Fehlzeiten-Erfassen-Fenster mehrere Lehrer hintereinander als fehlend erfasst hat, kam es zu fehlerhaften Einträgen im Lehrerplan - dies ist korrigiert
* FIX: Raumänderungen werden im Planfenster wieder korrekt angezeigt (+VRaum (Raum)) und wieder mit den Ausdruck übergeben
* FIX: Wenn man in der Liste offenen Vertretungen am gleichen Tag  und in der gleichen Stunde mehrere offene Vertretungen hat und diese nacheinander anklickt, wurde die Anzeige rechts in der Stundenplanansicht nicht aktualisiert. Dies wurde korrigiert.
* FIX: Symbolik (Spalte "Status") in der Liste der offenen Vertretung korrigiert

![Liste der offenen Vertretungen](/assets/images/6.5.48.01.png)

### Kursplan

* FIX: Bereich "Schüler" - Blockkonflikte werden wieder angezeigt
* FIX: Bereich "Schüler" - bei Änderung des Jahrgangs wechselt nun neben der Schülerliste auch wieder der Jahrgang

### Look

* FIX: Ansicht JETZT, hat man das Layout in der Ansicht JETZT über die DaVinci Optionen von Liste <-> Matrix umgestellt, kam es zu einer Fehlermeldung. Dies wurde korrigiert.
* FIX: Lehrer/Klassen/Räume jetzt in der Matrix wieder komplett ohne Laufbalken einsehbar

### DRUCK

* FIX: Gesamtplan Lehrer - Sperrzeiten der Lehrer werden wieder an richtiger Position in den Lehrergesamtplan übergeben

## DaVinci Version 6.5.47

Veröffentlichung: 19.09.2018
Dateiformat: 6.0.170

### Stundenplan

* FIX: Mit gesetztem Haken "Vertetungsinfos anzeigen" wurden im Stundenplan Konflikte angezeigt, die es als solche nicht gibt. Dies wurde korrigiert.
* FIX: Fehlermeldung beim Öffnen des Zusatzplanfensters im Stundenplanbereich
* FIX: `Extras > Übersichten anzeigen > Listen`in der Fachkonferenzliste werden die Lehrer gezeigt, die entweder unter `Stammdaten > Fächer` ein Fach eingetragen haben oder es unterrichten.
* FIX:  Verlegung von Unterricht im Stundenplan mit er Option "Räume nicht verplanen" wird korrekt berücksichtigt
* FIX:  Zeitkonflikte aufgrund von Kernzeiten werden nicht mehr angezeigt
* NEW: aktualisierte Lehrer-Soll-Schlüssel für NRW (13_NRW_Lehrer-Soll-Schluessel.key)

### Vertretungsplan

* FIX: Ansicht ``Vertretungsplan > Fehlzeiten`` - Beim Wechsel von Klasse zu Lehrer über ``Start > Inhalt wechseln > Lehrerbutton`` kam es zu einer Fehlermeldung. 
* FIX: trägt man eine Klassenfehlzeit ein, kann man für den mitfahrenden Lehrer einen separaten Fehlgrund eingeben, die Farbe dieses Fehlgrundes wird nun mit im Plan dargestellt
* FIX: Ist in einem Unterricht mit zwei oder mehr Klassen nur eine Klasse ausgeplant, erscheint die Lehrkraft als "indirekter Vertreter"
* FIX: `Publizieren > Pläne veröffentlichen > Änderungen freigeben` - in Spalte "Status" wird wieder der grüne Haken angezeigt
* FIX: Startbildschirm "Vertretungsplan > Stundenplan" - es wird wieder ein Raum/Lehrer/Klassen-Plan für eine bestimmte Woche angezeigt
* FIX: Freistellen über mehrere Stunden korrigiert
* NEW: beim Eintrag von Fehlzeiten werden nur Datumsangaben innerhalb des Planungszeitraumes der Datei zugelassen

### Kursplan

* FIX:  aufgestockte Grundkurse /  Korrektur der Konfliktanzeige 

### DRUCK

* FIX: Druckformat: Lehrer-Zeitkonto kann  mit Logo genutzt werden
* NEW: Gültigkeitszeitraum einer Veranstaltung kann im Ausdruck mit angegeben werden

### HTML Export

* FIX: Sortierung in Tagesvertretung nach Lehrern korrigiert 
* FIX: html Vorlagen von http auf https umgestellt 

## DaVinci Version 6.5.46

Veröffentlichung: 28.08.2018
Dateiformat: 6.0.170

### Stundenplan

* FIX: Am letzten Tag der Woche wurden die Veranstaltungen nicht korrekt im Plan eingeblendet.

### Vertretungsplan

* FIX: Am letzten Tag der Woche wurden die Veranstaltungen nicht korrekt im Plan eingeblendet.

### Look

* FIX: Am letzten Tag der Woche wurden die Veranstaltungen nicht korrekt im Plan eingeblendet.

## DaVinci Version 6.5.45

Veröffentlichung: 28.08.2018 
Dateiformat: 6.0.170

### Server

* CHANGE: Bislang wurde für den Einsatz vom DaVinci InfoServer mit zwei DaVinci Servern auf dem Publikationsserver die Auswahl der Einstellung `Sensitiv für Dateiänderungen` in der DaVinci.users gespeichert. Hat man diese Datei per SIGMA vom Verwaltungsserver auf den Publikationsserver kopiert, ist auch die Einstellung mit übernommen worden. Diese Einstellung wird daher nicht mehr über den DaVinci Explorer pro Plandatei ausgewählt, sondern wird zentral über das DaVinci Server Control in der Systemsteuerung des Publikationsservers (nur dort, bitte nie auf dem Verwaltungsserver) ausgewählt. Bitte aktivieren Sie einmalig diese Einstellung!

![](/assets/images/sensitiv.haken.png)

### Stundenplan

* FIX: `Stammdaten >Schüler` - Import aus der Zwischenablage korrigiert. Es werden nun alle Felder bis auf "Datails" aus der Zwischenablage übernommen. Bitte achten Sie auf Folgendes:

  * Reihenfolge der Spaltentitel müssen in der Benennung und Reihenfolge übereinstimmen
  * bitte LISTE BEARBEITEN Modus ausschalten (siehe Screenshot, Schaltfläche `Liste bearbeiten`)
  * unter `Stammdaten > Schüler` dürfen beim Import keine Spalten ausgeblendet sein (siehe Screenshot, `*` alle Spalten müssen angehakt sein)

![Aus Ablage einfügen](/assets/images/AusAblageEinfügen.png)

* FIX: `Stundenplan > Start > Inhalt wechseln > Gehe zu > Datum`  Anzeige springt zur gewählten Kalenderwoche

* FIX: beim Öffnen des Fensters "Veranstaltung bearbeiten &gt; Teilnehmer Veranstaltung =&gt; Wechsel auf Teilnehmer Termine" aktualisiert sich die Anzeige
* FIX:  Über ``Start > Plansicht``  "Keine Angabe in Spalte "Raum" ohne Raum verplanen" können Sie steuern, ob in der manuellen & automatischen Verplanung von Stunden die Raumautomatik greifen soll. 

### Vertretungsplan

* FIX: Vertreter mit Zusatzunterricht werden bei direkten Vertretern angezeigt 
* FIX: bei der Verwendung der Dauer einer Position 90min im Zeitrahmen, wird diese Zeit korrekt in den Vertretungsplan für Zusatzunterricht und Mitteilungen übernommen 
* FIX: Lehrerfehlzeit bei Zusatzunterricht kann nun auch vertreten werden
* FIX: Es kam immer wieder vor, dass bei der Ausplanung von Lehrern unter `Vertretungsplan > Vertetungen` (Fehlzeit erfassen oder Lehrer freistellen) die Plananzeige rechts nach Eintrag zu einem beliebigen anderen Lehrer gesprungen ist. Dies sollte gelöst sein. 
* FIX: ein durch `Änderung > Raum ändern` belegter Raum wird wieder korrekt mit Blitz als belegt angezeigt
* FIX: Vertreter mit der Option "Vorziehen" werden auch bei vorliegender Raumfehlzeit wieder angeboten

### Kursplan

* FIX: `Kursplan > Kurse > Schnittmengen` Ausgabe der Schnittmenge korrigiert

### KALENDER

* NEW: `Kalender > Aufgaben`: Neuer Aufruf: `Aufgaben in Ereignisse umwandeln`

### Look

* FIX: Suche mit Kürzeln nach Lehrern oder Klassen: aus dem Klassenplan heraus wird die 1. Klasse mit dem Kürzel angezeigt, aus dem Lehrerplan heraus der 1. Lehrer

## DaVinci WebBox Version 1.10.3

Veröffentlichung: 09.07.2018

[Anleitung für die Aktualisierung](https://doc.davinci6.stueber.de/09.infoserver/update-internet-publication/infoserver-und-webbox-aktualisieren/)

* FIX: Wenn man den Parameter "teacherDisplayName" mit dem Wert "lastName" verwendete, klappte der Wechsel vom Klassenplan auf den Lehrerplan (per Klick auf das Termindetail Lehrer) nicht, dieser Punkt wurde korrigiert.

## DaVinci Version 6.5.44

Veröffentlichung: 06.07.2018
Dateiformat: 6.0.170

### Stundenplan

* FIX: Einzelne Veranstaltungen oder die gesamte Veranstaltungsliste einer Klasse kann wieder gelöscht werden.
* FIX: Zeitrahmen \| Positionsschemata bleiben auch nach dem Trennen vom Server gespeichert
* FIX: Fehler "Der Termin liegt ausserhalb des Gültigkeitzeitraums" beim Anlegen einer neuen einmaligen Veranstaltung korrigiert

### KALENDER

* FIX:  Synchronisation von Google nach DaVinci klappt wieder,  es kann wieder ein Google Kalender ausgewählt werden

### DRUCK

* FIX: Ausdruck Gesamtplan Räume - Ausgabe der Sperrungen korrigiert

### SONSTIGES

* FIX: Import/Export: Die Anmeldedaten (`DaVinci Optionen > Upload`) werden beim Export von JSON-Daten (Beispiel: Auf einen Webserver) mit übergeben.

## DaVinci WebBox Version 1.10.2

Veröffentlichung: 10.04.2018

[Anleitung für die Aktualisierung](https://doc.davinci6.stueber.de/09.infoserver/update-internet-publication/infoserver-und-webbox-aktualisieren/)

* NEW: Gebäudeplan: Die Liste der Rauminformationen wird auch bei sehr vielen Einträge durch Scrollen mit dem Mausrad im sichtbaren Bereich gezeigt.

* NEW: Vertretungsliste: Tagesaktuelle Veranstaltungen werden links in der Liste mit einem gelben Punkt gekennzeichnet.

![Tagesaktuelle Informationen werden links mit einem gelben Punkt gekennzeichnet](/assets/images/liesmich/1.10.2.01.png)

* NEW: Gebäudeplan: Eine geöffnete Rauminfo wird auch beim Vergrößern/Verkleinern der Ansicht (STRG+Mausrad) am dazugehörigen Raum gezeigt.
* Gebäudeplan: Der Parameter teacherDisplayName=lastName (...| middleName | firstName | namePrefix | nameSuffix | nickName | maidenName) ist auch für den Gebäudeplan anwendbar.
* NEW: Planansicht: Mitteilungen aus der DaVinci Vertretungsliste (`Vertretungen > Vertretungen > Spalte Mitteilung`) werden im Planfenster mit angezeigt. Diese Mitteilungen gehören jeweils zu einer Änderung, werden daher in abwechselnd (alle 5 s) mit der roten Info "Geändert", "Zusätzlich", "verschoben von" usw. mit gelben Hintergrund eingeblendet. Bitte beachten Sie, dass die Mitteilung aus der Vertretungsliste erst für abgeschlossene Vertretungselemente gezeigt wird, nicht für offene Fehlzeiten.

![Beispiel für die Anzeige von Mitteilungen aus der Vertretungsliste](/assets/images/Mitteilungstext.png)

## DaVinci Version 6.5.43

Veröffentlichung:  10.04.2018
Dateiformat: 6.0.170

### Stundenplan

* FIX: Einstellung der Nachkommastellen in den Plan-Eigenschaften unter ``Statistik`` wirkt sich auf den Druck der Lehrer-Zeitkonten aus
![Plan-Eigenschaften](/assets/images/6.5.43.01.png)

![Ausdruck "Lehrer-Zeitkonto"](/assets/images/6.5.43.03.png)

### Explorer

* FIX: Ein Löschen angelegter Benutzer ist wieder möglich.

### DRUCK

* FIX: gesetzter Haken vor "Terminzeilen umbrechen" im Druckdesign wird nun wieder richtig in den Ausdruck übergeben

![](/assets/images/6.5.43.04.png)

### SONSTIGES

* CHANGE: SDTF: Beim Import des SDTF (Schuldatentransferformats, Beispiel Import aus edoosys) wird als Trennzeichen ein Komma erwartet.

## DaVinci Version 6.5.42

Veröffentlichung: 15.03.2018  
Dateiformat: 6.0.170

* Stundenplan: Zusatzplanfenster kann wieder angezeigt werden
* Stundenplan: Import aus ASV Bayern, Klassendatei und Stundenplandatei korrigiert
* Vertretungsplan: Aufsichtsvertretungen, Lehrer die bereits eine Aufsichtsvertretung haben werden angezeigt aber mit der Info "Hat bereits Aufsicht"
* Vertretungsplan: Lehrer mit Zusatzunterricht wird nicht mehr bei direkten Vertretern angezeigt, sondern bei den indirekten Vertretern

## DaVinci Version 6.5.41

Veröffentlichung: 09.03.2018 
Dateiformat: 6.0.170

* Vertretungsplan: Verschieben von Einzelstunden, Anzeige von x-Stunde auf y-Stunde korrigiert
* Vertretungsplan: Ausdruck "Lehrervertretungen" - Zusatzunterricht von Lehrern ohne Klassenzuweisung erscheint nun richtig nur bei den Lehrern, für die Zusatzunterricht angelegt wurde
* Stundenplan: Export der Schülerkurswahlen korrigiert (`Plan > Importieren und Exportieren > Nach Magellan exportieren > Schülerkurswahlen`)

## DaVinci Version 6.5.40

Veröffentlichung: 07.02.2018
Dateiformat: 6.0.170

* Vertretungsplan: Fehlstellen, die zunächst vertreten und dann wieder zurückgesetzt wurden, tauchen wieder als offene Fehlstellen in der Liste offenen Vertetungen auf
* Vertretungsplan: `Zurücksetzen` von Vertretungen, hier kam es fälschlicherweise auch zum Zurücksetzen anderer Vertretungen - dies ist nun korrigiert
* Vertretungsplan: ein `Zurücksetzen`von Fehlstellen führt nicht zum Zürücksetzen der erzeugten Vertretungen, durch die die Fehlstelle erzeugt wurde
* Kursplan: Blockungsautomatik - es werden wieder Kurse geblockt und Schüler verteilt
* EXPORT: Korrektur des Json Exportes Schülernamen

## DaVinci Version 6.5.39

Veröffentlichung: 23.01.2018  
Dateiformat: 6.0.170

* ALLGEMEIN: korrigiert - Größe der Scrollbalken
* DaVinci Look: korrigiert - Passwortgeschützter Aufruf der Optionen
* Stundenplan: korrigiert - Anzeige der Ist-Stunden im Lehrerzeitkonto und in der Übersicht Lehrer-Zeitkonten 
* Stundenplan:  korrigiert - Passende Lehrer/Passende Räume werden jetzt bei der Analyse im Stundenplan korrekt aktualisiert
* Vertretungsplan: korrigiert - beim Vorziehen zur Vertretungserstellung wird der korrekte ausgewählte Termin eingesetzt

## DaVinci Version 6.5.38.511 WebBox Version 1.9.12

Veröffentlichung: 08.01.2018  
Dateiformat: 6.0.170

* KALENDER: neue Kalenderdateien (Ferien/Feiertagskalender) für das Schuljahr 2018/2019 stehen zur Verfügung
* WebBox / DaVinci Mobile: Korrektur im DaVinci-InfoServer. Anmeldung mit einem Lehrer- und Schüler-Recht an der WebBox/DaVinci-Mobile wieder möglich.
* Stundenplan: Fixierung von gesetzten Stunden - werden diese aus dem Plan genommen und wieder neu verplant, ist die Fixierung nun wieder richtig aufgehoben
* WebBox: Farbgebung von Mitteilungen in der WebBox nun auch wie die Standardfarbe im Vertretungsplan -gelb-
* Kursplan: Problem beim Anlegen neuer Schüler im Kursplan behoben
* Kursplan: Fehler in der automatischen Kursblockung im Servermodus behoben
* Vertretungsplan: Fehlstellen, die durch das Vorziehen von Unterricht erzeugt wurden, werden nun durch ein Zurücksetzen der Vertretungen auch gelöscht (zurückgesetzt)
* Stundenplan: Aktualisierungsproblem im Zusatzfenster "passende Lehrer", "passende Räume" und "Unverplant" gelöst
