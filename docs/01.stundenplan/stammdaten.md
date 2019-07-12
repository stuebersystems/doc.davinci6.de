# Stammdaten

Die Stammdaten sind die grundlegenden Daten Ihres Plans bzw. Ihrer Schule. Hier erfassen Sie Klassen, Lehrer, Fächer, Räume, und vieles mehr. Den Programmbereich "Stammdaten" öffnen Sie, indem Sie auf der linken unteren Seite den Bereich anklicken.
![Stammdaten-Fenster](/assets/images/Stammdaten02.png)

Das Arbeitsfenster des Programmbereichs "Stammdaten" bestehen aus Listen, auf denen jeweils Einträge zu einer bestimmten Datenkategorie angelegt werden können.

Bei den Datenkategorien die hier erfasst werden können, handelt es sich namentlich um Klassen, Lehrer, Räume, Fächer,Stundentafeln, Aufsichtsbereiche, Perioden, Gebäude, Teams, Ressourcen, Schüler. Sie werden auf der linken Seite im oberen Abschnitt angezeigt.
Im Optionsmenü von DAVINCI unter `Extras > Optionen > Ansicht` können Sie einzelne Stammdatenbereiche ausblenden. Ungenutzte Bereiche werden so nicht mehr angezeigt und die Ansicht ist übersichtlicher.

![Ansicht](/assets/images/Optionen.Ansicht.Stammdaten.png)

Da die Stammdaten-Ansichten aus Listen bestehen, sollten Sie den Abschnitt "[Mit Listen arbeiten](/davinci-stundenplan/mit-listen-arbeiten.md)" lesen, um sich mit den Ansichts- und Sortierungsoptionen vertraut zu machen.

Um Stammdaten eintragen, bearbeiten oder löschen zu können müssen Sie sich im `BearbeitenModus`befinden. Sie können diese Option unter `Extras > Optionen > Einstellungen` für den Stammdatenbereich automatisch einstellen. Wählen Sie dazu den Haken bei `„Stammdatenfenster > Im Bearbeiten-Modus`. Sollten Sie sich nicht im Bearbeiten-Modus befinden, können Sie dies auch in den Stammdaten direkt unter `Start > Bearbeiten > Bearbeiten-Modus`, über `Rechtsklick > Bearbeiten-Modus` über das Tastenkürzel ``Strg+E`` einstellen.

!!! info "Hinweis"

    Neue Einträge in den Stammdaten benötigen wenigstens eine Eingabe im Feld **Kürzel**.
Jedes Kürzel ist eindeutig und kann nur einmal eingegeben werden. Je nachdem ob Sie unter `Extras > Optionen > Einstellungen` die Option ``Bei Kürzel-Eingabe Groß- und Kleinschreibung beachten`` markiert haben, wird die Groß- bzw. Kleinschreibung beachtet.

## Aufsichtsbereiche

![Aufsichtsbereiche](/assets/images/Stammdaten.Aufischtsbereiche.png)

In der Ansicht ``Stammdaten > Aufsichtsbereiche`` können Sie die Bereiche des Schulgeländes eintragen, in denen zu bestimmten Zeiten Lehrer zur Aufsicht anwesend sein müssen. Dazu erstellen Sie unter ``Stundenplan > Aufsichtsplan`` für jeden Bereich einen Aufsichtsplan.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Aufsichtsbereichs
Bezeichnung |  Bezeichnungstext
Zeitrahmen |  Zeitrahmen für die Aufsichten, siehe ``Extras > Zeitrahmen``
Räume |  die an den Aufsichtsbereich angrenzenden Räume, siehe  ``Stammdaten > Räume``
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

## Fächer

![Stammdaten Fächer](/assets/images/StammdatenFächer.png)

In der Ansicht  ``Stammdaten > Fächer`` erfassen Sie die Fächer, die an Ihrer Schule unterrichtet werden. Die eingegebenen Fächer können Sie in der Ansicht ``Stammdaten > Lehrer`` und ``Stammdaten > Stundentafeln`` zuordnen. 
Für jeden Eintrag kann dann ein Plan angezeigt werden. Den Plan eines bestimmten Fachs können Sie aufrufen, indem Sie auf die betreffende Zeile und dann  ``Start > Gehe zu Stundenplan`` oder ``Rechte Maustaste > Gehe zu Stundenplan`` klicken oder die ``F9`` Taste benutzen.

