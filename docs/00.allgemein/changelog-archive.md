# Änderungen 2014 (und früher)

## Version 6.0.181 (10.12.2014) Dateiformat 6.0.126 

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

### Fehlerkorrektur

* SETUP: Fehler beseitigt
* VERTRETUNGSPLAN: Das Eintragen eines Vertretungslehrer und eine anschließende gesonderte Raumänderung (Fehltzeit Raum) für die gleiche Unterrichtsstunden sind jetzt wieder möglich.
* VERTRETUNGSPLAN: "Folgende Termine analog vertreten" und Vertretung "Wie Woche zuvor" wieder möglich.

## Version 6.0.180 (08.12.2014)

### Verbesserte bzw. geänderte Funktion

* NEW: Neue Option  unter „Extras|Optionen|Ansicht|Lehrer-Ist Werte in Zeitkonten|Welcher Wert soll bei „Ist“ angezeigt werden“ ist jetzt für alle Verrechnungsarten verfügbar.

### Fehlerkorrektur

* SETUP: Fehlender Shortcut für DAVINCI
* VETRETUNGSPLAN: Vorziehen und anschließende Ramänderung fürhte dazu, dass Vertretungslehrer gelöscht wurde. Der Fehler ist behoben.

## Version 6.0.179 (05.12.2014)

### Fehlerkorrektur

* SETUP: Fehler beseitigt

## Version 6.0.178 Dateiformat 6.0.125 (04.12.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

### Fehlerkorrektur

* ALLGEMEIN: Fehlermeldung "Sie dürfen nur Daten Ihres Teams bearbeiten" im lokalen Betrieb korrigiert
* STUNDENPLAN: bearbeiten der Daten im Mehrbenutzerbetrieb (Stunden setzten, verschieben, Stammdaten bearbeiten) wieder möglich
* STUNDENPLAN: bearbeiten der Zeitpräfenrenzen im Mehrbenutzerbetrieb wieder möglich
* STUNDENPLAN: Stammdaten bearbeiten im Mehrbenutzerbetrieb wieder möglich
* STUNDENPLAN: LUSD Import doppelte Schüler bereinigt
* STUNDENPLAN: Neue Option in den DAVINCI-Optionen im Register "Ansicht": "Lehrer Ist-Werte in Zeitkonten"; damit kann eingestellt werden, ob im Zeitkonto als "Ist-Wert" der "Geplant-Wert" (lt. Veranstaltungsliste) oder "Verplant-Wert" (lt. gesetzten Stunden) ausgeben werden soll. HINWEIS: Standardmäig wird als "Ist-Wert" der "Geplant-Wert" ausgeben
* VERTRETUNGSPLAN: bei geblockten Veranstaltungen können Raumvertretungen wieder für Folgetermine übernommen werden
* VERTRETUNGSPLAN: Fehlstellen können wieder durch "Vorziehen" von Stunden gefüllt werden
* INFOSERVER: Übergabe der Daten vom daVinci-Server für den Infoserver korrigiert
* DRUCK: Ausdruck der Vertretungspläne ergänzt um die Spalten "Original Fach/Lehrer/Raum"

## Version 6.0.176 (17.10.2014)

### Neue Funktionen

* STUNDENPLAN: Automatiklauf lässt sich nach Teams filtern
* STUNDENPLAN: Situation zum Zeitpunkt Register "Räume" zeigt auch Kapazität und Raumart
* STUNDENPLAN: Stammdaten "Perioden" und "Ressourcen" haben jetzt auch eine Spalte "TEAM"
* STUNDENPLAN: Veranstaltungsliste > Veranstaltungen fortschreiben: Um PERIODE ergänzt und alle Elemente einer Blockung werden fortgeschrieben.
* STUNDENPLAN: Veranstaltungsliste > Veranstaltungen befristen: Um PERIODE ergänzt und alle Elemente einer Blockung werden befristet.
* STUNDENPLAN: Veranstaltungsliste > Veranstaltungen kopieren: Um PERIODE ergänzt. Es kann optional eine Periode auswählen werden, die dann den markiertern Veranstaltungen in Kopie zugewiesen wird.
* STUNDENPLAN: Neuer Befehl RECHTE MAUSTASTE > Termine verschieben = verschiebt einmalige Termine auf anderen Tag, es können auch mehrere Termine markiert und verschoben werden.
* STUNDENPLAN: Man kann jetzt den Endzeitpunkt in der Veranstaltungsliste und im Plan mit RECHTE MAUS * TERMINZEITDAUER BERBEITEN verändern.
* STUNDENPLAN: "Jahresverteilung" - ersten Spalten (Bereich Summen) sind nun fix, in die einzelen Kalenderwochen scrollt man wie gewohnt.
* * VERTRETUNGSPLAN: Erfassen von Klassenfehlzeit und der daraus resultierende Fehlzeiten/Anrechenstunden von Lehrern, Neu -> über "Hinzufügen" können Lehrer, die die Klasse zur Klassenfehlzeit nicht unterrichten hinzugefügt werden.
* VERTRETUNGSPLAN: Vorziehen von geblockten Stunden > Beim Vorziehen von geblockten Stunden kann im Dialogfenster "Vorziehen" die neue Option eingstelt werden, ob der gesamte Block (alle Termine des Blocks) vorgezogen werden sollen. 
* VERTRETUNGSPLAN: Vorziehen von mehrstündigen Veranstaltung > Beim Vorziehen von mehrstündigen Veranstaltungen wird im Plan und im Ausdruck in der Vertretungsinformationen zusätzlich mit ausgewiesen von-bis welcher Position verschoben wurde.
* INFOSERVER: für die Ausgabe von Klassenvertretungen, Lehrervertretungen und Vertretungslehrern (Parameteraufrufe classsubst, teachersubst und substteacher) gibt es jeweils eine Indexseite
* IMPORTIEREN/EXPORTIEREN: Der "Allgemeine Statistikexport" wurde erweitert
* IMPORTIEREN/EXPORTIEREN: WinLD Export korrigiert bei geblockten Veranstaltungen mit unterschiedlichen Perioden 
* Allgemein: Extras|Weitere Aktionen|Zeitverschiebung > Verschiebt die Zeitangaben von Terminen, Ereignissen, Fehlzeiten und Änderungen wochenweise. 

### Fehlerkorrektur