Spalte | Inhalt
--------|-------------------------------------------
Kuerzel | Fachkürzel
Bezeichnung |  Freies Bezeichnungsfeld
Kategorie | Kategorie (weitere Informationen im Abschnitt Kursplanung)
Aufgabenbereich | Aufgabenbereich laut Oberstufenverordnung
Farbe | Kann im Stundenplan eingeblendet werden, siehe "Plan > Eigenschaften> Stundenplan` > Planeinträge"
Hintergrund | Macht die gewählte Farbe im Stundenplan als Hintergrundfarbe sichtbar
Bemerkung | Bemerkungstext
Fachstatus | siehe ``Extras > Schlüsselverzeichnisse > Fachstatus``
Team | Teamzughörigkeit des Fachs, siehe ``Stammdaten > Teams``
Zeitkonto | Konto auf das Stunden des Fachs verbucht werden, siehe ``Extras > Schlüsselverzeichniss > Lehrer Soll-Schlüssel``
Fachräume | Liste der Fachräume, siehe ``Stammdaten > Räume``
Vertretung | Vertretungsoptionen ``Präsenz``, ``Keine Vertretung`` und ``keine Anrechenstunden``
Schlüssel | Bundeslandspezifische Kennzeichnung des Fachs
Details | Zusätzliche Optionen für den Magellan Abgleich ``nicht statistikrelevant`` und ``kein MAGELLAN-Abgleich``

## Gebäude

![Stammdaten Gebäude](/assets/images/Stammdaten Gebäude01.png)

Auf der Liste „Gebäude“ können Sie unterschiedliche Standorte sowie die Wegzeiten zwischen dem Hauptgebäude und den anderen Standorten erfassen.

In der Spalte ``Wegzeit`` können Sie die Wegzeit in Minuten von einem Nebengebäude zum Hauptgebäude eintragen. Das Hauptgebäude wird dabei durch keinen Eintrag (keine Wegzeit) definiert. Eine Erfassung der Wegzeiten zwischen den Nebengebäuden ist nicht möglich. In der Ansicht ``Räume`` können Sie jedem Raum eine Gebäude (Spalte ``Gebäude``) zuweisen. Im Stundenplan werden Terminkonflikte bei der Raumplanung, die durch nicht ausreichende Wegzeiten zwischen Haupt- und Nebengebäuden entstehen, mit einem Warnsymbol rechts unten im Termin markiert. Die DAVINCI Automatik achtet darauf, Wegzeiten zu vermeiden, indem möglichst wenig Wechsel zwischen den Gebäuden geplant werden oder in dem eine Pause oder Freistunde für die Wegzeit eingeplant wird.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Gebäudes
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt
Bezeichnung | Bezeichnung des Gebäudes
Wegzeit | Wegzeit in Minuten zum Hauptgebäude
Campus | Gebäude können wiederum in ``Campus`` zusammengefasst werden. Dazu müssen Sie in der Ansicht ``Stammdaten > Campus`` diese eingeben.

## Klassen

In der Liste "Klassen" erfassen Sie die Klassen, die an Ihrer Schule unterrichtet werden. Für jeden Eintrag, den Sie in der Liste "Klassen" vornehmen, wird im Bereich ``Stundenplan`` ein eigener Klassenplan angelegt. Den Plan einer bestimmten Klasse können Sie direkt aus der Stammdatenliste „Klassen“ heraus aufrufen. Klicken Sie dazu eine Klasse an und wählen `Start > Gehe zu Stundenplan`, `Rechtsklick > Gehe zu Stundenplan` oder benutzen Sie die Funktionstaste `F9`.

In der Stammdatenliste "Klassen" können Sie verschiedene Einstellungen vornehmen, die für die weitere Stundenplanung relevant sind. Außerdem stehen Ihnen zahlreiche Spalten zur Verfügung.

![Stammdaten Klassen](/assets/images/StammdatenKlassen01.png)

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel der Klasse
Bezeichnung | Bezeichnung der Klasse
Farbe | Kann im Stundenplan eingeblendet werden, siehe `Plan > Einstellungen >  Stundenplan > Planeinträge` 
Lehrer 1 | Klassenlehrer
Lehrer 2 | ggf. zweiter Klassenlehrer
Raum | Klassenraum/Stammraum der Klasse
Stundentafel | Stundentafel der Klasse
Modus | Unterrichtsmodus `Klassenverband` oder `Kurse`. Wählen Sie `Kurse` für Klassen der gymnasialen Oberstufe
Stufe | Stufenangabe, wichtig für die gymnasiale Oberstufe
Schüler | Schüleranzahl, falls Sie keine Schüler in DAVINCI eingeben, wird sonst durch die Schüler unter `Stammdaten > Schüler` automatisch berechnet.
Team | Team bzw. Abteilungen, siehe `Stammdaten > Teams`
Periode | siehe `Stammdaten > Periode`
Schule | Schulnummer bzw. Mandantennummer aus MAGELLAN
Bildungsgang | siehe `Extras > Schlüsselverzeichnisse > Bildungsgänge`
Benutzername | Benutzername für den Serverbetrieb, kennzeichnet den Plan der Klasse 
Schulform | siehe `Extras > Schlüsselverzeichnisse > Schulformen`
Gebäude | siehe `Stammdaten > Gebäude`
Zeitrahmen | Dieser Klasse einen eigenen, unter `Extras > Zeitrahmen` erstellten Zeitrahmen zuweisen
Attribut | Bundeslandspezifisches Feld
Details | Zusätzliche Optionen für den MAGELLAN Abgleich `nicht statistikrelevant` und `kein MAGELLAN Abgleich`
Startjahr | Bundeslandspezifisches Feld
Halbjahr | Bundeslandspezifisches Feld
Skript | Wählen Sie hier das Fachwahlskript für Oberstufenklassen
Verordnungstyp |  Bezeichnet ggf. die Prüfungsverordnung für das Fachwahlskript
Faktor | Für die Verrechnungsart `Faktorbezogen` eigener Klassenfaktor (z.B. für Halbtagsklassen)
Gültig von / bis | Gültigkeitszeitraum aller Veranstaltungen dieser Klasse
Merkmal | siehe Schlüsselverzeichnis `Klassenmerkmale`
Schulstelle | siehe Schlüsselverzeichnis `Schulstelle`
Zeiträume | Zeiträume für alle Veranstaltungen der Klasse
Ausnahmen | Ausnahme-Zeiträume für alle Veranstaltungen der Klasse
Kalender | Kalender dieser Klasse, z.B. falls Sie Klassen aus verschiedenen Bundesländern haben
Externe ID | ID für ein Fremdprogramm
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

## Lehrer

![Stammdaten Lehrer](/assets/images/StammdatenLehrer.png)

In der Liste "Lehrer" erfassen Sie die Lehrkräfte, die an Ihrer Schule unterrichten. Den Plan eines bestimmten Lehrers können Sie direkt aus der Liste "Lehrer" heraus aufrufen. Klicken Sie dazu einen Lehrer an und wählen `Start > Gehe zu Stundenplan`, `Rechtsklick > Gehe zu Stundenplan` oder benutzen Sie die Funktionstaste `F9`.

!!! info "Hinweis"

    Über `Stammdaten > Bearbeiten > Lehrer-Zeitkonto bearbeiten` öffnen Sie das Zeitkonto-Fenster für den aktuellen Listeneintrag. Dort können Sie die Ermäßigungs- und Mehrarbeitsstunden eingeben.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Lehrers