* STUNDENPLAN: Zusatzfenster (F12) können wieder angezeigt werden 
* STUNDENPLAN: Aktualisierungsproblem beim Wechsel von Ansicht "Liste" zu "Plan und Liste" behoben
* STUNDENPLAN: Komprimierte DAVINCI Datei kann wieder mit gleichem Namen überschrieben werden
* VERTRETUNGSPLAN: Anzeige direkter Vertreter bei den indirekten korrigiert
* VERTRETUNGSPLAN: Statistik|Unterrichtsausfall
* VERTRETUNGSPLAN: Raumtausch zwischen Veranstaltungen wird nun korrekt im Lehrerplan angezeigt
* VERTRETUNGSPLAN: Lehrertausch wird in den Lehrplänen wieder korrekt angezeigt 
* VERTRETUNGSPLAN: wenn das Fach durch Vorziehen einer Veranstaltung geändert wurde, ist Anzeige in Spalte "Fach" wieder wie folgt: „+V-Fach(Fach)“
* VERTRETUNGSPLAN: Veranstaltung mit Terminfolge größer als 3 wird nun korrekt über den Befehl "Teilen" in Einzelstunden aufgeteilt
* VERTRETUNGSPLAN: gelbe Markierung für offene Vertretungen von Aufsichten wieder vorhanden
* KURSPLAN: Fehlende Zuordnung von Schülerfachwahlen zu Kursen behoben
* DRUCK: Beim Druck der Kursliste wird die Klasse des Schüler ausgegeben (vorher alle Klassen des Kurses)
* DRUCK: Ausdruck von Lehrerplänen mit Veranstaltungsliste wieder möglich
* DRUCK: Druckformat "Aufsichtsplan" - es können Langnamen der Lehrer ausgegeben werden
* DRUCK: Druckformat "Veranstaltungsliste Klasse"  - Spalte "Schüler" wird wieder befüllt 
* ALLGEMEIN: Der Befehl "Plan|Server verwalten" ist nicht verfügbar, wenn man in der Registry unter "HKEY_CURRENT_USER/Software/Stueber Systems/daVinci 6/Main" neu einen DWORD-Wert "NoServerManage=REG_DWORD 0x000000001(1)" angibt.
* ALLGEMEIN: Wenn man in der Registry unter "HKEY_CURRENT_USER/Software/Stueber Systems/daVinci 6/Main"  neu einen DWORD-Wert "NoUpdates=REG_DWORD 0x000000001(1)" angibt, dann wird die Schaltfläche "Extras|Aktualisieren" und die Lizenzeingabe-Schaltflächen ausgeblendet.
* ALLGEMEIN: Die Daten unter "Plan|DAVINCI-Optionen|Meine Daten|Allgemein" werden standardmäßig zentral in der Datei "daVinci.site" im gleichen Ordner wie die EXE-Dateien abgelegt. Für zentrale Installationen (z.B. Terminalserver) kann diese Datei im Ordner "daVinciDataFolder" (unter Windows 8 z.B. C:\Users\%BENUTZER%\AppData\Roaming\Stueber Systems\daVinci 6" gepeichert werden, wenn man in der Registry unter "HKEY_LOCAL_MACHINE/Software/Stueber Systems/daVinci 6/Main" neu einen DWORD-Wert "SiteFileLocal=REG_DWORD 0x000000001(1)" angibt.
* HTML Export: alle Positionen (voreingestellt bei "Mindestens bis") werden beim Export wieder korrekt ausgegeben
* HTML Export: Aufsichten bei Lehrern, die nach der Aufsicht in ihrem Plan keinen Unterricht haben, werden nun wieder ausgegeben
* EXPLORER:  Teamzugehörigkeitsrechte ergänzt
* LOOK: Anwendung kann pro Arbeitsplatz wieder mehrfach geöffnet werden.
* LOOK: Lehrersuche in "Lehrer Jetzt" korrigiert 
* LOOK: Mit der LOOK Installation werden nun auch die Druckformate mit installiert.

## Version 6.0.175 (12.09.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

### Neue Funktionen

* ALLGEMEIN: Option „Plan|Eigenschaften|Datenschutz|Fehlgrund im Titel geänderter Termine anzeigen“ zeigt jetzt Fehlgrund+Änderungstitel an (vormals nur Fehlgrund bei markierter Option)
* ALLGEMEIN: Neue Option „Plan|Eigenschaften|Datenschutz Lehrer-Veranstaltungen und -Zeitkonten in DAVINCI LOOK nicht druckbar“ verhindert es, dass Benutzer in DAVINCI LOOK Lehrer-Veranstaltungslisten und Lehrer-Zeitkonten drucken, diese Kollegendaten können also nicht angezeigt werden.
* STUNDENPLAN: Im Stundenplanbereich gibt es neu unter „Ansicht“ den Aufruf „Drei Pläne“. Es werden Klassen-, Lehrer- und Raum Plan korrespondierend nebeneinander geöffnet.
* STUNDENPLAN: Neue Ansicht „Stundenplan|Tagesplan“ für das Setzen von Jahresterminen (siehe dazu entsprechendes Kapitel im Benutzerhandbuch).
* STUNDENPLAN: Beim Aufruf „Jetzt“ wird nun auch die "Position" (Positionsnummer) angezeigt
* STUNDENPLAN: Unverplant Fenster | neue Option „Ohne Räume verplanen" 
* VERTRETUNGSPLAN: Die Lehrerart ist jetzt neu einblendbar in der VERTRETUNGEN ERSTELLEN Ansicht.
* VERTRETUNGSPLAN: Im Dialog Zusatzunterricht können jetzt b Lehrer und Räume gefiltert werden.
* VERTRETUNGSPLAN: Vertretungsplan|Vertretungen: neue Funktion: Status "offen" kann mit rechter Maustaste auf erledigt gesetzt werden, wenn keine Vertretung erstellt werden soll 
* VERTRETUNGSPLAN: Zusatzunterricht wird jetzt standardmäßig in Blau ausgewiesen. Die Farbe kann jetzt über das Optionen-Dialogfenster frei gewählt werden.
* VERTRETUNGSPLAN: Neues Dialogfenster „Raumvertretung“ in der Ansicht VERTRETUNGEN erlaubt es alle Räume im Block bzw. alle Termine des Fehlzeitraums gleichzeitig zu vertreten, analog zu Lehrervertretungen.
* DRUCK: Auswahl filtern nach mehreren Teams möglich
* DRUCK: Ausdruck "Kurslisten" - Spalten aus dem Stammdatenfenster "Schüler" sind optional ausdruckbar
* DRUCK: Kursliste lässt sich  vollständig formatieren 
* HTML Export: Auswahl filtern nach mehreren Teams möglich

### Fehlerkorrektur

* ALLGEMEIN: Der Befehl "Plan|Server verwalten" ist nicht verfügbar, wenn man in der Registry unter "HKEY_CURRENT_USER/Software/Stueber Systems/daVinci 6/Main" neu einen DWORD-Wert "NoServerManage=REG_DWORD 0x000000001(1)" angibt.
* ALLGEMEIN: Wenn man in der Registry unter "HKEY_CURRENT_USER/Software/Stueber Systems/daVinci 6/Main"  neu einen DWORD-Wert "NoUpdates=REG_DWORD 0x000000001(1)" angibt, dann wird die Schaltfläche "Extras|Aktualisieren" und die Lizenzeingabe-Schaltflächen ausgeblendet.
* ALLGEMEIN: Die Daten unter "Plan|DAVINCI-Optionen|Meine Daten|Allgemein" werden standardmäßig zentral in der Datei "daVinci.site" im gleichen Ordner wie die EXE-Dateien abgelegt. Für zentrale Installationen (z.B. Terminalserver) kann diese Datei im Ordner "daVinciDataFolder" (unter Windows 8 z.B. C:\Users\%BENUTZER%\AppData\Roaming\Stueber Systems\daVinci 6" gepeichert werden, wenn man in der Registry unter "HKEY_LOCAL_MACHINE/Software/Stueber Systems/daVinci 6/Main" neu einen DWORD-Wert "SiteFileLocal=REG_DWORD 0x000000001(1)" angibt.
* STUNDENPLAN: Automatik erzeugt "Konflikte" – bitte führen Sie einmal den Befehl Extras|Plandatei aufräumen durch und starten dann die Automatik
* STUNDENPLAN: Exportieren|Statistik Export NRW korrigiert
* STUNDENPLAN: Mit der F12 Taste kann das Zusatzplanfenster geöffnet werden 
* STUNDENPLAN: WIN LD Export für ABS unter dem Aufruf "Import/Export|Statistik Bayern WIN LD" integriert
* STUNDENPLAN: Ausgabe "Dauer" in der Veranstaltungsliste bei gesetzten Terminen korrigiert, wenn angehakt: "Termin-Ende automatisch an Zeitrahmen anpassen"
* STUNDENPLAN: F6 Klassenplan anzeigen, F7 Lehrerplanplan anzeigen, F8 Raumplanplan anzeigen
* STUNDENPLAN: Zusatzfenster "Summen" | Lehrplan - Fehler, dass der "Geplant"-Wert verändert wird sobald eine Veranstaltungen gesetzt ist, korrigiert
* STUNDENPLAN: Jahresverteilung 
* VERTRETUNGSPLAN: Einrichten einer Fehlzeit mit der Option "Nicht öffentlich" korrigiert, diese wird nun nicht mehr in daVinci Look angezeigt
* VERTRETUNGSPLAN: "Ressourcen zuweisen" im lokalen Betrieb nun möglich
* VERTRETUNGSPLAN: "Immer Uhrzeiten anzeigen“ wird auch für den Zusatzunterricht korrekt dargestellt
* VERTRETUNGSPLAN: Zusatzunterricht - "von" - "bis" Datum kann eingetragen werden
* VERTRETUNGSPLAN: Zusatzunterricht – Option „Nicht öffentlich“ kann erfasst werden, um diesen ggf. nicht zu veröffentlichen
* VERTRETUNGSPLAN: Zusatzunterricht – Filtermöglichkeit in Register "Räume" nach "freie Räume", "Raumart", "Kapazität" und "Teams
* VERTRETUNGSPLAN: Anrechenstunden beim Zusatzunterricht korrekt erfasst
* VERTRETUNGSPLAN: Ressourcen buchen, zusätzlich gebuchte Raumressource - Eintrag wird im Raumplan angezeigt
* VERTRETUNGSPLAN: direkte Vertreter die Freistunde haben, werden in Spalte "Art" wieder mit "Zusätzlich" ausgewiesen
* VERTRETUNGSPLAN: Unterrichtsgarantie Plus/Verlässliche Schule HESSEN - Die externen Vertreter werden in daVinci unter „Stammdaten|Lehrer“ eingetragen und entsprechend der drei Lehrerarten als „Vertreter 1“, „Vertreter 2“, bzw. „Vertreter 3“ in der Spalte „Lehrerart“ gekennzeichnet. (1. Personen ohne Befähigung für ein Lehramt, aber mit abgeschlossenem Studium an einer Hochschule, Fachhochschule oder mit abgeschlossener Berufsausbildung, 2. Personen mit Befähigung für ein Lehramt 3. Personen, auf die 1 und 2 nicht zutreffen) Hierfür definieren Sie im Schlüsselverzeichnis "Lehrerart" die Vertreter "Vertreter1", "Vertreter2" und "Vertreter3". Im Vertretungsplan kann nun neu im "Vertretungen"-Fenster in der Auswahl der möglichen Vertreter die Spalte „Lehrerart“ angezeigt werden. Dort erkennen Sie z.B. am Eintrag „Vertreter1“, dass es sich um einen externen Vertreter der Lehrart1 handelt.
* VERTRETUNGSPLAN: Raumänderung bei geblockten Unterricht, neues Dialogfenster bei der Vertretungsregelung "Weitere Termine dieses Raums im Block analog vertreten" 
* VERTRETUNGSPLAN: Priorität" "Fach" erscheint, wenn Lehrer in den Stammdaten diesem Fach zugewiesen ist  
* VERTRETUNGSPLAN: Priorität" "Klasse" erscheint nur bei wieder bei zusätzlich gehaltenem Unterricht
* KURSPLAN: Ansicht "Schüler" - Ausdruck der Fachwahlen nur für bestimmte Schüler ist möglich, wenn man die Liste filtert. Man filtert nach den Schülern, für die man die Fachwalliste ausgeben möchte und startet den Druck.
* KURSPLAN: Ansicht „Kurse“: Sperrt man einen einzelnen Kurs (Haken setzen in Spalte "gesperrt"), wird der Haken sofort gespeichert, ohne erst in eine andere Zeile zu wechseln um zu aktualisieren.
* KURSPLAN: Ansicht „Kurse" Zusatzfenster "Kursteilnehmer“: Die Schaltfläche „Aus diesem Kurs entfernen“ wurde herausgenommen.
* EXPLORER: Import Benutzer 

## Version 6.0.173 (22.08.2014)

> Einige benutzerdefinierte Einstellungen wie Fensterpositionen, -größen, Voreinstellungen werden mit diesem Update zurückgesetzt.

* Druckformate: Raumpläne|Wochenplan Räume korrigiert, eingestelltes "Von" und "Bis" Datum wird berücksichtigt
* Stundenplan: Ansicht "Unterrichtsmatrix", Darstellung bei geblockten Veranstaltungen in Register "Klassen-Lehrer" korrigiert
* Vertretungsplan: Ansicht "Vertretungen", bei den Vertretungslehrern wird in Spalte "Art" wieder angezeigt, wenn eine Lehrer eine Ausfallstunde aufgrund einer Klassenfehlzeit hat (Ausfallstd Klasse) 
* Vertretungsplan: Fehlgrundanzeige im Titel geänderter Termine (die man in den DAVINCI-Eigenschaften unter "Vertretungsplan" aktivieren kann) wird nun auch bei Doppelstunden ausgegeben
* Stundenplan: WinLD-Export löst wieder richtig den WinLD-Export aus 
* ÜBERSICHTEN: "Zeitkonten" gibt nun auch die Spalten "Bezeichnung" und "Kürzel" der zugwiesenen Lehrer-Soll-Schlüssel aus
* Neue Ansicht ÜBERSICHTEN: "Jahresplanung" (setzt ANALYTICS Lizenz voraus).
* Neue Ansicht ÜBERSICHTEN: "Lehrerausfall" überarbeitet, summiert jetzt auch Zusatzunterricht (setzt ANALYTICS Lizenz voraus).
* Dialogfenster "Ressourcen/Räume zuweisen" überarbeitet und Fehler korrigiert.
* Die Daten unter "Plan|DAVINCI-Optionen|Meine Daten|Allgemein" werden standardmäßig zentral in der Datei "daVinci.site" im gleichen Ordner wie die EXE-Dateien abgelegt. Für zentrale Installationen (z.B. Terminalserver) kann diese Datei im Ordner "daVinciDataFolder" (unter Windows 8 z.B. C:\Users\%BENUTZER%\AppData\Roaming\Stueber Systems\daVinci 6" gepeichert werden, wenn man in der Registry unter "HKEY_CURRENT_USER/Software/Stueber Systems/daVinci 6/Main" neu einen DWORD-Wert "SiteFileLocal=REG_DWORD 0x000000001(1)" angibt.
* Wenn man in der Registry unter "HKEY_LOCAL_MACHINE/Software/Stueber Systems/daVinci 6/Main" neu einen DWORD-Wert "NoUpdate=REG_DWORD 0x000000001(1)" angibt, dann wird die Schaltfläche "Extras|Aktualisieren" und die Lizenzeingabe-Schaltflächen ausgeblendet.

## Version 6.0.172 (31.07.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* STUNDENPLAN: Lehrer-Ist-in-Klasse- und Geplant-Werte beim Setzen im Klassenplans angepasst
* STUNDENPLAN: Die Felder Wochen und Periode sind in der Terminliste gleich denen der Veranstaltung vorbesetzt
* STUNDENPLAN: Beim Anpassen der Terminaufteilung (zum Beispiel von 2 auf 1-1) bleibt die Dauer der Veranstaltung gleich
* STUNDENPLAN: Stundenplanung über Pausen in Stundenlänge angepasst
* STUNDENPLAN: unter Stammdaten|Klasse|Stufe wird der Wert "0" angezeigt
* STUNDENPLAN: Raumautomatik für in den Stammdaten vorgebene Fachräume optimiert
* STUNDENPLAN: Anzeige unter Unterrichtsmatrix|Klassen-Fächer für Veranstaltungen mit Kursnummern korrigiert
* STUNDENPLAN: Beim Löschen der Raumvorgabe aus der Veranstaltungsliste|Spalte "Räume" bleibt der Raum bei gesetzten Veranstaltungen bestehen
* STUNDENPLAN: Ausgabe der Differenz im Ausdruck der Lehrer-Soll-Berechnung unter Lehrerplänen korrigiert
* STUNDENPLAN: Problem beim Speichern von Optionen für Länder außer Deutschland korrigiert
* VERTRETUNGSPLAN: unter Plan|Eigenschaften|Vertretungsplan kann für DAVINCI und für LOOK eingestellt werden, ob die Fehlgründe für Abwesenheiten gezeigt werden sollen
* VERTRETUNGSPLAN: wird für einen Termin zuerst der Raum geändert, anschließend eine Lehrerfehlzeit eingetragen, stimmt die Ausgabe in der Vertretungsliste
* VERTRETUNGSPLAN: Fehlerhafte Einträge in der Änderungsliste (30.12.1899) können über Extras|Plan aufräumen korrigiert werden
* Skript: RLP-FW-APO-BGY-2010.js geändert für den Verordnungstyp GS

## Version 6.0.171 (18.07.2014)

* STUNDENPLAN: geplant/verplant-Werte im Lehrerplan angepasst
* STUNDENPLAN: wenn einer Klasse eine Periode zugewiesen wurde, wird diese auch für alle anschließend gesetzten Veranstaltungen übernommen
* KURSPLAN: Beim Kurswechsel aufgetretene Probleme können über Hilfe|Plan aufräumen behoben werden
* STUNDENPLAN: unter Stundenplan|Automatik gibt es die Möglichkeit die Raumzuweisungen eines Planes zurückzusetzen. Optional alle Raumzuweisungen oder nur die durch die Automatik erzeugten Zuweisungen.
* Allgemein: bei der Planübernahme fürs neue Schuljahr wird aus der Vorjahresdifferenz ein D-Schlüssel im Zeitkonto des Lehrers angelegt

### Pre-Release 6.0.170 (15.07.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* STUNDENPLAN: Lehrer-Zeitkonto IST- Wert bei tages- und wochenbezogener Berechunng korrigiert
* STUNDENPLAN: Aktualisierung des Wochenfaktors bei Perioden: Start|Bearbeiten|Faktor aktualisieren
* STUNDENPLAN: Ansicht im Stundenplan bei Ereignis erfasst (nicht ganztätig, unterrichtsfrei) korrigiert
* LOOK: Optionen werden korrekt gespeichert
* HTML Export: Problem beim Abändern duplizierter HTML-Exportformate korrigiert
* VERTRETUNGSPLAN: Doppelstunden werden bei gesetzter Option (Optionen|Vertretungsplan)als Einzeltermine zur Vertretung in der Vertretungserstellung angeboten
* VERTRETUNGSPLAN: In der Ansicht Vertretungen|Anrechnungen wird das Lehrerkürzel für Zusatzunterricht mit angezeigt
* VERTRETUNGSPLAN: Lehrerfehlzeit für Einzelstunde einer Doppelstunde korrigiert
* VERTRETUNGSPLAN: ganztägige Fehlzeit, die als doppelspaltige Anzeige erscheint bitte mit "Extras|Plandatei aufräumen" korrigieren
* Allgemein: Es kann ein serverseitiges Backup für den Serverbetrieb eingestellt werden. Bitte wählen Sie dazu die Option auf der Resiterkarte "Backup" im daVinci-Server-Control in der Systemsteuerung. Das Backup wird im Arbeitsbereich des daVinci-Servers erstellt, Sie können zusätzlich wählen, nach wie vielen Tagen Backups wieder gelöscht werden sollen.
* Allgemein: Backup-Dateien werden mit "Datum.backup" benannt, also z.B. „beispiel.2014-07-14.backup“.
* Allgemein: Die Option für das Nicht-Anzeigen von Fehlgründen gilt nun auch für DAVINCI (unter "Plan|Eigenschaften|Vertretungsplan"). Bisher galt sie nur für LOOK.


## Version 6.0.169 (02.07.2014)

* EXPLORER: Der "Administrator" heißt jetzt "Super-Administrator", da es nun auch einen "Sub-Administrator" (für mandantenfähige DAVINCI Versionen, Dokumentation folgt noch) gibt.
* STUNDENPLAN: Veranstaltungsliste: Befristung mehrerer markierter Veranstaltungen über "Veranstaltung|Veranstaltung bearbeiten|Veranstaltung befristen" möglich
* STUNDENPLAN: Duplikate einer bereits gesetzten Veranstaltung werden wieder als unverplant in der Veranstaltungsliste aufgeführt
* STUNDENPLAN: Eintrag einmaliger Sperrungen
* VERTRETUNGSPLAN: Unter "Eigenschaften|Vertretungsplan" kann eingestellt werden, wie Fehlgründe in DAVINCI LOOK angezeigt werden (1. „Keine Fehlgründe anzeigen“ - es werden in LOOK keine Fehlgründe angezeigt | 2. „Alle Fehlgründe als "abwesend" anzeigen“ - es werden in LOOK ALLE Fehlgründe als "abwesend" anstatt von z.B. "krank" angezeigt | 3. „Alle Fehlgründe anzeigen“ - es werden in LOOK ALLE Fehlgründe mit der im Schlüsselverzeichnis zugewiesenen Farbe angezeigt)
* VERTRETUNGSPLAN: beim Erfassen einer Fehlzeit gibt es optional die Möglichkeiten (beides gilt nur für LOOK)Fehlzeiten nicht öffentlch -- Fehlzeit und die damit verbundenen Änderungen werden nicht angezeigt 
* KURSPLAN: Ansicht "Blöcke|Kursteilnehmer" - wenn man Alternativkurse anklickt, werden nun automatisch passende Schüler farblich markiert
* KURSPLAN: Blöcke erzeugen, gibt automatisch als Vorgabe die minimal benötigten GK und LK vor
* LOOK: Ansicht Klasse/ Lehrer/ Raum jetzt in Listenansicht Sortierung nach einem Spaltenkopf wird beibehalten
* LOOK: Ansicht Klasse/ Lehrer/ Raum jetzt in Listenansicht Ausgabe von-bis
* HTML Export: Zugriffsverletzung beim Export von Klassenvertretungen korrigiert
* Druckformate und HTML Formate für Stundenpläne: Auf der Registerkarte "Termine" kann über die neue Option "Originaltermine bei Änderungen nicht anzeigen" eingestellt werden, ob z.B. in Raumplänen der durch eine Raumfehlzeit entfallende Termin angezeigt werden soll oder nicht.

## Version 6.0.168 (24.06.2014)

* STUNDENPLAN: Automatik|Lehrereinsatz zurücksetzen (Auswahl nach nur der Automatik zugewiesenen Lehrern oder alle Lehrer)
* VERTRETUNGSPLAN: Übersicht Lehrerausfall korrigiert
* VERTRETUNGSPLAN: HTML-Export Klassenvertretungen

## Version 6.0.167 (23.06.2014)

* VERTRETUNGSPLAN: Aufruf der Änderungsliste korrigiert

## Version 6.0.166 (20.06.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* LOOK: Wechsel in die Ansicht Räume, Lehrer, Klassen Jetzt korrigiert
* STUNDENPLAN: Zuweisen von zwei Lehrern in der Veranstaltungsliste wird auch in die Terminzeilen übernommen
* STUNDENPLAN; Fehler und Planvorbereitungsassistent korrigiert, der dazu führte, dass beim Löschen von Lehrerdaten, die Datei nicht mehr zu bearbeiten war (Bitte beachten Sie, dass die Planübernahme erneut durchgeführt werden muss!)
* STUNDENPLAN: Überschneidungen beim Setzen, die nur innerhalb des Planes auftreten, werden jetzt als gelber Streifen rechts hinter einem Eintrag angezeigt (d.h. auf den im Plan gelb schraffierte Positionen kann gesetzt werden, wenn der mit einem Strefifen versehene Termin entfernt wird, d.h. es gibt keine weiteren Überschneidungen in anderen Plänen.)
* STUNDENPLAN: Manuelles Setzen von Terminen ohne Raumzuordnung, wenn diese deaktiviert ist, korrigiert.
* STUNDENPLAN: Summendaten überarbeitet
* STUNDENPLAN: Korrekturfunktion "Extras|Datei laden und Zeichensatz korrigieren"
* STUNDENPLAN: Sternchen links oben in Listen ruft einen „Spalten bearbeiten“ Fensterersatz auf und erleichtert das Bearbeiten der Spalten
* STUNDENPLAN: Bearbeiten der Spalten klappt nun auch, wenn man in Veranstaltungsliste die Termine aufklickt und dann „Spalten bearbeiten“ das Fenster öffnet oder eben über Sternchen.
* STUNDENPLAN: Bei Blöcken wird Dauer Null bei klassenfremden Elementen nicht mehr angezeigt.
* STUNDENPLAN: In Spalte TERMINE der Veranstaltungsliste werden nun immer alle Lehrer/Räume je Termin aufgelistet.
* STUNDENPLAN: Lehrerart wird im Passende-Lehrer-Fenster angezeigt.
* STUNDENPLAN: Wechsel im Übersichtsplan korrigiert
* STUNDENPLAN: Befehl "Veranstaltung bearbeiten|Teilnehmerplanung" - Schaltflächen "entfernen, hinzufügen" wieder aktiv
* STUNDENPLAN: Stundenplan prüfen - Ergebnisse korrigiert
* STUNDENPLAN: Automatik für Klassen im Kursmodus korrigiert
* VERTRETUNGSPLAN: Im Fehlzeiten Dialog kann man angeben, ob die Fehlzeit bzw. die Änderungen nicht veröffentlicht werden soll
* VERTRETUNGSPLAN: Anzeige vorziehbarere Lehrer kann im OPTIONEN Dialog unter VERTETUNGSPLAN ausgeschaltet werden (z.B. für Grundschulen)
* VERTRETUNGSPLAN: gleichzeitige Lehrer- und Raumfehlzeit: alle Vertretungselemente werden in einer Zeile angezeigt und sind dort zu bearbeiten (Lehreränderung mit fehlendem Raum (den Ersatzraum muss man ggf. nachtragen) 
* VERTRETUNGSPLAN: Klasse fehlt: Vorbelegung der Anrechenstunden von Lehrern in geblockten Klassen 
* VERTRETUNGSPLAN: E-Mail versenden von Änderungsmitteilungen funktioniert wieder.
* VERTRETUNGSPLAN: Anzeige der Anzahl der freizugebenden und eigenen Änderungen korrigiert
* VERTRETUNGSPLAN: Neue Option im Dialog "Optionen|Vertretungsplan": Markieren Sie "Aufsichten bei "Direkte Vertreter" anzeigen", wenn Lehrer mit Aufsicht in der Liste "Direkte Vertreter" in der Ansicht "Vertretungsplan" aufgelistet werden sollen. Andernfalls erscheinen Lerher mit Aufsicht dort nicht.
* VERTRETUNGSPLAN: Vertretungselemente für Aufsichten werden gelb in der Vertretungserstellung markiert
* ÜBERSICHTEN: Neue Ansicht "Lehrerausfall" listet die Lehrerstundensummen und den Ausfall pro Tag über das gesamte Schuljahr. Diese Übersicht kann insbesondere für die PES Statistik (Rheinland-Pfalz) und die Lehrerausfallstatistik in Bremen und Schleswig-Holstein verwendet werden.
* HTML-Export: bei Tagesvertretungen nach Klassen/Lehrern/Stunden ist die Dateibenennung geändert (Wochenenden werden nicht mitgezählt)
* HTML-Export: bei Tagesvertretungen nach Klassen/Lehrern/Stunden ist die Dateibenennung geändert (erste Datei ist mit 001 benannt)

## Version 6.0.162 (26.05.2014)

* EXPLORER: Installationsproblem behoben

## Version 6.0.161 (23.05.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* STUNDENPLAN: Eigenschaften|Vertretungsplan die Option "Aenderungen freigeben" funktioniert jetzt auch für den Betrieb ohne DAVINCI SERVER.
* STUNDENPLAN: Extras|Übersichten zeigen|Jetzt neue Spalten TEAM und GEBÄUDE.
* STUNDENPLAN: Bei Kürzeleingabe in den Stammdaten wird die genaue Schreibweise beachtet
* STUNDENPLAN: Neue Option im Dialog "Optionen" für "Parallele Termine kompakt nebeneinander anordnen" (standardmässig markiert). Kann demarkiert werden, dann verändert sich die Reihenfolge paralleler Termine nicht, wenn die Termindauer verändert wird.
* STUNDENPLAN: Im Dialog "Optionen" neue Option "Immer Uhrzeiten anzeigen" auf Register "Stundenplan" zeigt auf Wunsch immer die Uhrzeit in den Bildschirm-Terminen an.
* STUNDENPLAN: Verplanung zeitgleicher Termine ohne Block korrigiert
* STUNDENPLAN: Verplanung einmaliger Veranstaltungen unterschiedlicher Dauer zeitgleich
* STUNDENPLAN: Doppelstunden-Termine können nun versetzt gesetzt werden (Bsp. Doppelstunde verplant 7.+8. Std., kann nun im Plan per Drag&Drop auf die 8.+9. Std. gesetzt werden)
* STUNDENPLAN: Aufsichten werden am letzten Tag der Gültigkeit des Planes wieder in den Lehrerplänen angezeigt
* STUNDENPLAN: "Extras|Weitere Aktionen|Terminende anpassen" - Anpassen bereits gesetzter Termine an den Zeitrahmen (z.B. um das Terminende von Doppelstunden über eine Pause hinweg anzupassen)
* STUNDENPLAN: Beim manuellen Setzen in der Ansicht STUNDENPLAN konnten evtl. Termine nicht-adaptiv auf Zeitslots gesetzt werden, d.h. ein blauer Balken links im Termin zeigt eine unvollständig abgedeckten Slot an. Dieser Fehler wird durch EXTRAS|PLAN AUFRÄUMEN korrigiert.
* STUNDENPLAN: einmalige eintägige Sperrungen setzen wurde korrigiert
* STUNDENPLAN: "Veranstaltung bearbeiten", Aktualisierung der Wochen erfolgt nun beim Ändern einer Periode
* STUNDENPLAN: nach dem Beenden des Automatiklaufes mit dem x für Schließen des Automatikfensters und dem Setzen einer unverplanten Veranstaltung wird der gesetzte Plan nicht mehr geleert
* STUNDENPLAN: Feherl Soll-Ist-Differenz korrigiert
* STUNDENPLAN:Protokoll - Aktionen rückgängig machen  
* STUNDENPLAN: Mehrfachmarkierung in den Übersichten Zeitkonten, Lehrer Soll-Ist, Fach Soll-Ist, Klassen Soll-Ist  und im Blockauswahlfenster möglich
* VERTRETUNGSPLAN: neue Funktion "Extras|Terminzeiten anpassen"
* VERTRETUNGSPLAN: ein durch Raumänderung freigewordener Raum wird als verfügbarer Raum angezeigt
* VERTRETUNGSPLAN: Raumfehlzeit und anschließender Eintrag einer Lehrerfehlzeit, der von Raumänderung betroffen, wird nun als offenen Vertretung in der Vertretungsliste geführt
* VERTRETUNGSPLAN: Extras|Plandatei aufräumen entfernt Vertretungseinträge der Änderungsliste mit dem Datum 1899
* VERTRETUNGSPLAN: Fehlzeiten werden im Zeitplan wieder angezeigt
* VERTRETUNGSPLAN: Geschwindigkeitsverbesserung im Vertretungsplanbereich für sehr große Dateien
* VERTRETUNGSPLAN: Raumfehlzeit, betroffener Raum wird nicht mehr als frei zur Raumvertretung angeboten
* VERTRETUNGSPLAN: beim Erfassen von Klassenfehlzeiten von Pos. x bis Pos.y (ohne ganztägig-Häkchen), werden die unterrichtenden Kollegen mit zur Begleitung gezeigt
* VERTRETUNGSPLAN: Lehrer-Ist bei "einmaligen" Terminen 
* VERTRETUNGSPLAN: Fehler beim automatischen Erstellen von Änderungen korrigiert. Es wurden in bestimmten Situationen Ändeurngszueilen gedoppelt.
* VERTRETUNGSPLAN: Fehler bei Präsenzfächer beseitigt.
* VERTRETUNGSPLAN: Anzeige eines Lehrers mit Ausfallstunden Klasse als direkter Vertreter
* VERTRETUNGSPLAN: Freistellen ist nun auch mehrfach mit markieren mehrerer Termine/Positionen möglich.
* VERTRETUNGSPLAN: Zusatzunterricht | Entfernen der Teilnehmer per Doppelklick wieder möglich 
* VERTRETUNGSPLAN: beim Eintragen einer Mitteilung wird diese bei allen ausgewählten Planelementen übernommen und angezeigt
* VERTRETUNGSPLAN: Fehlzeitenerfassung von getauschten Veranstaltungen werden mit erfasst
* VERTRETUNGSPLAN: Änderungen die in der Änderungsliste als "nicht veröffentlicht" markiert wurden (rechte Maustaste "Nicht Veröffentlichen") werden nun nicht mehr im Ausdruck, HTML-Export in LOOK angezeigt
* VERTRETUNGSPLAN: doppelter Eintrag für erfasste Fehlzeit der letzten Position (gemäß Zeitrahmen) behoben  

* KURSPLAN: Schüler versetzen, alte Kurs- und Blockzuordnungen der Schüler werden gelöscht
* KURSPLAN: 2 Leistungskurse des selben Faches im gleichen Block, in der Anicht "passende Kurse" wird der jeweils andere Kurs als Alternativkurs angezeigt
* KURSPLAN: Ansicht Kursplan|Blöcke|Matrix korrigiert
* KURSPLAN: Anlegen von neuen Blöcken mit der Bezeichnung von Blöcken, die bereits einmal gelöscht wurden
* KURSPLAN: Ansicht Fachwahlen: mit dem Markieren aller Schüler  und der Auswahl der Funktion Start|"alle Fachwahlen markieren" können Sie alle Fachwahlen der markierte Schüler aktivieren/deaktivieren
* KURSPLAN. Eingabe der Fachwahlen direkt in er Ansicht Kursplan|Schüler
* LOOK: Ansicht Lehrer und Räume jetzt korrekte Anzeige geblockter Veranstaltungen
* LOOK: Farben für Fehlgründe können wie in DAVINCI Vertretungsplan auch in LOOK ausgegeben werden
* KALENDER: löschen von Terminen im Zusatzkalender korrigiert
* KALENDER: Eintrag eines ganztägigen Ereignisses mit Erfassen derFehlzeit korrigiert
* Druck: Klassen-, Lehrer-,Raumpläne mit Wochenauswahl werden korrekt ausgegeben
* Druck: Druckformat Klassenvertretungen Ausgabe des Krüzels in der Überschrift
* Druck: Ausdruck von Kurslisten nach Tutor sortierbar (sortiert wird nach der ersten Spalte mit Ausnahme der Zeilennummer)
* HTML-Export: im Format Klassenvertretungen kann über die Pfeile geblättert werden
* Allgemein: beim Export aus verscheidenen Ansichten wird Excel standarmäßig voreingestellt
* Allgemein: Schuldatentransferformat L5 korrigiert
* Allgemein: Strg+K öffnet Auswahl Klassen wie in Version 5
* Allgemein: Strg+L öffnet Auswahl Lehrer wie in Version 5
* Allgemein: Strg+R öffnet Auswahl Räume wie in Version 5
* Allgemein: manuelles Setzen von zeitgleichen Terminen
* Allgemein: Filterung in der Klassenauswahl bleibt dauerhaft erhalten 
* Allgemein: Im Schlüsselverzeichnis Fachstatus kann für KURSPLAN die Schriftfarbe pro Wert vorbelegt werden.
* Export: Export Statistik Bayern Wiederholungfaktor bei geblockten Veransatltungen korrigiert
* Import SDTF: Beim Importieren des Schuldatentransferformates wird auch das Format L3 berücksichtigt

* Dokumentation: Schuldatentransferformat korrigiert L5

## Version 6.0.157 (01.04.2014)

> Leicht geändertes Standardfarbschema für DAVINCI und DAVINCI LOOK verfügbar: Dazu im Dialogfenster "Optionen|Farben" auf "Standardangaben wiederherstellen" klicken.

* AUFSICHTSPLAN: ein Lehrer der aus einer Aufsicht gelöscht wird, kann dieser wieder zugewiesen werden
* STAMMDATEN: Im Stammdatenfenster können jetzt Leerzeichen vor das Kürzel eingegeben werden, z.B. " 10a", um die alphabetische Sortierung dazu zu bewegen, " 10a" nach "8a" einzusortieren.
* STUNDENPLAN: Im Dialogfenster "Extras|Zeitrahmen|Bearbeiten" neue Option "Termine dürfen nur passgenau in Stunde verplant werden": Automatik verplant 45-Minuten-Stunden ausschließlich in eine 45-Minuten Position aber nicht in eine 50-Minuten Position (nur für Zeitrahmen mit unterschiedlichen Positionsdauern).
* STUNDENPLAN: Im Dialogfenster "Extras|Zeitrahmen|Bearbeiten" neue Option "Termine dürfen nicht über Pause verplant werden": Automatik verplant z.B. keine Doppelstunde über eine 5-Minuten-Pause.
* STUNDENPLAN: Automatik korrigiert.
* KURSPLAN: beim Erstellen der Blöcke wird eine Minimalanzahl vorgeschlagen
* KURSPLAN: Fächer für die Schüler können direkt über die Tastatur eingeben werden
* KURSPLAN: Ausnahme von Blöcken aus der Automatik
* KURSPLAN: Sortierung der Schüler mittels Hoch- und Ab Bewegen korrigiert. Optional kann auch per Drag&Drop sortiert werden.
* KURSPLAN: Löschen von Kursen funktioniert
* KURSPLAN: Mehrfachzuweisung hinsichtlich der Wahl eines Faches korrigiert
* VERTRETUNGSPLAN: nicht vertretende Veranstaltungen (offene) werden im Ausdruck nicht ausgegeben
* Druck: Beim Tausch von Veranstaltungen wird bei beiden Kollegen im Ausdruck korrekt informiert
* Druck: Ausdruck von Schülerplänen können nach Tutor filterbar
* Dokumentation: Schuldatentransferformat korrigiert  K9, R9, L9 

## Version 6.0.156 (25.03.2014)

* VERTRETUNGSPLAN: Fehlzeitenerfassung für mehrere Lehrer eines Blockes korrigiert
* VERTRETUNGSPLAN: Ausfallstunden Klasse wird beim betreffenden Lehrer für die Vertretungsertsellung angezeigt  
* VERTRETUNGSPLAN: Fehlzeitenerfassung aus Sicht alle Wochen | Jahreszahl bezieht sich aud das aktuelle Datum 
* VERTRETUNGSPLAN: Klassenfehlzeit bei geblockten Fächern korrigiert
* VERTRETUNGSPLAN: Darstellung bei Fehlzeiten "Klasse" korrigiert 
* VERTRETUNGSPLAN: Erfassen einer Fehlzeit nur einer Stunde innerhalb einer Doppelstunde
* VERTRETUNGSPLAN: als fehlend erfasster Raum, wird beim Ändern eines Raumes als fehlend angezeigt
* VERTRETUNGSPLAN: Ändern von Fach und Raum bei verschobenen Veranstaltungen
* VERTRETUNGSPLAN: Freistellung einer Einzelstunden werden nur einmal ausgegeben
* VERTRETUNGSPLAN: Ausgabe Stundenausfall in Vertretungsplan|Statistik|Unterrichtsausfall korrigiert 
* VERTRETUNGSPLAN: Anrechenstunden für Klassenfehlzeit korrigiert
* VERTRETUNGSPLAN: freigestellter Lehrer kann nur einmal als direkter Vertreter eingesetzt werden, danach erscheint er als indirekter Vertreter
* VERTRETUNGSPLAN: weist man einem Kurs einer Veranstaltung über "Räume ändern" einen neuen Raum zu, wird der Raum dann für einen weiteren Kurs derselben Veranstaltung als belegt dargestellt
* STUNDENPLAN: Plan|Neu|Neues Schuljahr|Unterrichtsverteilung löschen korrigiert
* STUNDENPLAN: Automatik|Setzautomatik ermöglicht das Umsetzen der Klassen- und Lehrervorgaben
* STUNDENPLAN: Termin-Ende beim Verplanen automatisch an den Zeitrahmen anpassen korrigiert
* STUNDENPLAN: Veranstaltungsdetails|löschen der "Periode"(Kürzel) Entfernen der eingetragenen Kalender-"Wochen
* KURSPLAN: Beim Verschieben von Blöcken werden Konfliktmeldungen für alle betroffenen Schüler erzeugt
* AUFSICHTSPLAN: bereits zugewiesener Aufsichtslehrer kann einr Position nicht mehrfach zugewiesen werden
* LOOK: Plananzeige fehlenden Lehrer und Klassen nicht anzeigen korrigiert
* LOOK: Wechsel in die Anzeige "Lehrer Jetzt" wechselt immer in die aktuelle Kalenderwoche, auch wenn in einer anderen Planansicht eine andere Kalenderwoche geöffnet war
* LOOK: die Spalte "Info" kann für die Vertretungsplanansicht mit eingeblendet werden.
* Drucken: Druckformat Klassenpläne Ausgabe des Raum-Langname, Lehrer-Langname, Fach-Langname korrigiert
* Drucken: Druckformat Tagesvertretung nach Klassen VLehrername wird korrekt ausgegeben
* Drucken: Druckformat Aufsichtspläne Ausgabe des Lehrer-Langname korrigiert
* Drucken: Druckformat Kurslisten Anzeige der (nicht)ausgeblendeten Spalten korrigiert
* Drucken: Ausdruck "nur geänderte Pläne ab" auch für Stundenplanänderung
* Drucken: Klassenpläne lassen sich mit Veranstaltungsliste (Lehrer, Klassen, Räume, Fächer oder Kursliste) unter dem Plan ausgeben
* Drucken: zentrierte Ausrichtung der Termine in den Zeilen möglich
* HTML-Export: Ausgabe der Vertretungsdaten für die Formate Vertretungslehrer und Lehrervertretungen korrigiert.

## Version 6.0.155 (25.02.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* STUNDENPLAN: daVinci 5 Pläne lassen sich wieder öffnen
* STUNDENPLAN: in den Automatikvorgaben ist das Verschieben der Spalten in der Ansicht Lehrer- und Klassenvorgaben wieder fehlerfrei möglich
* STUNDENPLAN: Das Zusatzplanfenster (z.B. rechte Maustaste in STUNDENPLAN Ansicht) kann wieder geöffnet werden. Die Anzeige der Zusatzpläne richtet sich jeweils nach der aktuelle Cursorposition im Plan: Ändert sich die Cursorposition im Plan, so wird die Anzeige der Zusatzpläne aktualisiert. 
* STUNDENPLAN: Problem "unabhängig von Block" bei geblockten Veranstaltungen unterschiedlicher Länge behoben 
* STUNDENPLAN: Ansicht "Plan", Anlegen "einmaliger" Veranstaltungen (hier Wiederholung: einmalig)im Planfenster korrigiert.
* KURSPLAN: Problem beim "Schüler versetzen" behoben. 
* KURSPLAN: Löschen der Kursnummer im Bereich "Kurse" wieder möglich 
* KURSPLAN: Übersichten|Kursteilnehmer Export von Bereichsmarkierungen möglich 
* KURSPLAN: Neue Eingabemaske für das Anlegen eines neuen Kurselementes
* KURSPLAN: Fachstatus kann jetzt im Bereich "Kurse" in der neuen Spalte "Fachstatus" eingegeben werden.
* KURSPLAN: Eingebrachte Fächer in den HJ (E1, E2, Q1-Q4) werden nun im Bereich "Fachwahlen" mit einer EINS (1) angezeigt, auch wenn keine Stundenzahl eingetragen wurde, also 1=eingebracht, leer=nicht eingebracht.
* KURSPLAN: Fachwahlen "markieren" wieder aktiv, wenn Spalten E1, E2, Q1-Q4 ausgeblendet sind
* KURSPLAN: Lehrerzuweisung funktioniert
* KURSPLAN: Spalten ein- und ausblenden in der Fachwahl funktioniert
* KURSPLAN: Neue Option im Bereich "Fachwahlen" ermöglicht es, alle Fachwahlen als "GEWÄHLT" zu setzen
* VERTRETUNGSPLAN: Darstellung bei Fehlzeiten über Doppelstunden korrigiert
* VERTRETUNGSPLAN: doppelte Fehlzeiten korrigiert
* VERTRETUNGSPLAN: Druckvorschau Lehrervertretungen und Vertretungslehrerliste korrigiert
* VERTRETUNGSPLAN: doppelte Anzeige beim Tausch von Terminen im Lehrerplan korrigiert 
* VERTRETUNGSPLAN: Raumänderung wird nun korrekt im Plan angezeigt
* KALENDER: neues Ereignis anlegen funktioniert wieder
* KALENDER: Neue Kalenderdateien für das Schuljahr 2014/15 verfügbar
* LOOK: Ansicht STUNDENPLAN, Bemerkungstext bei Veranstaltungen wird angezeigt.
* INFOSERVER: Links, die auf die daVinciApp verwiesen, wurden korrigiert.
* EXPLORER: Doppelter Aufruf für "Stundentafeln bearbeiten" in den Richtlinien korrigiert
* Drucken: Aufruf aller Aufsichtsbereiche wieder möglich
* Drucken: "Heute voreinstellen" kann aktiviert und deaktiviert werden
* Drucken: Langname in der Überschrift wird nun wenn voreingestellt korrekt angezeigt 
* Export: XML-Export korrigiert
* Druckformat: In der "Vertretungslehrerliste" werden ganztägig fehlende Klassen nicht mehr pro Position aufgelistet, sondern erscheinen nur in Aufzählung am Listenanfang
* Druckformat: In den Einstellungen für Druckformate können auf der Karte "Termine" Terminelemente auch zentriert angeordnet werden.
* Druckformat: In der "Vertretungslehrerliste" werden ganztägig fehlende Klassen nicht mehr pro Position aufgelistet, sondern erscheinen nur in Aufzählung am Listenanfang  
* Druckformat: Im "Einzelplan Klassen schmal 3 Zeilig" ist die Funktion "Jeden Plan auf neuer Seite drucken" korrigiert
* Druckformat: Lehrergesamtpläne werden korrekt bei Auswahl bestimmter Wochentage ausgegeben. Bitte beachten Sie, dass die Auswahl der Ausgabetage nur innerhalb einer Woche (Mo-So) möglich ist. 
* Druckformat: Beim Ausdruck von Schülerplänen kann nach Jahrgangsstufe gefiltert werden.
* Statistik Bayern ASV Datenaustausch: Unter "Plan|Importieren und Exportieren" befinden sich nun die Punkte "Bayern ASV importieren" und "Statistikdaten exportieren |Statistk Bayern (ASV) exportieren"
* SAR-FW-APO-2007.js korrigiert

## Version 6.0.154 (31.01.2014)

* VERTRETUNGSPLAN: Fehler in der Vertretungserstellung beim Erstellen einer Raumfehlzeit behoben. Bereits angelegte überzählige Vertretungselemente bitte in der Änderungsliste löschen.

## Version 6.0.153 (27.01.2014)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* STUNDENPLAN: Fehler beim Aufruf des Fensters zur Eingabe von Sperrungen und Kernzeiten beseitigt.
* STUNDENPLAN: Fehler beim "Plandatei aufräumen" für Sperrungen behoben.
* STUNDENPLAN: Problem beim Speichern der Einstellungen unter Plan|Eigenschaften|Statistik behoben
* VERTRETUNGSPLAN: Fehlerkorrektur: Bei Doppelstunden wurden fälschlicherweise mehrfache Vertretungseinträge erstellt. Für neu erstellte Fehlzeiten behoben.
* VERTRETUNGSPLAN: Gesperrte Räume werden nicht mehr zur Vertretung angeboten.
* LOOK: Ganztägige Klassenfehlzeiten werden nicht mehr in der Liste sondern nur noch als Hinweis unten aufgeführt.
* LOOK: Ansicht VERTRETUNGEN neue Spalte INFO einblendbar.
* LOOK: Problem beim Aufruf mit der Standardansicht "Interaktives Vollbild für Touchscreens" behoben

## Version 6.0.152 (21.01.2014)

* HINWEIS: Nach dem Installieren des Serviceupdates müssen Sie in DAVINCI und DAVINCI LOOK einmalig Ihr Land bzw. Bundesland einstellen, damit ortsspezifische Funktionen verfügbar werden. 
* Export: Beim D6-Datensatz werden auch Veranstaltungen mit der Dauer Null berücksichtigt
* STUNDENPLAN: korrekte Anzeige von Veranstaltungen auf Schienen
* STUNDENPLAN: unterschiedliche Sperrungen auf Zeitschienen ist möglich
* STUNDENPLAN: in der Listenansicht werden die Kalenderwochen ausgegeben
* VERTRETUNGSPLAN: Verlängern der Termindauer bei Aufsichten möglich, um Aufsichten mit unterschiedlicher Dauer zu erstellen, die zur gleichen Zeit beginnen
* VERTRETUNGSPLAN: Beim Öffnen der "Vertretungen" Ansicht werden jetzt automatisch entsprechende neue Änderungen aufgrund von Planänderungen erzeugt
* VERTRETUNGSPLAN: Fehler beim Ausfall von Aufsichtsvertretungen korrigiert
* VERTRETUNGSPLAN: Klassenfehlzeit als Teil einer Doppelstunde wird korrekt erfasst
* VERTRETUNGSPLAN: Klassenfehlzeit nur Kurs korrigiert
* VERTRETUNGSPLAN: Erfassen einer Raumfehlzeit und nachträglich einer Lehrerfehlzeit an der selben Position, fehlender Lehrer wird nun als offene Vertretung angezeigt
* VERTRETUNGSPLAN: Raumänderung wird korrekt im Lehrerplan ausgegeben
* VERTRETUNGSPLAN: In der Liste der Anrechnungen werden auch Lehrerfehlzeit mit "0" Anrechenstunden" ausgegeben
* KURSPLAN: Kurse können beim Blocken von der Automatik ausgenommen werden
* KURSPLAN: Ansicht "Kurse" - hier werden nun auch "passende Blöcke" angezeigt
* KURSPLAN: "Block-Eigenschaften ändern" wieder möglich
* KURSPLAN: Schüler versetzen in die nächste Klasse
* KURSPLAN: "Fachwahlen erzeugen|Aus Schülerkursen" ist gedacht für den seltenen Fall, dass man Schüler zu Kursen zugeordnet hat. Man kann darüber aus den Schülerkursen die Kurswahl erzeugen. Man kann Schüler außerhalb des KURSPLANS mit Hilfe des Veranstaltungendialogs als TEILNEHMER HINZUFÜGEN, völlig unabhängig vom KURSPLAN Schüler wie auch andere Personen (Lehrer) einem Kurs zuordnen. Man kann so im Nachhinein die Kurswaheln erzeugen.
* LOOK: Fehler bei der Ansicht des Vertretungsplanes behoben
* Druckformat: Klassenpläne für eine bestimmte Woche korrigiert
* Druckformat: Tagesvertretung nach Stunden Ausgabe der Lehrerfehlzeit korrigiert
* Druckformat: Gesamtpläne Klassen und Einzelpläne Klassen; Zeilentrennlinien werden korrekt dargestellt
* Druckformat: Gesamtplan Lehrer, bei Auswahl von "Tage" von/bis im Layout wird der Plan korrekt ausgegeben
* Druckformat: Klassenpläne; korrekte Ausgabe der Anfangs- und Endzeit aus Layout|Titel vertikal links|Format
* ENTERPRISE: Problem beim "Speichern unter" aus dem Serverbetrieb behoben
* INFOSERVER: Anzeige der fehlenden Lehrer und Klassen oberhalb der Pläne korrigiert
* HTML-Export: Anzeige der fehlenden Lehrer und Klassen oberhalb der Pläne korrigiert 

## Version 6.0.151 (28.11.2013)

* Neuer Befehl: "Extras | Weitere Aktionen | Personennummern erzeugen" übernimmt die Magellan-ID als Personennummer(z.B. für die Infoserver-Schülerplananzeige).
* HTML-Export: "sandbox" Ordner und Bilddateinamen werden kleingeschrieben erzeugt.
* HTML-Export und Drucken: Bei Lehrern und Schülern kann die "ID" bzw. die "GUID" im Namen ausgegeben werden, wenn dies im Druckformate bzw. HTML-Exporteformate Dialogfenster angegegeben wird.
* Vertretungsplan: Fehler im Vertretungsplan beseitigt, der zu einer Datei führen konnte, die nicht geladen werden konnte.
* Vertretungsplan: Fehler bei der Anzeige von Vertretungen (Doppelanzeige) beseitigt.
* Vertretungsplan: Fehlzeiten über Weggezogene Elemente erzeugen keine Vertretungen.
* Vertretungsplan: Fällt aufgrund einer Raumänderung Unterricht aus, steht der freiwerdende Lehrer für VErtretungen zur Verfügung. Es muss keine Freistellung eingegeben werden.
* Vertretungsplan: Fehlzeiten über Einzelstunden einer Doppelstunde könne nun wieder korrekt erfasst werden.
* Vertretungsplan: Beim Eingeben von Freistellungen kann mit einer neuen Option im Dialogfenster gewählt werden, ob der Unterricht vertreten werden soll oder nicht, z.B. in Blockungen.
* Druckformat: für fehlende Klassen wird das Kürzel der Klassen statt der Bezeichnung ausgegeben

## Version 6.0.150 (20.11.2013)

* Modifiziertes Farbschema: Im Optionen-Dialogfenster bei "Farben" auf "Standardvorgabe wiederherstellen" klicken: Die aktuelle Woche wird in Stundenplänen farblich durch einen blauen Titel hervorgehoben.
* HTML-Export: Beim HTML-Export werden anstatt der Lehrer/Klassen/Raumkürzel eine Zahlen als Dateinamenbestandteile exportiert. Dadurch treten keine Probleme mehr mit Sonderzeichen/Umlauten auf.
* HTML-Export: Formatvorlage davinci.content.minimal.html korrigiert
* HTML-Export: Aufruf von Kürzel mit Umlauten, Schrägstrichen oder &-Zeichen korrigiert
* Infoserver:  Aufruf von Kürzel mit Umlauten, Schrägstrichen oder &-Zeichen korrigiert
* Druckformate: Vorschau der Wochenpläne korrigiert
* Statistik-Export: für BBS Bayern WinLD korrigiert
* Vertretungsplan: Erfassen von Fehltzeiten über mehrere Tage korrigiert
* Vertretungsplan: Auswahlfenster Wochen unter Vertretungen ist wieder aktiv
* Stundenplan: in der Veranstaltungsliste kann in der Terminliste einer Veranstaltung mit der ENTF-Taste Tag und Uhrzeit entfernt werden
* Stundenplan: unter Stammdaten|Gebäude kann ein neues Gebäude mit Wegezeit erfasst werden
* Stundenplan: bei geblockten Unterricht werden die Stunden nur noch einmal angerechnet
* Stundenplan: korrekte Anzeige der Tauschoptionen
* Look: Optionen|Plananzeige gibt es die Möglichkeit Registerkarten unten im Plan ausblenden zu lassen

## Version 6.0.149 (07.11.2013)

* Infoserver: die Auswahlschaltfläche (Lupe) im Klassenplan funktioniert korrekt
* Infoserver: die für die Pläne gewählten Wochentage werden korrekt angezeigt
* Kalender: im Kalender eingetragene Ereignisse, die Doppelstunden im Stundenplan berühren, werden korrekt dargestellt
* Kalender: Pfad zu den Kalenderdateien in die System-Information eingebaut
* Kalender: diverse Probleme beim Anlegen von Ereignissen behoben
* Kalender: wenn eigene Kalenderdateien (*.ics, *.ical) importiert werden, können mit "Plan aufräumen" eventuell fehlende Enddaten vorbesetzt werden.
* Kalender: ein neues Ereignis kann über die grüne Plusschaltfläche angelegt werden
* Kalender: Löschen aller Ereignisse korrigiert
* Stundenplan: korrekte Angabe des Ist/W in der Veranstaltungsliste wenn Perioden über die Angabe der Woche im Dialog "Veranstaltung bearbeiten" hinterlegt werden"
* Stundenplan: Anzeigefehler beim Wechsel vom Stunden- zum Aufsichtsplan behoben
* Stundenplan: Aktualisierung der Summenanzeige beim Wechel der Klassen oder Lehrer korrigiert
* Stundenplan: Anzeige Summen LehrerIst/Wochernschnitt bei tagesbezogener Berechnung korrigiert
* Stundenplan: Ansicht "Plan", Wechsel in einen anderen Plan über Pfeile links oben im Planfenster korrigiert 
* Stundenplan|Unterrichtsmatrix: Dauerangabe in der Unterrichtsmatrix korrigiert
* Stundenplan|Jahresverteilung: im Spaltenkopf werden nun die Kalenderwoche und nicht mehr die absolute Woche angezeigt.
* Stundenplan|Zusatzfenster "Zeitkonflikte": Konflikte, die man durch manuelles Tauschen im Stundenplan erzeugt hat, werden nun richtig im Zeitkonfliktefenster angezeigt
* Stundenplan: Korrespondierende Pläne aktualisieren beim ersten Klick auf ein Terminelement
* Stundenplan: beim Hinzufügen eines weiteren (korrespondierenden) Plans bleiben die zuvor ausgewählten Pläne(z.b. Klassen-, Lehrer- oder Raumplan) erhalten
* Stundenplan: unter daVinci-Optionen|Einstellungen|Veranstaltungsliste|Wiederholung können Sie mit "einmalig" oder "periodisch" den Wert für das Feld "Wiederholung" einer neu angelegten Veranstaltung vorbesetzen
* Kursplan: doppelte Blöcke aus der Übernhame von daV 5 Dateien über "Plan Aufräumen" korrigiert
* Kursplan: Doppelungen in Kursliste bei Kursen in unterschiedlichen Blöcken korrigiert
* Kursplan: Kursauswahl beim Drucken von Kurslisten ist vertikal angeordnet
* Vertretungsplan: Raumfehlzeiten werden beim Anlegen von Zusatzunterricht berücksichtigt
* Vertretungsplan: bei indirekten Vertretern (die gesperrt sind) können bei Vertretung auch Anrechenstunden vergeben werden
* Vertretungsplan: Zugriffsverletztung im Bereich "Vertretungen" korrigiert
* Vertretungsplan: Zugriffsverletzung beim Erzeugen einer Fehlstelle behoben
* Vertretungsplan: bei den direkten Vertretern wird bei vorziehbaren Stunden wieder die Positionsnummer mit angezeigt
* Vertretungsplan: entfällt eine Stunde einer Doppelstunde für eine Klasse, wird unter Vertretung|Statistik|Unterrichtsausfall der korrekte Wert gezeigt.
* Vertretungsplan: Lehrerfehlzeiten über mehrere Tage ("ganztägig" angehakt) werden nun korrekt in der Vertretungsplanung angezeigt
* Vertretungsplan: unter Änderungen wird beim Klick auf einen Spaltenkopf sortiert statt gruppiert
* Vertretungsplan: Vorziehen von Stunden (nur eine Stunde einer Doppelstunde) Fehler korrigiert  
* Vertretungsplan: Vertretungsanzeige bei geblockten Veranstaltung korrigiert
* Vertretungsplan: die Spaltenbreite der Änderungsliste kann angepasst werden
* Vertretungsplan: beim Klick auf die Spaltenköpfe der Änderungsliste wird die nach den Spalteninhalten sortiert, beim Hochziehen des Spaltenkopfes wird nach den Spalteninhalten gruppiert
* Vertretungsplan: offene Raumvertretungen bei fehlenden Klassen korrigiert
* Automatik: Auswahl der Blöcke für einen Automatiklauf möglich 
* Automatik: Fachraumzuweisung korrigiert
* Druckausgabe: ganztägige Mitteilungen werden am korrekten Termin im Ausdruck ausgegeben
* Druckausgabe: die im Design unter Layout|Positionen angebenen Werte werden korrekt berücksichtigt
* Druckausgabe: im Druckformat Gesamtplan Räume werden die Sperrungen mit ausgegeben
* Druckausgabe: Drucken Klassenpläne werden seitenweise ausgegegeben, wenn der Haken gesetzt ist
* Druckausgabe: Ausgabe von Trennlinien im Plan funktioniert
* Druckausgabe: neue Einstellung "Termine auf Zellen verteilen" auf der Registerkarte "Termine" beim Ausdruck erlaubt die alte Darstellung der zeitgleichen Termine untereinander, wenn "Einzeltermine, zeitgleiche untereinander" eingestellt wird.
* Druckausgabe: Neue Option im Druckformat für Klassen-, Lehrer- und Raumpläne auf der Registerkarte "weitere Listen" ermöglicht eine "Fach/Lehrer-Legende" unter dem Plan
* Druckausgabe: Klassenpläne/Raumpläne, bei Terminen ist die Auswahl Lehrer Format "Langname" korrigiert
* Druckausgabe: Veranstaltungsliste Lehrer, es werden unter der Liste die Summe Lehrer-Soll und Lehrer-Ist ausgegeben
* daVinci Server: Korrektur eines Benutzerrechtes wenn das Bearbeiten der Stammdaten ausgeschlossen ist, können nun auch in der Veranstaltungsliste keine neuen Fächer und Lehrer mehr angelegt werden
* HTML Export: beim Export der Vertretungspläne ist die Einstellung im HTML-Format unter Register "Dateien"|"Export-Ordner Inhalt zuvor löschen" wieder einstellbar
* Aufsichtplan: Lehrerfarben werden korrekt angezeigt
* Aufsichtsplan: Korrektur beim Zuweisen der Aufsichtsbereiche
* daVinci-Optionen: neue Einstellung unter „Extras|Optionen|Einstellungen|Teamfilter“, ob die Fächer in der Veranstaltungsliste nach Teamzugehörigkeit gefiltert werden sollen. Unter „Stammdaten|Teams“ können Sie in der Spalte „Fächer“ die Fächer eines Teams definieren. 
* daVinci-Optionen: optional kann die Ansicht im Auswahlfenster auf mehrspaltig gestellt werden
* daVinci-Eigenschaften: Neue Option für Stunden unterschiedlicher Zeitdauer: "Minuten pro Einheit" laut Zeitrahmen anstatt realer Dauer laut Plan rechnen
* Stammdaten: eingegebene Schulzweige werden gespeichert 
* Statistik Rheinland-Pfalz (auch edoo.sys) exportieren: Für den Export nach edoo.sys wurde die Exportdatei um den T1-Datensatz des Schuldatentransferformats ergänzt
* Neue Möglichkeiten der daVinci Automation, um über Kommandozeilenparameter eine Automation des Statistikexports zu ermöglichen. Vergleichen Sie dazu das akualisierte 
  daVinci 6 Stundenplan Benutzerhandbuch in Kapitel "17.7 daVinci-Automation", welches mit dem Serviceupdate installiert wird bzw. auf unseren Internetseiten unter http://www.stueber.de/index.php/de/service/dokumente.html verfügbar ist.

## Version 6.0.147 (25.10.2013)

* Fehler beim Erstellen von Fehlzeiten mit Lehrern in mehreren Klassen gleichzeitig behoben.
* Fehler in der Statistik Export Rheinland-Pfalz korrigiert: Soll-Stundenzuordnung bei Kursen mit mehreren Lehrern korrigiert.
* Fehler beim Vorziehen von Stunden korrigiert: Es wurden nicht alle vorziehbaren Vertreter aufgelistet.
* Fehler bei Aufsichtsvertretungen behoben.
* XML-Export: XML-Tag <Supervision* um weitere Daten ergänzt in neuer Liste <Supervisions>. 

## Version 6.0.146 (23.10.2013)

> WICHTIG: Wegen eines Fehler in Druckformaten des Typs "Raum Gesamtplan" wurde das Format der Datei "daVinci.pfm" korrigiert. 

Beim Starten von daVinci erhalten Sie daher Fehlermeldungen. 
Bitte löschen Sie VOR dem Installieren dieses Updates in Ihrer Druckformate-Datei alle Druckformate dieses Typs und importieren Sie diese nach dem Update über die Schaltfläche "Druckformate|Aktualisieren" erneut. 
Wenn Sie das Update bereis ausgeführt haben sollten, öffnen Sie die Datei "daVinci.pfm" in einem Texteditor und löschen Sie im Text das HTML-Tag ```<item class="RaumGesamtplan"*``` und zwar alles zwischen den Anfangstag ```<item class="RaumGesamtplan"*``` und dem dazugehörigen Ende-Tag ```</item>```. 
Bitte wenden Sie sich mit dieser Datei an unser Support, falls es Probleme geben sollte.

! Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* Neue Druckformate "Wochenplan Klassen" und "Wochenplan Räume". Klicken Sie dazu im Druckformate-Fenster auf "Druckformate|Aktualisieren".
* Druckformat Gesamtplan Räume bezüglich der Ausgabe Tage, Stunden korrigiert
* Vertretungsplan: Fehler bei der Vertretungserstellung mit Lehrern aus unterschiedlichen Zeitrahmen behoben
* Vertretungsplan: Fehler beim Vorziehen aus Doppelstunden korrigiert
* Vertretungsplan: Druckausgabe des VFaches in der Spalte VLehrer korrigiert. Einmal auf Eigenschaften|Bezeichnungen "Bezeichnugen zurücksetzen" gehen.
* daVinci Look: Ausblenden der Uhr
* Stundenplan: korrekte Ausgabe des Ist/W wenn Wochen über Veranstaltung bearbeiten|Zeitvorgaben|Wochen zugeweisen werden
* Anzeige des Lehrer Ist "Wochenschnitt" bei tagesbezogener Berechnung im Fenster Summen korrigiert
* Ausgabe der Plan-Ist aus Lehrer Sicht im Fenster Summen korrigiert
* Ausgabe der Lehrer-Ist Stunden im Zeitkonto korrigiert bei wochen- und faktorbezogener Berechnung, entspricht nun dem Wert aus dem Fenster Summen
* Import|daVinci Änderungen für Planwechsel importiert korrigiert
* RLP-Statistik: Solländerungsstunden der Klassenwerden korrekt exportiert
* WinLD Export: Fehler bei Stundenzahlen und Wochenfaktoren korrigiert 
* WinLD Export: Fehler beim Wiederholungsfaktor korrigiert
* HTML Export: Option "Export-Ordner Inhalt zuvor löschen" wird jetzt korrekt ausgeführt.
* eingetragene Bemerkungen werden in den Dateieigenschaften gespeichert
* Fehler beim Import von Daten aus Version 5 behoben.
* Neue Option "Heute/Morgen anstatt Tag" für HTML-Exportformate und Druckformate der Tagesvertretungslisten.
* HTML-Exportformat: neue Einstellung "Termine auf Zellen verteilen" auf der Registerkarte "Termine" bei HTML-Exportformaten erlaubt die alte Darstellung der zeitgleichen Termine untereinander, wenn "Einzeltermine, zeitgleiche untereinander" eingestellt wird.
* Bei indirekten Vertretern kann man im entsprechenden Dialogfenster optional Anrechenstunden eingeben.
* Die Spalte "Team" in der Ansicht "Stammdaten|Fächer" entfällt zugunsten der neuen Spalte "Fächer" in der Ansicht "Stammdaten|Teams", mit der man Fächer Teams zuordnen kann. Wenn die Option "Optionen|Einstellungen|Fächer in Veranstaltungsliste nach Teamzughörigkeit filtern" aktiviert ist, dann werden nur die Fächer des Teams (der Klasse) angezeigt.
* In der Ansicht "Stundenplan|Jahresverteilung" kann die Anzeige mit "Listenansicht|Nur statistkrelevante Summen" auf nur statistikrelevante Summen eingeschränkt werden, d.h. die als "Nicht statistikrelevant" markierten Fächer werden nicht gezählt.
* Neue Spalte "Wochenanzahl" in der Veranstaltungsliste bei Veranstaltungen und Terminen.
* Neue Spalte "Stammdatenfenster|Perioden|Wochenanzahl", es wird die Anzahl der markierten Wochen einer Periode ausgegeben
* Neue Spalte "Stammdaten|Räume|Zeitrahmen".
* Neue "Option|Einstellungen": "Kursnummer beim Duplizieren eines Kurse erhöhen".
* Neue Vorbesetzung für neu eingefügte Veranstaltungen unter "Option|Einstellungen|Wiederholung"
* Im "Plan|Auswahl" Fenster kann man über das Aufklappmenü neben "OK" mit "Mehrspaltige Liste" die ältere mehrspaltige Ansicht einstellen.
* Blockauswahlfenster ist nun exportierbar (*.xml, *.txt, *.html, *.xls)
* Modifzierte HTML-Vorlage "davinci.showtime.subst.local.html" und "davinci.showtime.subst.main.html": Es wird automatisch die maximale Zeilenanzahl pro Seite und die Zeit bis zum Weiterschalten aus der HTML-Exportvorlage übernommen.
* Jahresverteilung: IstJ in der Jahresverteilung korrigiert
* Ausdruck "Lehrerplan" mit Zeitkonto korrigiert

## Version 6.0.142 (09.10.2013)

* HTML Export: Export für Schülerpläne, alle Schülerpläne werden exportiert
* da Vinci Look: Infozeile wird im Serverbetrieb bei Änderungen neu geladen
* daVinci Export: D6 Datensatz Soll der Klasse korrigiert, wenn ein Fach einer Klasse von verschiedenen Lehrern unterrichtet wird, erhält der erste Lehrer die Sollstunden der Klasse aus der Stundentafel
* daVinci Export: NRW BBS Statistik bei geblocktem Unterricht (ein Fach mit 2 Lehrern) wird das Stunden-Ist korrekt exportiert
* Soll-Stunden in der Veranstaltungsliste werden korrekt ausgegeben laut Stundentafel
* daVinci Vertretungsplan: Löschen von Anrechenstunden (gesamte Liste) möglich
* daVinci Explorer: Richtlinie "Zugriff auf daVinci Explorer" implementiert
* Neue Option "Plananzeige|Touch Screen/Maus Gesten zulassen" für "Rechts/links wischen" (Weiterschalten der Woche) und "Oben/unten wischen" (Weiterschalten des Plans) für Touch Screens.
* Überarbeitete Kinect Gestensteuerung

## Version 6.0.139 (26.09.2013)

> Für Nutzer des daVinci InfoServers: Bitte beachten Sie die daVinci.InfoServer.Liesmich.txt!

! HTML Export: Formatvorlagen wurden vollständig überarbeitet. Die CSS-Datei wird ausschließlich in der HTML-Vorlage angegeben. Bitte passen Sie ggf. selbst erstellte HTML/CSS-Vorlagen entsprechend an!

* HTML Export: Alphabetisch bzw. nach Klassenstufe und Name (nur Klassen) gruppierter Index per Option in der Vorlage einstellbar.
* HTML Export: Neues Format "Kalender".
* HTML Export: Parallele Stunden werden wie in der Bildschirmanzeige parallel ausgegeben.
* HTML Export: Vertretungspläne Ausgabe der Spalte Art und Info
* HTML Export: Klassenpläne mit geblockten Veranstaltung, die nur teilweise zeitgleich stattfinden
* HTML Export: Exportformat Schülerpläne bearbeitbar
* Pfad für die Exportdatei zur Statistikerstellung bleibt auch nach dem Schließen der Datei gespeichert
* Lehrer-Ist Klasse bei geblocktem Unterricht wird nun korrekt ausgegeben
* Arbeitszeitkonten Lehrer | Ansicht aus Stammdaten nun übereinstimmend mit Druckvorschau
* Stundenplan|Zusatzfenster "Passende Lehrer", die Filterung "Nur Lehrer des Teams" zeigt nun nur Lehrer des Teams an 
* Summen Ansicht Lehrerplan: Lehrer-Ist berücksichtigt parallelen Unterricht im Block (ein Lehrer unterrichtet in zwei Klassen zeitgleich)
* daVinci Export: Bei geblockten Veranstaltungen mit gleichem Lehrer werden Ist-Stunden korrekt exportiert
* fehlerhafte Anzeige beim Öffnen des Planvorbereitungsassistenten aus einer Plandatei heraus behoben
* daVinci Export: Datensatz D2 D2 enthält das Klassen-Ist der Woche
* Stundenplan im Servermodus: Problem beim Setzen von neu angelegten Veranstaltungen behoben
* daVinci Export: der Aufruf zum Übertrag nach Magellan konnte für einige Plandateien nicht gestartet werden
* Druck: Ausdruck von Vertretungen korrigiert
* Druck: unter Design|Layout eingestellte Positionen werden korrekt berücksichtigt
* Problem beim Autospeichern im Netzbetrieb ohne Enterprise-Modul behoben
* daVinci Look: Aktualisierung der Anzeige "Räume jetzt"(zwei Listen) korrigiert 
* daVinci Look: in den Systeminformationen wird korrekt auf die daVinciLook.path verwiesen
* daVinci Look: Anzeige der Ausichtbereiche korrigiert
* Im Vertretungsplanbereich "Fehlzeiten" Ansicht "Liste und Zeitplan" können nun im Listenkopf Spalten ein- und ausgeblendet werden
* Stundenplan: Problem bei der Berechnung Ist/W bei periodischen Unterricht behoben

## Version 6.0.135 (06.09.2013)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* Zusammenführen von Dateien über Schuldatentransferformat, Lehrer-Arbeitszeitkonten werden korrekt dargestellt
* Mehrfachzuweisung von Fächern in daVinci Kursplan 
* Ausgabe der Summe Lehrer Ist in Klasse bei geblockten Veranstaltungen
* Veranstaltungen im Lehrerplan ohne Klassen wieder speicherbar
* Schaltfläche frei beweglich wieder aktiv
* Anlegen neuer Veranstaltungen mit mehreren Klassen im Lehrerplan wieder möglich
* Ausgabe "Raum-Langname" im Druck funktioniert
* Funktion "Räume nicht berücksichtigen"  beim Setzen von Veranstaltungen funktioniert
* Summe Lehrer Ist in Klasse korrigiert
* Ausdruck von Perioden (Kalenderwochen) funktioniert wieder
* Aufruf Woche aktualisieren im Bereich Stammdaten|Perioden|Bearbeiten verfügbar
* Ansicht "Kursplan": Neues Dialogfenster "Mehrfachzuweisung"
* Neues Druckformat "Kursliste" für den Ausdruck von Kurslisten, siehe Beispielvorlage (klicken Sie auf "Aktualisieren" im Dialogfenster "Druckformate").
* Neues Zeitschienen-Register "#" unten im Plan zeigt zusammenfassend die Termine aus allen Zeitschienen ein.
* Anzeige von Zeitschienen in der Ansicht "Stundenplan" korrigiert.
* korrekte Ausgabe des Lehrer-Ist bei veränderter Zeitdauer in den "Planeigenschaften|Statistik"
! Schnellere Anzeige bei Plänen mit Zeitschienen.
* In einigen Plänen wurde beim "Plan aufräumen" die Meldung "Ungültige Typumwandlung" ausgegeben
* Druckausgabe für Klassenpläne (Unterricht in Schienen)korrigiert 
* bei wochenbezogener Berechnung wird das Lehrer-Ist wieder korrekt ausgegeben
* In der Ansicht Übersichten|Kursteilnehmer werden alle Kursteilnehmer gezeigt
* daVinci LOOK: Gebäudefilter wird in der Ansicht "Klassen/Räume jetzt" korrekt beachtet.
* daVinci Kursplan: Mehrfachzuweisung bei Kursen möglich
* daVinci INFOSERVER: Beim Export werden die Kalenderwochen zur Auswahl zum Beispiel der Blockwochen mit übergeben
* daVinci INFOSERVER: unter Systemsteuerung|daVinci Server (32 Bit|Unterkarte "Infoserver" wird der Pfad zur daVinci.hfm gezeigt, auf die der Infoserver für die Darstellung der Pläne zugreift. Bitte legen Sie an dieser Stelle Ihre bearbeitete daVinci.hfm ab.
! XML-Export von Terminen: Die XML-Tags "Teacher" und "Room" sind in "Teachers" und "Rooms" geändert worden. Zusätzlich sind die neuen Tags "SClasses", "STeachers" und "SRooms" ergänzt worden.

## Version 6.0.132 (16.08.2013)

* Fehlerkorrektur in daVinci Drucken: Druckformat Layout|Positionen (mindestens bis/ höchstens bis)
* Fehlerkorrektur in daVinci: Die Angabe "Integrierte Klasse" wird nun beim Drucken, der HTML-Ausgabe und der Automatik korrekt beachtet.
* Falls die Lehrerfarben als Terminhintergrund angezeigt werden, wird die Hintergrundfarbe des Fachs angezeigt, falls für den Lehrer keine Farbe vergeben wurde.
* Bei Aufsichtsplänen kann man mit "Neue Aufsicht" wieder Aufsichten mit einem Klick anlegen, die Schlatfläche ist nicht mehr grau hinterlegt bei Positionen ohne Eintrag.
* Fehlerkorrektur im Fachwahlskript Berlin "BER-FW-APO-2011.js"
* Veranstaltungsliste|Veranstaltung bearbeiten: werden über "Wochen bearbeiten" die Wochen einer zugewiesenen Periode bearbeitet, entfällt die Zuweisung zur Periode, die Periodenwochen und die bearbeiteten Wochenwerte werden für die Veranstaltung übernommen. Unter Stammdaten|Periode wird nichts verändert.
* Ausdruck von Vertretungsdaten pro Team korrigiert
* Die Anzeige der Lehrerspringstunden unter Extras|Planungsstand wurde korrigiert
* Beim Autospeichern in gewählten Abständen wird bei bereits gespeicherten Dateien nicht mehr das "Speichern unter"-Fenster aufgerufen
* In der Terminliste ergänzte Räume werden in der Veranstaltungsliste|Spalte Termin hinter dem dazugehörigen Termin in eckigen Klammern gezeigt
* Im Kursplan erscheinen in der Übersicht der Kursteilnehmer aus duplizierten Kursen nur einfach
* Fehlerkorrektur im Aufsichtsplan: Problem beim Ändern der Fensterbreite (Planfenster) gelöst
* Problem beim Plan|Importieren und Exportieren|daVinci XML-Daten exportieren ist gelöst
* Übersichten|Kursteilnehmer: neue Spalte "Lehrer" 
* Übersichten|Kursteilnehmer: Man kann per Filter (Spaltenkopf "Kurs") genau einen Kurs anzeigen und diesen drucken
* Fehlerkorrektur im Kursplan: Nachträgliche Kurszuweisung bei einzelne Schülern per Automatik gelöst
* Fehlerkorrektur im Bereich "Übersichten|Kursteilnehmer": Wechsel in eine andere Klasse über "Auswahl" (Listenkopf) nun möglich
* Setzen aus einem Raumplan gelöst
* daVinci INFOSERVER: Verweise mit Umlauten werden korrekt verarbeitet
! Modifiziertes XML-Ausgabeformat für Termine 

## Version 6.0.130 (07.08.2013)

* Fehlerkorrektur in daVinci Look: Schaltfläche "Suchen" im Touchscreen Modus wieder sichtbar.
* Fehlerkorrektur in daVinci Stundenplan: beim Setzen von Veranstaltungen ohne Raum manuell oder per Automatik wird auch kein Raum mehr zugewiesen
* Fehlerkorrektur in daVinci Drucken: Druckformat Layout|Positionen (mindestens bis/ höchstens bis)
* Fehlerkorrektur in daVinci Stundenplan: Nachträgliches Ändern von Stundendauern bei Veranstaltungen führte zu Zugriffsverletzung
* Fehlerkorrektur in daVinci Stundenplan: Ansicht "Stundenplan": Warnung "Fach mehrfach am Tag" funktioniert jetzt auch für Ansicht "Alle Wochen".
* Fehlerkorrektur bei HTML-Export für Stundenpläne (letzte Stunde wurde ggf. nicht ausgegeben).
! Korrektur in daVinci Look: Anzeige der Kalenderwoche mit z.B. "32. KW: ..."
! Modifizierte HTML-Vorlagedateien "daVinci.hfm" 
! Modifizierte CSS-Vorlagedateien  

## Version 6.0.129 (25.07.2013)

* Neue Spalte "Vertreter" in der Ansicht "daVinci|Vertretungsplan|Änderungen"
* Fehlerkorrektur bei den Berechnungsfaktoren (Klassen- und Lehrerfaktor) beseitigt, Dezimalzahlen können wieder eingetragen werden
* Fehlerkorrektur bei der Wochensummenanzeige in der Ansicht "Stundenplan"
* Fehlerkorrektur bei der Übersicht "Lehrer Soll-Ist", Lehrer-Differenz wird nun korrekt berechnet
* Fehlerkorrektur beim Einspielen der Stundentafeln in die Veranstaltungslisten wird die Dauer bei gebrochenen Stundenzahlen (1,5 oder 2,5 Stunden) nun wieder korrekt angezeigt
* Fehlerkorrektur in daVinci VERTRETUNGSPLAN: in der Vertretungsstatistik ist die Filterung nach Teams nun korrekt
* Fehlerkorrektur in daVinci ANALYTICS: Summenberechnungsfehler korrigiert, Zusatzunterricht wird beachtet, Druckenfehler beseitigt.
* Kleinere Fehlerkorrekturen

## Version 6.0.126 (12.07.2013)

! Performanceverbesserungen für größere Plandateien im Stundenplanmodul

* Neues Auswahl-Dialogfenster (siehe Benutzerhandbuch)
* In den Druckformaten wurden die Gesamtplan - Layouts überarbeitet und ergänzt
* Modifizierte Druckformate in "daVinci.pfm" Vorlagedatei 
* Fehlerkorrektur Veranstaltungsliste - manuelles Ändern von Lehrern
* Sortierung von Kursen in Blöcken im Druckformat an den Stundenplan angeglichen
* Schriftarten im Druckformat "Gesamtplan Klassen" korrigiert
* Grafisches Problem im Aufsichtsbereich (Bezeichnungen der Positionen) behoben
* In den Vertretungen werden nun alle anwesenden Lehrer als mögliche Aufsichtsvertretung angeboten
* Funktion Blockungen zusammenfassen ist nun in allen Druckformaten gegeben
* Fehlerkorrektur im HTML-Export
* Spalte Klassenverband wurde entfernt, neue Spalte "Gruppe" in den Stundentafeln, der Veranstlalungsliste und in den Veranstaltungsdetails. 
  Es kann nun ein Gruppenkürzel (1, 2, A, B,..) eingetragen werden, d.h. "nicht im Klasssenverband".

## Version 6.0.124 (02.07.2013)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* Langsame Anzeige in Oberstufenplänen korrigiert.
* Schriftgrößeneinstellungen bei den Druckformaten "Einzelplan" korrigiert.
! HTML-Formatvorlagen etwas korrigiert: Vertretungsliste und Bemerkung wird über gesamte Breite angezeigt.
* Neues Eingabefeld "Gruppe" bei Veranstaltungen für Klassengruppen, z.B. A-Gruppe und B-Gruppe. Weitere Informationen siehe daVinci-Handbuch.
* Neues Auswahlfenster. Weitere Informationen siehe daVinci-Handbuch.

## Version 6.0.124 (24.06.2013)

* Fehler bei der Synchronisation der Detailfenster in der Ansicht Stundenplan bei mehreren Plänen und Listen korrigiert.
* Fehler beim Zuordnen von Räumen/LEhrer über das Passende Lehrer/Räume Fenster beiseitigt.
* Fehler beim Löschen von Fachwahlen beseitigt (Schüler wurde nicht gleichzeitig aus Kurs gelöscht).
* Fehler beim Importieren/Exportieren von Schüler Fachwahldaten (P1-Datensatz) beseitigt.
* Fehler beim Umbenennen von Blöcken beseitigt.
* Neuer Befehl "Blöcke anpassen" in der Ansicht "Kursplan|Blöcke" passt die Blockbezeichnungen an den Klassennamen an. Gleichnamiger Befehl ist auch in der Ansicht "Stundenplan | Veranstaltungsliste" zu finden.
! Mitgelieferte HTML Formatvorlagen bezüglich Ausdruck verbessert.


## Version 6.0.123 (18.06.2013)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* Fehler beim Anmelden beim ENTERPRISE Server beiseitigt (Server konnte unter betimmten Umständen Indexdatei nicht laden)
* Fehler bei Fehlzeit Klasse beeitigt: JEtzt kann auich nur ein Kurs korrekt als Fehlzeit (Entfall) eingegeben werden.
* Beim Ausdruck von Tagesvertretungsplänen wird der Tag auch dann gedruzckt, wenn nur Fehlzeit-Informationen vorhanden sind, aber die Tabelle selbst leer ist.
* Anzeige von Kursnummer in Stundenplänen korrigiert.
* daVinci LOOK: Fehler beim automatischen Neuladen von Infozeiele und Plandatei im lokalen Betrieb korrigiert.

## Version 6.0.122 (13.06.2013)

* Die Unterordner im HTML-Vorlagenordner sind umbenannt worden.
* Modifizierte Druckvorlagen
* Modifizierte HTML-Vorlagen
* Ergänztes daVinci Benutzerhandbuch.
* Ergänztes daVinci InfoServer Benutzerhandbuch.
* Ergänztes daVinci Vertretungsplan Benutzerhandbuch.
* Neue HTML-Vorlage "stsubst" für die Anzeige von HTML-Vertretungslisten auf SHOWTIME ähnlichen Public Displays. Die Vorlage nutzt JavaScript zum Weiterblättern langer Listen, d.h. die Aufteilung einer Liste auf mehrere HTML-Dateien entfällt (siehe "Tagesvertretungen Klassen Listflip").
* Neues daVinci Handbuch Kapitel "daVinci Automation" beschreibt, wie Sie daVinci mit Kommandozeilenparametern starten können, um Statistikdaten zu exportiernen.
* Wochenbezogene Veranstaltungen werden in der Veranstaltungsliste nur noch in der betreffenden Woche angezeigt (und natürlich in der Einstellung "Alle Wochen").
* daVinci Automation für Statistikexporte, siehe gleichnamigen Abschnitt im daVinci-Handbuch.
* Statistikexport Rheinland-Pfalz (edoosys) 
* Korrektur beim Audruck von Vertretungslisten
! Der Inhalt der PATHS-Datei hat sich geändert. Bitte beachten Sie die Dokumentation im daVinci Benutzerhandbuch.

## Version 6.0.121 (10.06.2013)

* Beim Tauschen von Terminen kann nun jeweils auch ein Ersatzraum direkt im Dialogfenster angegeben werden.
* Über den neuen Befehl "Raum ändern" kann der Raum einer Veranstaltung unmittelbar geändert werden.
* In den Vertretungsdialogen können jetzt mit der neuen Option "Weitere Termine dieses Lehrers im Block analog vertreten" alle Termine im Block gleichzeitig vertreten werden.
* Für die Blockkürzel Zuordnung für Termine gibt es ein  neues Auswahlfenster, in dem nur die Blockkürzel aller Termine angezeigt werden.
* "Stammdaten|Lehrer" um das Feld Personalnummer erweitert
* Im Dialog "Publizieren|Änderungen mitteilen" können jetzt auch Schüler benachrichtigt werden.
* Fehler beim Laden von Version 5 Dateien behoben: Blöcke wurden nicht korrekt übernommen.
* Fehler im daVinci Vertretungsplan: Info und Mitteilung beim Eintragung einer Vertretung mit der Art "Entfällt" wird wieder in die Auswahlliste übernommen
* Im Dialog "Publizieren|Änderungen mitteilen" funktioniert das TEAM Filter nun korrekt.
* Fehler in daVinci Kursplan: Überschneidungsprüfung bei der Kurszuordnung funktioniert wieder
* Optionen: Betreffzeile für Notfallmitteilungen ist jetzt auch im Optionenfenster eingebbar
* Fehler im Menü Drucken: Format der Datumsangabe bei Ausdruck wird beibehalten
* Fehler im Kursplan: Fehler beim Erzeugen der Blöcke korrigiert
* Neu: Fachwahlskript Hessen
* Übersichten: Zeitkonten Lehrer Darstellung der Summen in der Übersicht der Soll und Ist Stunden
* Fehler im daVinci Stundenplan: Tastenkombination Strg * F zum Löschen von Zeitpräferenzen funktioniert wieder
* Fehler im Menü Übersichten: Optionen "Alle expandieren" und "Alle schließen" korrigiert
* Fehler im daVinci Stundenplan: Anzeige der jeweiligen Fachfarbe funktioniert wieder
! Diverse Fehlerkorrekturen

## Version 6.0.120 (17.05.2013)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformatkorrektur updaten!

* Fehler beim Import von Daten im Servermodus beseitigt.
* Fehler beim Arbeiten im Servermodus (Zugriffsverletzung) beseitigt.
* Fehler beim Erzeugen von Blöcken in Kursplan im Servermodus beseitigt.
* Fehler beim Export/Import von Kurswahlen beseitigt (die Kurszuordnung wurde nicht übertragen).
! Das Benutzerrecht "Schuldatentransferdatei importieren" heißt jetzt "Daten importieren" und kontrolliert den Zugriff auf das Dialogfenster "Plan|Importieren und Exportieren".
! Das Benutzerrecht "Schuldatentransferdatei exportieren" heißt jetzt "Daten exportieren" und kontrolliert den Zugriff auf das Dialogfenster "Plan|Importieren und Exportieren".

## Version 6.0.119 (15.05.2013)

* Fehler (Zugriffsverletzung) in Ansicht "Vertretungegsplan|Vertretungen" beseitigt.
* Fehler bei Aufsichtsänderungen im Vertretungsplan beseitigt.
* Fehler beim Import von Schüler-Kurswahlen aus Magellan beseitigt: Die Kurszuorndung wurde nicht übernommen.
* HTML-Format "Mit Vertretungsplaninformationen" korrigiert, so dass Ausgabe von Änderungsinfos wieder korrekt ist.
* In HTML-Formaten ist die Zeilen/Spaltenposition der Klassen-/Fach-/Raumkürzel wieder eingebbar.
* LUSD Datenimport/export siehe "Plan|Importieren und exportieren")
* Leicht modifizierte CSS- und HTML-Vorlagen

## Version 6.0.115 (30.04.2013)

> Bitte daVinci, daVinci LOOK, daVinci INFOSERVER und daVinci-Server wegen Datenformaterweiterung updaten!

* Fehler beim Übernehmen von Blöcken aus Version 5 korrigiert.
* Fehler in Ansicht "Aufsichten" korrigiert.
* Fehler in der Ansicht "Kursplan" korrigiert.
* Fehler im Serverbetrieb (Änderungen wurden nicht gespeichert) korrigiert.
* Problem bei der Schülerverteilung im Kursplan gelöst
* Termineingabe in den Stundentafeln korrigiert
* Bei Lehrer-Stammdaten kann in der Spalte "Details" der Lehrer mit "Keine Aufsicht" aus dem Angebot der Aufsichtslehrer herausgenommen werden.
* Im Dialogfenster "Automatikparameter" kann für Lehrer nun auch die maximale Anzahl von Aufsichten eingeben werden.
* In der Ansicht "Kursplan" kann man nun über die Schaltfläche "Sortieren" im Menüband die Schüler-Fachwahlen nach Unterrichtsart/Fachstatus sortieren.
* In der Ansicht "Kursplan|Blöcke" kann man über das Rechte-Maustaste Menü die Blockung bzw. Verteilung durch Umschalt- bzw. Strg* Mausklick markierter Blöcke zurücksetzen.

## Version 6.0.114 (23.04.2013)

* Fehler unter "Vertretungen|Vertretungen" beim Vertretungseinsatz "Entfall" behoben.
* Fehler beim HTML-Export der Indexseite für Stundenpläne und Vertretungspläne behoben.
* Fehler beim Befehl "Plandatei aufräumen": Die Lehrer-Aufsichten wurden gelöscht. Wenn dies der Fall ist bitte erneut mit dieser Version "Plandatei aufräuimen" ausfüphren, damit wird der Fehler korrigiert.
! CSS-Dateien für HTML-Export etwas korrigiert.

## Version 6.0.112 (18.04.2013)

> Bitte daVinci, daVinci LOOK und daVinci-Server wegen Datenformaterweiterung updaten!

* Die Konvertierung von daVinci 5 Dateien funktioniert jetzt wieder
* Beim Drucken im Serverbetrieb konnten Vertretungsänderungen nicht bzw. nur nach "Änderungen freigeben" gedruckt werden. Dieser Fehler wurde behoben.
* Fehler bei Ereignissen des Zusatzkalenders korrigiert
* Fehler beim Eingeben von Unterrichtsentfall in Ansicht "Vertretungsplan|Vertretungen" Dialog "Vertretung entällt": Es wurde teilweise kein Entfallgrund gespeichert.
* Fehler beim Vertreten von Doppelstunden korrigiert
* Fehler beim Export von Vertretungsplänen korrigiert
* Korrigiertes Fachwahlskript für Berlin
* WICHTIG: Neue Option "Änderungen freigeben" im Dialog "Plan|Eigenschaften" auf Registerkarte "Vertretungsplan": Dadurch kann nun das explizeite Freigeben von Änderungen in lokalen wie im Servermodus gewählt werden. 
* Neue Funktion "Kursschnittmenge" in daVinci KURSPLAN
* Neue Einstellungsmöglichkeit "Änderungen freigeben" (Datei-Eigenschaften)
* INFOSERVER Ausgabe korrigiert: Indizes werden korrekt erstellt und Anpassungen für neue HTML5 Vorlagen
* Neuer HTML5 kompatibler HTML-Export, siehe dazu überarbeitetes Kapitel 16. "HTML Export" im daVinci Benutzerhandbuch
* Erweiterter Export Statistik Rheinland-Pfalz

## Version 6.0.106 (22.03.2013)

* daVinci LOOK Neuladen bei Änderungen im Serverbetrieb klappte nicht und wurde korrigiert.
* daVinci LOOK: Anzeige der Infozeile unten funktioniert wieder.
* Fachsortierung korrigiert unter "Kursplan|Fachwahlen"
* Abstürze beim Ansichtswechel in Kursplan Ansichten korrigiert.
* Kursblockungsautomatik funktioniert wieder.
* Beim Neuerstellen von Blöcken in der Ansicht KURSPLAN werden die alten Blöcke gelöscht. Dies war zuvor nicht vollständig der Fall.
* Beim Importieren einer mit daVinci 5 erzeugten Schuldatentransferdatei werden die Halbjahre als "Gewählt" markiert übernommen.

## Version 6.0.105 (20.03.2013)

> Bitte daVinci, daVinci LOOK und daVinci-Server wegen Datenformaterweiterung updaten!

* Neues Fachwahlskript für das Saarland jetzt verfügbar
* Warnung "Fach mehrfach am Tag" in der Ansicht STUNDENPLAN
* Neues Attribut "Klassenverband" bei Stundentafeln einblendbar, wird beim Kopieren in Veranstaltungsliste übernommen
* Neue Datensätze im Schuldatentransferformat für Termine (U8) und Zeitpräferenzen (K9, L9, R9, F9)
* Im Schlüsselverzeichnis-Dialog kann man jetzt wie in den Stammdaten Schlüssel aus der Windows-Zwischenablage einfügen und in diese kopieren (siehe "In Ablage kopieren" und "Aus Ablage einfügen").
* Beliebig viele Stundenplanfenster können jetzt über ANSICHT|STUNDENPLAN FREI BEWEGLICH geöffent und ggf. auf 2. Monitor geschoben werden wie in Version 5. Das Öffnen eines solchen Stundenplanfensters entspricht auch der Funktion "Zusatzpläne" in der Version 5.
* im daVinci EXPLORER wird bei "Plandatei|Hinzufügen" anschließend das Dialogfenster zum Hochladen einer Datei angezeigt (entspricht der Schaltfläche "Hochladen")  
* Neues Dialogfenster "Bearbeiten|Einzeltermine verplanen" in der Veranstaltungsliste
* Neues Dialogfenster "Bearbeiten|Barcode neu erstellen" in der Ansicht "Stammdaten|Ressourcen".
* Neue Option "Barcode-Präfix" Optionen|Einstellungen|Ressourcen
* Neues Dialogfenster "Bearbeiten|Exemplare erstellen" in der Ansicht "Stammdaten|Ressourcen".
* Das Handbuch "daVinci RESSOURCENPLAN" ist nun Teil der Auslieferung.
* Das Handbuch "daVinci ANALYTICS" ist nun Teil der Auslieferung.
* Verbessete Aufsichtsautomatik
* Fehler im Server-Modus in der Ansicht "Kursplan|Fachwahlen" beseitigt. Die markierten Halbjahre wurden nicht übertragen bzw. es gab eine Fehlermeldung.
* Funktionen Termindauer verlängern/Termindauer verkürzen/Termin teilen funktionieren jetzt wieder
* Problem beim Drucken/HTML-Export von Zusatzunterricht behoben
* Problem in Lehrer-SOLL-Berechnung bei faktorbezogener Berechnung behoben
* Ansicht "Kursplan|Blöcke": Problem beim Löschen von Blöcken behoben
* Vertretungsplan: Fehler bei nachträglicher Raumänderung behoben
* Lehrer/Raumtausch Angaben erschienen nicht im Druck und HTML-Export. Dieser Fehler wurde behoben.
* Fehlerhafte Lehrer-Ist Berechnung in daVinci ANALYTICS korrigiert
* Unnötiges Dialogfenster beim Beenden des Exports ins Schuldatentransferformat beseitigt
* Anzeigefehler im Zeitkonflikte-Fenster in der Ansicht STUNDENPLAN beseitigt.

## Version 6.0.103 (05.03.2013)
  
* Neue Kalenderdateien für das Schuljahr 2013/14 verfügbar
* In der Ansicht "Vertretungsplan|Stundenplan" werden passende Termine und Positionskonflikte angezeigt, wenn entsprechende Optionen im Menü "Plananzeige" markiert sind.
* Im Übersichtsplan können nun mehr als 20 Spalten angezeigt werden
* Wochenanzeige im Stundenplan mit KW
* Wochenauswahl im Stundenplan über KW
* Drag&Drop für Lehrer- und Raumtausch / Verschieben in "Vertretungsplan|Stundenplan"
* Neue Infozeile in daVinci-Look analog zu Version 5
* Fehlende Anzeige der verschobenen Stunden im Vertretungsplan beseitigt.
* Fehlerhafte Fokussierung auf Woche/Stunde bei Umschalten auf Klassen/Lehrer/Raumplan behoben 
* Anzeigefehler im daVinci EXPLORER für "Analysieren" (daVinci ANALYTICS) behoben

## Version 6.0.102 (18.02.2013)

* Im Vertretungsplan Ansicht "Vertretungen" konnte manchmal die Registerkarte FÄCHER bzw. RÄUME nicht angeklickt werden und somit kein Fach oder Raum modifiziert werden (bei Vertretungen). Dieser Fehler wurde behoben.
* Anzeigefehler im daVinci EXPLORER für "Analysieren" (daVinci ANALYTICS) behoben.
* Kleinere Anzeigefehler bei der Vollbildanzeige von daVinci-Look korrigiert.
! Bitte auch daVinci-Server updaten!

## Version 6.0.101 (01.02.2013)

* Anzeigefehler beim Vertauschen von Terminen/Lehrern/Raumen im Vertetungsplan korrigert.
* In der Ansicht "Vertretungsansicht|Stundenplan" können Sie über den Befehl "Neue Fehlzeit" direkt eine Raumfehlzeit eingeben. Neu ist dabei nun, dass Sie auch einen Ersatztraum direkt eingeben können, ohne dazu in der Ansicht "Vertretungen" den Ersatzraum zuzuordnen.
* Erweiterter XML-Datenexport für Stundenplan- und Vertretungsplandaten unter "Plan|Importieren und Exportieren".
! Bitte auch daVinci-Server updaten!

## Version 6.0.100 (18.01.2013)

* Fehler bei der Änderung von Blockbezeichnungen für Termine gelöst.
* Ansicht "Kalender|Jahresansicht" zeigt nun korrekt an.
* Fachstatus bei Stundentafeln wird nun korrekt gespeichert.
* Neuer XML-Datenexport für Stundenplan- und Vertretungsplandaten unter "Plan|Importieren und Exportieren".
! Bitte auch daVinci-Server updaten!

## Version 6.0.98 (11.01.2013)

* Blöcke löschen und neu erzeugen wurde ab letztem Servieupdate erst nach "Plan aufräumen" korrekt umgesetzt. Dieser Fehler ist beseitigt.
* Fehler beim Importieren eines Schlüsselverzeichnissses und danach folgendem Import von Magellan beseitigt.
* Raum-/Lehrerautomatik ohne Setzautomatik funktionierte nicht. Der Fehler ist nun behoben.
* Aufsichtsautomatik funktionierte nicht bei wochenbezogenen Aufsichten. Der Fehler ist behoben.

## Version 6.0.97 (07.01.2013)

> Modifiziertes Dateiformat, bitte auch daVinci Server und daVinci Look updaten!

* * daVinci-Infoserver ist nun Teil des Setups
* Fehler bei der Anzeige vertauschter Termine beseitigt.
* Neues Fachwahlskript RLP-FW-APO-BGY-2010.js
* Neue Spalte "Verordnungstyp" in Ansicht "Stammdaten|Klassen". Angabe für bestimmte Fachwahl-Skripte erforderlich. 
* Beim Ausführen des Befehls PLAN AUFRÄUMEN konnten ggf. die Aufsichtspläne gelöscht werden. Dieser Fehler wurde korrigiert.
! Diverse Fehlerkorrekturen

## Version 6.0.96 (04.12.2012)

* Neue Option in "Optionen|Plananzeige" erlaubt das Einblenden der fehlenden Klassen/Lehrer in den Stundenplänen der Ansicht "Vertretungsplan"
* Neues Dialogfenster "Fehlstelle" zum nachträglichen Bearbeiten einer Fehlstelle.
* Anzeige von Vertretungsinformationen war nicht in allen Fällen vollständig. Dieser Fehler wurde korrigiert.
* Raumautomatik zusammen mit Setzautomatik funktionierte nicht. Dieser Fehler wurde korrigiert.

## Version 6.0.95 (30.11.2012)

> Modifiziertes Dateiformat, bitte auch Server und Look updaten!

* Performanz verbessert
* Überarbeitete Automatik mit neuen Automatikparametern (Doppelstunden z.B. "1-2" in Veranstaltungsliste)
* Automatik für Aufsichten
* Darstellungsstil etwas modifiert 
* Alle Listen (Stammdaten, Übersichten etc.) können jetzt gedruckt oder als PDF abgelegt werden inkl. Vorschau
* Vertretung, Raumänderung, Aufsichtsvertretung kann jetzt durch frei wählbare Hintergrundfarbe im Optionen-Fenster unterschieden werden
* Fachfarben, falls vergeben, werden in der Veranstaltungsliste angezeigt
* Neuer Navigationspunkt links "Übersichten", enthält auch die Übersichten die bisher unter "Extras" zu finden waren.
* Bei Termintausch kann jetzt angegeben werden, ob Lehrer/Raum mitgetauscht werden sollen oder nicht
* daVinci-Explorer: Analysieren überarbeitet und um neuen Diagrammansichten ergänzt inkl. Druckmöglichkeit
* Unter "Plan" neuer Befehl "Eigenes Kennwort ändern". Damit kann in daVinci und daVinci-Look der Benutzer das eigene Kennwort ändern. Dies sollten neue Benutzer als erstes ausführen, um das vom Masterplaner zugewiesene Kennwort in ein eigenes zu ändern.
* Leichtere Datenerfassung: Beim Eintippen von Klassen, Fächern, Lehrern und Räumen in der Veranstaltungsliste wird bei einem neuen Kürzel (also einem, das noch nicht als Stammdatum vorhanden ist) gefragt, ob es unmittelbar als Stammdatum angelegt werden soll. 
* In Liste (Stammdatenliste, Veranstaltungsliste usw.) kann man jetzt per Strg+C und Strg+V oder über das neue feldbeuzogenen Kontextmenü (rechte Maustaste) kann man Texte kopieren und einfügen. 
* Mit Strg+Mausrad kann man jetzt im Bildschirmplan die Anzeige vergrößern und verkleinern. Nur Mausrad scrollt den Plan nach oben und unten. Damit entspricht das Verhalten dem Windows-Standard.
* Mit Strg+C und Strg-V kann man Inhalte aus Textfeldern und Zahlenfelder in Tabellen kopieren, z.B. in den Stammdatenansichten.
* Neuer Befehl "Stammdaten|Termine löschen" für einzel- und mehrfach markierte Zeilen
* Neuer Befehl "Stammdaten|Veranstaltungen löschen" für einzel- und mehrfach markierte Zeilen
* Neuer Befehl "Stammdaten|Klassen|Stundentafel erzeugen" für einzel- und mehrfach markierte Zeilen
* Neuer Befehl "Stammdaten|Zeitpräferenzen zuweisen" für Sammlezuweisungg von Zeitpräferenzen
* Neue Spalte "Stundentafel Spalte "Doppelstd"
* Behebung des Pfadproblems der daVinci.pfm, daVinci.htm und daVinciLogo.png -* sind nun wieder im Benutzerverzeichnis abgelegt
* Behebung der Fehlermeldung bei tages- und wochenbezogener Summenberechnung
* Neue Option "Nur Einzeltermine" in HTML-Formaten, sorgt für Einzeltermine und damit korrekte Darstellung bei Stundenplänen mit überlappenden Doppelstunden 
* Diverse Fehlerkorrekturen  

## Version 6.0.94 (25.09.2012)

### Neue Funktionen

* Entfall-Dialog funktioniert jetzt auch für Mehrfachmakriereungen.

### Fehlerkorrektur

* Fehler bei direkten Vertretern korrigiert.
* Fehler in der Ansicht "Aufsichtplan" korrigiert.

## Version 6.0.93 (24.09.2012)

### Neue Funktionen

* Im Fenster "Plan|Eigenschaften" können Sie jetzt unter Termine die Schriftfarbe und die Schriftauszeichnung der Termininhalte für die Bildschirmpläne ändern.
* Unter "Plan|daVinci-Optionen|Vertretungsplan" können Sie vordefinierte Angaben für die Spalten "Info", "Mitteilung" und "Bemkerung" im Vertretungsplan machen.
* In der Ansicht "Stundenplan|Aufsichtsplan" stehen die neuen Befehle "Aus Wochen übernehmen" (alle Aufsichten aus einer Woche übernehmen) und "Alle löschen" (alle Aufsichten in allen Aufsichtsbereichen löschen) zur Verfügung.

### Fehlerkorrektur

* Fehler in der Ansicht KURSPLAN, der zum Absturtz des Programms in bestimmten Anzeige situationen führte, beseitigt. Rufen Sie ggf. einmalig den Befehl "Extras|Plandatei aufräumen aus". 

## Version 6.0.91 (18.09.2012)

* Bei Vertretungen wird bei "Ausfallstd" und "Ausfallstd Klasse" ggf. die Klasse unter "Priorität" angezeigt.

### Fehlerkorrektur

* Fehler beim D6-Datensatz für Landesstatistik Rheinland-Pfalz korrigiert.
* Druckformat für Aufsichtspläne setzt Schriftangaben und Seitenumbruch nun korrekt um.
* Diverse Fehlerkorrekturen

## Version 6.0.90 (14.09.2012)

### Neue Funktionen

* In der Ansicht "Vertretungsplan|Änderungen" kann man mit Rechter-Maustaste Änderungen veröffentlichen bzw. nicht veröffentlichen. 
* daVinci-Look: Über "Start|daVinci-Optionen|Vollbild" kann jetzt das Logo Ihrer Schule in der Kopfzeile bei Vollbildmodi angezeigt werden.
* Das neue daVinci KURSPLAN Benutzerhandbuch ist nun Teil dieses Setups und kann auch von unserer Website geladen werden.

### Fehlerkorrektur

* Fehler beim D6-Datensatz für Landesstatisk Rheinland-PFalz korrigiert.
* Anzeige von Änderungen in Aufsichtsplänen weren auf Bildschirm und Ausdruck korrekt wiedergegeben.
* daVinci-Look: Schülerpläne und Fachpläne sind nun korrekt auswählbar.
* daVinci-Look: Lehrerpläne können nun nicht mehr über das Suchen-Feld ausgewähjlt werden, wenn die Lehreransicht in den Optionen weggeblendet wurde.

## Version 6.0.89 (07.09.2012)

### Fehlerkorrektur

* Fehler beim Drucken von stundenplänen mit Änderungsinfos beseitigt.
* Lizenz "Enterprise" war wegen eines Fehlers unberücksichtigt, die entsprechenden Befehle waren nicht verwendbar. Dieser Fehler ist beseitigt.
* Fehlerhaftes Weiterschalten der Detailansicht beim Planen beseitigt.
* Verbesserte Kursblockungsautomatik
* Fehler in Blockungsautomatik beseitigt.
* Importieren von Schlüsselverzeichnissen funktionierte unter bestimmten Umständen nicht. Dieser Fehler wurde beseitigt.

## Version 6.0.88 (03.09.2012)

### Fehlerkorrektur

* Weiterschalten der Wochen im Planeditor schaltet nun auch korrekt die Detaiansichtinhalte weiter.
* "Listenindex out of range" Fehler im Planeditor beseitigt.
* Spalten "VLehrer" und "VFach" werden jetzt beim Ausdruck korrekt gefüllt.
* Teilnehmer doppelt in Kurs Fehler und damit verbundene Programmabstürze beseitigt. Bitte führen Sie ggf. "Extras|Plandatei aufräumen" aus.
* Fehler in Blockungsautomatik beseitigt.

## Version 6.0.87 (17.08.2012)

### Fehlerkorrektur

* Korrigiertes Fachwahlskript Berlin
* Diverse Fehler beseitigt.

## Version 6.0.86 (09.08.2012)

> Neues Datenformat, bitte auch daVinci-Server updaten.

### Neue Funktionen

* Neue Eingabemöglichkeit im Eingenschaften-Dialog auf Registerkarte "Kursplan" zur Kennzeichnung von Leistungskursen.
* Das in Rheinland-Pfalz verwendete Beifach wird im Dialog "Veranstaltung bearbeiten" als "+" im neuen Eingabefeld "Öffentlich" eingegeben und auch nach dort aus Version 5 konvertiert. Eingaben in diesem Feld werden in Plan an das Kürzel des Fachs angehangen.

### Fehlerkorrektur

* Diverse Fehler in Kursplan beseitigt.

## Version 6.0.85 (06.08.2012)

> Auch der daVinci-Server musste geupdatet werden wegen einer Datenstrukturerweiterung. Das war im Update davor nicht der Fall.

### Version 6.0.84 (06.08.2012)

### Fehlerkorrektur

* Fehler beim Serviceupdate beseitigt: Beim Updaten konnte die Einträge im Start-Menü verloren gehen.

## Version 6.0.83 (04.08.2012)

### Neue Funktionen

* Statistik Export Niedersachen
* Statistik Export Nordrhein-Westfalen BBS
* Statistik Export Nordrhein-Westfalen ABS
* Statistik Export Hessen

### Fehlerkorrektur

* Gross-/Kleinschreibung von Leistungs- und Grundkursen im Plan erfolgt jetzt korrekt aufgrund der Einstellung im Dialog "Plan|Einstellungen|Kursplan".
* Diverse Fehler in Kursplan beseitigt.