Titel | Titel des Lehrers
Nachname | Nachname des Lehrers
Mittelname | Zweitname
Vorname | Vorname des Lehrers
Farbe | Kann im Stundenplan eingeblendet werden, siehe "Plan > Einstellungen > Stundenplan` > Planeinträge"
Symbol | Lehrersymbol, klicken Sie im Bearbeiten-Modus in die Spalte und dann auf ``Rechte-Maustaste > Laden`` um ein Bild zu laden, kann im Plan angezeigt werden, siehe ``Plan > Einstellungen > Stundenplan > Planeinträge > Lehrersymbole anzeigen`` 
Geschlecht | Geschlecht des Lehrers
Geb. Datum | Geburtsdatum
Fächer | Klicken Sie hier und wählen Sie die Fächer, die der Lehrer unterrichten darf
Teams | Teams, zu denen der Lehrer gehört, siehe "Stammdaten > Teams“
E-Mail | E-Mail des Lehrers
Mobil | Handynummer des Lehrers
Schule | Schulnummer oder Mandantennummer aus MAGELLAN
Bemerkung | Freies Bemerkungsfeld
Details | Zusätzliche Optionen für den MAGELLAN Abgleich ("nicht statistikrelevant" und "kein MAGELLAN Abgleich") und die Option "inaktiv"
Zeitrahmen | siehe "Extras > Zeitrahmen" erstellten Zeitrahmen zuweisen
Benutzername | Benutzername für den Serverbetrieb, kennzeichnet den Plan des Benutzers/Lehrers
Personalnr. | Personalnummer
Stundensatz | Stundensatz, z.B. 50 für 50EUR, kann in Zeitkonto mit "Normierter Stunde" multipliziert werden (siehe "Plan > Eigenschaften > Statistik")
Eintritt / Austritt | Eintritts- und Austrittsdatum
Externe ID | ID für ein Fremdprogramm
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

## Lehrer-Zeitkonten

![Zeitkonto bearbeiten](/assets/images/ZeitkontoBearbeiten.png)

Im Lehrer-Zeitkonto Fenster erfassen Sie für einen Lehrer dessen Ermäßigungs- und Mehrarbeitsstunden. Die Ermäßigungs- und Mehrarbeitsgründe können Sie im Schlüsselverzeichnis `Extras > Schlüsselverzeichnisse > Lehrer-Soll-Schlüssel eingeben`.

!!! info "Hinweis"

    Für bestimmte Bundesländer werden in DAVINCI bereits die offiziellen Schlüssel mitgeliefert. Sie können Sie im Dialogfenster `Lehrer-Soll-Schlüssel `über die Schaltfläche `Importieren` einlesen.

Für jeden Ermäßigungs- bzw. Mehrarbeitsgrund geben Sie in der Spalte ``Stunden`` die entsprechende Stundenzahl ein.

### Zeitkonto Operatoren

Operator| Beschreibung
-|-
P |Pflicht- oder Regelstunden, die einem Lehrer aufgrund rechtlicher Vorgaben als allgemeine Unterrichtsverpflichtung auferlegt sind. Geben Sie in der Spalte „Stunden“ die betreffende Stundenzahl an. Einen Standardwert können Sie unter `Extras > Optionen > Einstellungen > Lehrer-Pflichtstunden standardmäßig` eingeben.
- | Ermäßigungsstunden, um welche die allgemeine Unterrichtsverpflichtung des Lehrers gemindert wird. Geben Sie in der Spalte „Stunden“ die betreffende Stundenzahl an.
+ |Ergänzungs- bzw. Mehrarbeitsstunden, um welche die allgemeine Unterrichtsverpflichtung des Lehrers erhöht wird
D |Differenz aus Soll und Ist vom Vorjahr. Die Stundenanzahl in der Spalte „Stunden“ wird in beim Erstellen eines neuen Stundenplans über den Planvorbereitungsassistenten automatisch aus dem vorhergehenden Plan übernommen. Sie können sie hier auch manuell eingeben.
A |Stundenplan-Zeitkonto: In der Ansicht `Stammdaten > Fächer`  können Sie in der Spalte „Zeitkonto“ für einem Fach einen Lehrer-Soll-Schlüssel als Zeitkonto zuweisen. Die Stundenanzahl in der Spalte „Stunden“ wird in diesem Fall automatisch aufgrund des Lehrerplans berechnet.
C |Kalender-Zeitkonto: In der Ansicht „Kalender“ können Sie im Ereignis-Fenster bei „Zeitkonto“ einem Ereignis einen Lehrer-Soll-Schlüssel als Zeitkonto zuweisen. Die Stundenanzahl in der Spalte „Stunden“ wird in diesem Fall automatisch aufgrund des der entsprechenden Kalendereinträge berechnet.
<Leer> |Bemerkung, geht nicht in die Berechnung ein

### Zeitkonto Summen

Summe |Beschreibung
-|-
Soll |Summe aus Pflichtstunden, Ermäßigungs- und Mehrarbeitsstunden
Ist |Ist-Stunden des Lehrers, die sich aus den geleisteten Unterrichtsstunden entsprechend dem individuellen Stundenplan des Lehrers ergeben
Diff |Differenz zwischen Soll und Ist

![Schlüsselverzeichnis Lehrer-Soll-Schlüssel](/assets/images/Lehrer-Soll-Schlüssel.png)

!!! info "Hinweis"

    Die Pflichtstunden können Sie für jeden Lehrer gesondert festlegen. Einen Standardwert können Sie unter `Extras > Optionen > Einstellungen > Lehrer-Pflichtstunden standardmäßig` eingeben.

Alle Lehrer die Sie nun im Stammdatenfenster hinzufügen (neu erfassen), erhalten automatisch den eingetragenen Lehrer-Pfichtstundenwert standardmäßig. Lehrer die bereits im Stammdatenfenster gelistet sind, bleiben von diesem eingetragenen Standardwert unberührt.

![DAVINCI Optionen, Bereich "Einstellungen"](/assets/images/DAV.Optionen.Einstellungen.png)

## Perioden

![Stammdaten Aufsichtsbereiche](/assets/images/Stammdaten.Perioden.png)

In der Ansicht ``Stammdaten > Perioden`` können Sie individuelle Wochenschemata für wiederkehrenden Unterricht anlegen. Eine Periode stellt eine Teilmenge aller Unterrichtswochen eines Planungszeitraums dar. Das Anlegen von Perioden ist immer dann sinnvoll, wenn Sie mit wiederkehrenden Unterricht planen möchten, der nicht in allen Unterrichtswochen in gleicher Weise stattfinden oder eine Klasse nur in bestimmten Wochen unterrichtet werden soll (z.B. Turnusunterricht).

Beim Anlegen einer neuen Veranstaltung in der Ansicht Stundenplan haben Sie grundsätzlich die Wahl, ob eine Veranstaltung nur "einmalig" in einer bestimmten Kalenderwoche oder "periodisch" in bestimmten Unterrichtswochen eingefügt wird (siehe ``Stundenplan > Veranstaltungen > Veranstaltung/Termin bearbeiten`` Eingabefeld ``Wiederholung``).

Durch das Zuweisen einer Periode können Sie festlegen, dass ein wiederkehrender Termin nicht in allen, sondern nur in ausgewählten Unterrichtswochen stattfinden soll. So besteht z.B. die Möglichkeit anzugeben, dass ein bestimmter Unterricht nur im 1. Halbjahr oder in den ungeraden Kalenderwochen stattfindet. Daraus ergibt sich womöglich der Bedarf, dass anderer Unterricht komplementär dazu im 2. Halbjahr oder in den geraden Kalenderwochen verplant werden soll. Damit Sie diese und andere Wochenschemata für die Unterrichtsplanung einsetzen können, können Sie in den Stammdaten jeweils eine Periode mit den zugehörigen Kalenderwochen anlegen.

Neben der Möglichkeit, Perioden einzelnen Veranstaltung oder Terminen zuzuweisen, können Sie eine Periode auch in den Stammdaten einer Klasse zuweisen (Spalte ``Periode``). Alle wiederkehrenden Unterrichtstermine dieser Klassen finden dann standardmäßig nur in den vorgegebenen Kalenderwochen der ausgewählten Periode statt.

![Wochen bearbeiten](/assets/images/WochenBearbeiten.png)

Die wesentliche Aufgabe beim Anlegen einer Periode besteht darin, zu definieren, welche Kalenderwochen diese Periode umfassen soll. Dazu dient das Dialogfenster "Wochen bearbeiten", das Sie über die Schaltfläche mit den drei Pünktchen im Spaltenfeld "Wochen" aufrufen können. Die Nummern bei "Unterrichtswochen" stehen für die Kalenderwochen einer Plandatei. Die eingeklammerten Nummern kennzeichnen die Kalenderwochen, die unter ``Plan > Eigenschaften > Statistik`` vom Unterricht ausgenommen wurden. Sie stehen nicht mehr als Unterrichtswochen zur Verfügung.

Mit den Kontrollkästchen neben den nicht eingeklammerten Nummern legen Sie fest, welche Kalenderwochen die Periode beinhaltet. Setzen Sie den Haken im Kontrollkästchen um die nebenstehende Kalenderwoche hinzuzufügen. Entfernen Sie den Haken um die zugehörige Kalenderwoche wieder zu löschen.

Mit den fünf Schaltflächen neben dem Bereich "Unterrichtswochen" können Sie die Auswahl der Kalenderwochen teilweise automatisieren. Klicken Sie auf die Schaltfläche ``Alle Wochen löschen``, um die Haken aus allen Kontrollkästchen zu entfernen. Klicken Sie auf die Schaltfläche `Alle Wochen markieren`, um Haken vor allen Kalenderwochen zu setzen. Mit der Schaltfläche `Jede 1. Woche markieren` erreichen Sie, dass jede erste Woche ausgehend von der ersten angezeigten Kalenderwoche markiert wird. Mit der Schaltfläche `Jede 2. Woche markieren` bewirken Sie, dass jede zweite Woche ausgehend von der zweiten angezeigten Kalenderwoche aktiviert wird. Die Schaltfläche `Wochen markieren` markiert alle Kalenderwochen entsprechend Ihrer Eingaben in den Feldern "Alle X Wochen" und "Jede X. Woche". Die Angabe im erstgenannten Feld legt fest, in welchem Wochenabstand die Markierung erfolgt. Mit der Eingabe im letztgenannten Feld definieren Sie ausgehend von welcher Kalenderwoche die Markierung vorgenommen wird. Auf diese Weise können Sie komplexere Wochenschemata automatisch eintragen lassen. Mithilfe dieser Funktion können Sie bestimmte häufig auftretende Wochenmuster sehr leicht zu erzeugen, z.B. eine Periode, die jede 4. Woche ausgehend von der ersten Kalenderwoche umfasst. Klicken Sie ``OK`` und die Nummern der ausgewählten Kalenderwochen werden nun im Feld "Wochen" der zugehörigen Periode eingetragen.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Teams
Bezeichnung | Bezeichnungstext
Faktor | Wert wird für die Umrechnung von Wochenstunden auf Wochenmittelwerte verwendet
Wochen | Unterrichtswochenmuster
Wochenanzahl   | Anzahl der Unterrichtswochen, errechnet sich automatisch aufgrund der Spalte "Wochen")
Team   | ordnet die Periode einem Team zu
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

## Räume

![Stammdaten Räume](/assets/images/StammdatenRäume.png)

In der Liste "Räume" können Sie die Räume erfassen, die für die Unterrichtsplanung zur Verfügung stehen. Den Plan eines bestimmten Raumes können Sie direkt aus der Liste „Räume“ heraus aufrufen. Klicken Sie dazu einen Raum an und wählen `Start > Gehe zu Stundenplan`, ``Rechtsklick | Gehe zu Stundenplan`` oder Sie benutzen die Funktionstaste `F9`.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Raumes
Bezeichnung | Bezeichnungsfeld
Farbe | Kann im Stundenplan eingeblendet werden, siehe `Plan > Eigenschaften > Stundenplan > Planeinträge`
Bemerkung | Bemerkung
Kapazität | Maximale Plätze in diesem Raum
Raumart | siehe `Extras > Schlüsselverzeichnisse > Raumarten`
Teams | Teams/Abteilungen, siehe `Stammdaten > Teams`
Gebäude | Verknüpft mit dem  `Stammdaten > Gebäude`
Alternativ | Alternativer Raum wenn dieser besetzt ist 
Austattung | Ausstattungsliste des Raums
Benutzer | Benutzername
Eingeschränkt | 0=keine Einschränkung..4=möglichst nicht verwenden
Lehrer | siehe ``Stammdaten > Lehrer``
Details | weitere Optionen ``Nicht verfügbar`` und ``Zwingend dieser oder Alternativraum``
Barcode | zur Kennzeichnung des Raums
Zeitrahmen | siehe `Extras > Zeitrahmen` erstellten Zeitrahmen zuweisen
Externe ID | ID für ein Fremdprogramm
DAVINCI-ID   | eindeutige DAVINCI-ID, wird automatisch erzeugt

## Ressourcen

![Stammdaten Ressourcen](/assets/images/StammdatenRessourcen.png)

In DAVINCI können jeder Veranstaltung bzw. jedem Termin beliebige Ressourcen, z.B. Audiogeräte, Beamer, Werkzeugkisten usw. zugeordnet werden. Ressourcen werden in der Ansicht ``Stammdaten > Ressourcen`` eingetragen. Logisch gesehen sind Klassen, Lehrer und Räume spezielle Ressourcenarten, die durch eine Veranstaltung bzw. einen Termin für die zeitliche Verplanung zusammengefasst werden. Ausführliche Darstellung der Ressourcenplanung erhalten Sie in der Dokumentation für den [DAVINCI RESSOURCENPLAN](/davinci-ressourcen/README.md).

## Schüler

![Stammdaten Schüler](/assets/images/StammdatenSchüler.png)

!!! info "Hinweis"

    Die Liste ``Schüler`` besitzt als einzige keine Spalte ``Kürzel``. Einträge in der dieser Liste sollten daher wenigstens die Angaben ``Vorname`` und ``Nachname`` erhalten. 

In der Ansicht ``Stammdaten > Schüler`` erfassen Sie Ihre Schüler. Über die Spalte "Klasse" oder "Stufe" sollte jeder Schüler einer Klasse oder einer Stufe zugeordnet werden. Sollten Sie mit DAVINCI KURSPLAN arbeiten, sollten Sie die Schüler in der Ansicht ``Kursplan > Schüler`` eingeben, da Sie dort gleichzeitig deren Fachwahl erfassen können. Sie können Schüler einer Veranstaltung zuweisen. In der gymnasialen Oberstufe wird im ersten Schritt die Fachwahl der Schüler erfasst, dann das Kursangebot erstellt und dann werden die Schüler den Kursen zugewiesen. Wie Sie zur Kursplanung, d.h. zur Planung mit Schülerkursen vorgehen, erfahren Sie im [DAVINCI KURSPLAN](/course-plan/README.md).

Spalte | Beschreibung
--------|-------------------------------------------
Nachname | Nachname
Vorname | Vorname
Mittelname | Mittelname
Personen-Nr. | Personennummer, für DAVINCI ohne Relevanz
Klasse | Klasse bzw. Jahrgang, zu dem der Schüler gehört
Stufe | Stufenangabe
Geschlecht | Geschlecht des Schülers. Diese Angabe besitzt keine unmittelbare Relevanz für die Terminplanung. Sie wird aber benötigt, um im Ausdruck sowie im HTML-Export der Stundenpläne der Oberstufenschüler eine Anrede, z.B. "Frau", ergänzen zu können. 
Tutor | Lehrer, der dem Schüler ggf. als Tutor zugeordnet wurde
E-Mail | E-Mail-Adresse, wird für E-Mail-Benachrichtigung verwendet
Mobil | Telefonnummer für das Mobiltelefon, wird für SMS-Benachrichtigung verwendet
Schule | Schulnummer
Postleitzahl | Postleitzahl
Ort | Ort
Straße | Straße
Bemerkung| Bemerkungstext
Benutzername | Kennung des Schüler zur Identifzierung des Schülerplans im Serverbetrieb
Externe ID |  Externe ID für Fremdprogramm
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt
MAGELLAN-ID | Eindeutige ID für den MAGELLAN Abgleich
Nicht statistikrelevant | dieser Schüler wird für Statistiken nicht exportiert
Kein MAGELLAN Abgleich  | dieser Schüler wird beim Datenaustausch mit MAGELLAN nicht importiert oder exportiert
Inaktiv         | Dieser Schüler ist nicht mehr aktiv, weil er z.B die Schule verlassen hat
Keine Fachwahl | Für diesen Schüler wird in DAVINCI keine Fachwahlüberprüfung durchgeführt

!!! info "Hinweis"

    Ein Schüler wird über seine ID identifiziert. Daher können auch zwei Schüler mit gleichem Vornamen/Nachnamen eingetragen werden. Verwenden Sie das Feld ``Personen-Nr.`` zur Unterscheidung gleichnamiger Schüler.

## Stundentafeln

![Stammdaten Stundentafeln](/assets/images/StammdatenStundentafel.png)

In der Stammdatenliste "Stundentafeln" legen Sie klassen- bzw. jahrgangsbezogene Fächerlisten an, welche die offizielle Unterrichtsverpflichtung der zugehörigen Klassen- bzw. Jahrgangsstufen wiederspiegeln. Sie bilden die Vorlage für die Veranstaltungslisten der Klassen. In der Spalte "Stundentafel" der Ansicht `Stammdaten > Klassen` können Sie jeder Klasse eine Stundentafel zuweisen. 

In der Ansicht `Stundenplan` können Sie mit `Stundenplan > Neu > Aus Stundentafel erzeugen` bzw. `Veranstaltung > Neue Veranstaltung > Aus Stundentafel erzeugen` die Fächer der Stundentafel inkl. Stundenvorgabe als Unterrichtsverteilung übernehmen. Die Stundenvorgabe kann von Ihnen in der Unterrichtsverteilung abgeändert werden, also beispielsweise um eine entsprechende Stundenzahl reduziert werden, weil Ihnen Fachlehrer fehlen. Die Differenz aus der durch die Stundentafel vorgegebenen Stundenzahl und der tatsächlich verplanten Stundenzahl wird in DAVINCI als Soll-Ist-Statistik erfasst und dient so als Grundlage für die elektronische Landesstatistik.

!!! info "Hinweis"

    Sie können das Stundentafel-Fenster auch in der Ansicht "Stundenplan" über das Zusatzfenster ``Summen > Stundentafel`` öffnen. Wenn Sie dort oder in der Stammdaten-Ansicht von einer Klasse zur anderen wechseln, wird der Inhalt des Stundentafel-Fensters automatisch angepasst. 

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel der Stundentafel
Bezeichnung | Freies Textfeld
Fächer | Bearbeiten Sie die Fächer in dem Sie auf die ``…`` Schaltfläche klicken, weitere Informationen dazu erhalten Sie im Folgenden
Stufe | Jahrgangsstufe
Bildungsgang | Verknüpft mit dem Schlüsselverzeichnis "Bildungsgänge"
Profil | Freies Feld (schulspezifisch)
Team | Teams zu denen die Stundentafel gehört
Externe ID | ID für Fremdprogramme
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

Geben Sie mit ``Neu`` oder der Taste ``EINFG`` neue Schlüssel ein. Mit ''Löschen'' können Sie Schlüssel wieder löschen. 

!!! info "Hinweis"

    Einige Spalten sind standardmäßig ausgeblendet. Wenn Sie auf `Spalten ein-/ausblenden` klicken, werden Ihnen die nicht sichtbaren Spalten angeboten. Mit der Maus können Sie sie anklicken und auf die Spaltenposition in der Liste ziehen, um sie dauerhaft einzublenden.

## Teams

![Teams](/assets/images/teams.png)

In der Ansicht ``Stammdaten > Teams`` können Sie die Teams erfassen. In der Liste „Teams“ können Sie verschiedene organisatorische Gliederungen an Ihrer Schule oder Hochschule erfassen. Dies können z.B. Abteilungen berufsbildender Schulen, verschiedene Schulformen an einer integrierten Gesamtschule oder verschiedene Fachbereiche an einer Hochschule sein. 
Für jedes Team können Sie in der Spalte "E-Mail" die Kontakt-Email des Teams eintragen. Über diese E-Mail können die Teams benachrichtigt werden.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Teams
Bezeichnung | Bezeichnungstext
E-Mail | E-Mail Adresse des Teams, falls dieses eine eigene Adresse hat
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

!!! info "Hinweis"

    Wenn Sie im Dialogfenster ``Extras > Optionen`` unter ``Plan > Einstellungen > Teamfilter`` die Option ``Fächer in Veranstaltungsliste und Stundentafeln nach Teamzugehörigkeit filtern`` markiert haben, werden in Stundentafeln und der Veranstaltungsliste der Klassen nur die Fächer des Teams und die Fächer ohne Teamzugehörigkeit angezeigt. Voraussetzung dafür ist, dass Sie bei der Stundentafel bzw. Klassen in der Spalte "Team" eine Teamzughörigkeit festgelegt haben.

## Zeiträume

Diese Registerkarte ist standardmäßig ausgeblendet, da Eintragungen in DAVINCI 6 keine Bedeutung finden.
