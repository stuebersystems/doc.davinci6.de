# Das Stammdatenfenster

Die Stammdaten sind die grundlegenden Daten Ihres Plans bzw. Ihrer Schule. Hier erfassen Sie Klassen, Lehrer, Fächer, Räume etc.. 

Öffnen Sie den Programmbereich "Stammdaten" über die Navigationsleiste links unten, indem Sie den Aufruf "Stammdaten" wählen. Die Navigation darüber passt sich dem gewählten Bereich an und führt die Stammdatenregister auf.

![Stammdaten-Fenster](/assets/images/Stammdaten02.png)

Das Arbeitsfenster besteht aus Listen, auf denen jeweils Einträge zu einer bestimmten Datenkategorie (Stammdatenregister) angelegt werden können.

Bei den Datenkategorien die hier erfasst werden können, handelt es sich namentlich um Klassen, Lehrer, Räume, Fächer,Stundentafeln, Aufsichtsbereiche, Perioden, Gebäude, Teams, Ressourcen, Schüler.

!!! info "Hinweis"

    Unter `Extras > Optionen > Ansicht` können einzelne Stammdatenbereiche ausgeblendet werden. Ungenutzte Stammdatenregister werden so nicht mehr angezeigt und die Ansicht ist übersichtlicher.

![Ansicht](/assets/images/Optionen.Ansicht.Stammdaten.png)

Da die Stammdaten-Ansichten aus Listen bestehen, sollten Sie den Abschnitt [Mit Listen arbeiten](/davinci-stundenplan/mit-listen-arbeiten.md) lesen, um sich mit den Ansichts- und Sortierungsoptionen vertraut zu machen.

Um Stammdaten eintragen, bearbeiten oder löschen zu können, müssen Sie darauf achten, dass der Aufruf `Liste bearbeiten` aktiv ist.

![Liste bearbeiten](/assets/images/stundenplan/bild001.png)

Die Stammdatenregister bestehen aus verschiedenen Spalten. Neue Einträge in den Stammdaten benötigen wenigstens eine Eingabe im Feld "Kürzel". Jedes Kürzel ist eindeutig und kann nur einmal eingegeben werden. 

!!! info "Hinweis"

    Je nachdem, ob Sie unter `Extras > Optionen > Einstellungen` die Option `Bei Kürzel-Eingabe Groß- und Kleinschreibung beachten` markiert haben, wird die Groß- bzw. Kleinschreibung beachtet.

## Stammdaten eingeben

Geben Sie im Stammdaten-Fenster Jahrgänge, Lehrer, Räume, Fächer usw. ein. Gehen Sie zur Eingabe der Stammdaten möglichst in folgender Reihenfolge vor:

1. Teams eingeben
2. Gebäude eingeben
3. Perioden eingeben
4. Räume eingeben
5. Aufsichtsbereiche eingeben
6. Fächer eingeben
7. Stundentafeln eingeben
8. Lehrer eingeben
9. Klassen eingeben

## Teams

![Teams](/assets/images/stundenplan/bild002.png)

Wenn Sie in Ihrer Schule verschiedene organisatorische Gliederungen (Teams, Abteilungen bzw. Fachbereiche) haben, können Sie hier Kürzel und Bezeichnung des jeweiligen Teams bzw. des Fachbereiches eingeben. Für jedes Team können Sie in der Spalte "E-Mail" die Kontakt-Email des Teams eintragen. Über diese E-Mail können die Teams benachrichtigt werden.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Teams
Bezeichnung | Bezeichnungstext
E-Mail | E-Mail Adresse des Teams, falls dieses eine eigene Adresse hat
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

!!! info "Hinweis"

    Wenn Sie im Dialogfenster `Extras > Optionen` unter `Plan > Einstellungen > Teamfilter` die Option `Fächer in Veranstaltungsliste und Stundentafeln nach Teamzugehörigkeit filtern` markiert haben, werden in Stundentafeln und der Veranstaltungsliste der Klassen nur die Fächer des Teams und die Fächer ohne Teamzugehörigkeit angezeigt. Voraussetzung dafür ist, dass Sie bei der Stundentafel bzw. Klassen in der Spalte "Team" eine Teamzughörigkeit festgelegt haben.

## Gebäude

![Stammdaten Gebäude](/assets/images/stundenplan/gebäude.png)

In dieser Registerkarte können Sie die einzelnen Außenstellen oder unterschiedliche Gebäude Ihrer Schule eingeben, soweit der Unterricht nicht in nur einem Gebäude stattfindet. Zusätzlich zu Kürzel und Bezeichnung können Sie hier die einzelnen Wegzeiten vom Hauptgebäude zu dem jeweiligen Gebäude eintragen. Die DAVINCI Automatik achtet bei der Verplanung der Termine darauf, dass Pausen bzw. Freistunden für den Weg zwischen dem Hauptgebäude den Außenstelle vorgesehen werden.

Im Stundenplan werden Terminkonflikte bei der Raumplanung, die durch nicht ausreichende Wegzeiten zwischen Haupt- und Nebengebäuden entstehen, mit einem Warnsymbol rechts unten im Termin markiert. 

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel des Gebäudes
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt
Bezeichnung | Bezeichnung des Gebäudes
Wegzeit | Wegzeit in Minuten von einem Nebengebäude zum Hauptgebäude
Campus | Gebäude können wiederum in ``Campus`` zusammengefasst werden. Dazu müssen Sie in der Ansicht ``Stammdaten > Campus`` diese eingeben.

## Perioden

![Stammdaten Perioden](/assets/images/stundenplan/perioden.png)

Wenn Sie als Schule mit wochenbezogenen Veranstaltungen  unterrichten, können Sie auf der Registerkarte „Perioden“ häufig benutzte, individuelle Wochenschemata für wiederkehrenden Unterricht anlegen.

Spalte | Inhalt
--|--
Kürzel | Kürzel der Periode
Bezeichnung | Bezeichnungstext
Faktor | Wert wird für die Umrechnung von Wochenstunden auf Wochenmittelwerte verwendet
Wochen | Unterrichtswochenmuster
Wochenanzahl   | Anzahl der Unterrichtswochen, errechnet sich automatisch aufgrund der Spalte "Wochen")
Team   | ordnet die Periode einem Team zu
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

Eine Periode stellt eine Teilmenge aller Unterrichtswochen eines Planungszeitraums dar. Das Anlegen von Perioden ist immer dann sinnvoll, wenn Sie mit wiederkehrenden Unterricht planen möchten, der nicht in allen Unterrichtswochen in gleicher Weise stattfindet oder eine Klasse nur in bestimmten Wochen unterrichtet werden soll (z.B. Turnusunterricht, Blockklassen).

Durch das Zuweisen einer Periode können Sie festlegen, dass ein wiederkehrender Termin nicht in allen, sondern nur in ausgewählten Unterrichtswochen stattfinden soll. So besteht z.B. die Möglichkeit anzugeben, dass ein bestimmter Unterricht nur im 1. Halbjahr oder in den ungeraden Kalenderwochen stattfindet. Daraus ergibt sich womöglich der Bedarf, dass anderer Unterricht komplementär dazu im 2. Halbjahr oder in den geraden Kalenderwochen verplant werden soll. Damit Sie diese und andere Wochenschemata für die Unterrichtsplanung einsetzen können, können Sie in den Stammdaten jeweils eine Periode mit den zugehörigen Kalenderwochen anlegen.

Neben der Möglichkeit, Perioden einzelnen Veranstaltung oder Terminen zuzuweisen, können Sie eine Periode auch in den Stammdaten einer Klasse zuweisen. Die Zuweisung erfolgt in der Spalte "Periode". Alle wiederkehrenden Unterrichtstermine dieser Klassen finden dann standardmäßig nur in den vorgegebenen Kalenderwochen der ausgewählten Periode statt.

Die wesentliche Aufgabe beim Anlegen einer Periode besteht darin, zu definieren, welche Kalenderwochen diese Periode umfassen soll. Dazu dient das Dialogfenster "Wochen bearbeiten", das Sie über die Schaltfläche mit den drei Pünktchen im Spaltenfeld "Wochen" aufrufen können. Die Nummern bei "Unterrichtswochen" stehen für die Kalenderwochen einer Plandatei. 

![Wochen bearbeiten](/assets/images/stundenplan/perioden.wochen.bearbeiten.png)

Die eingeklammerten Nummern kennzeichnen die Kalenderwochen, die unter `Plan > Eigenschaften > Statistik` vom Unterricht ausgenommen wurden. Sie stehen nicht mehr als Unterrichtswochen zur Verfügung.

Mit den Kontrollkästchen neben den nicht eingeklammerten Nummern legen Sie fest, welche Kalenderwochen die Periode beinhaltet. Setzen Sie den Haken im Kontrollkästchen um die nebenstehende Kalenderwoche hinzuzufügen. Entfernen Sie den Haken um die zugehörige Kalenderwoche wieder zu löschen.

Mit den fünf Schaltflächen neben dem Bereich "Unterrichtswochen" können Sie die Auswahl der Kalenderwochen teilweise automatisieren. 

Schaltfläche | Wofür?
--|--
`Alle Wochen löschen` | Klicken Sie auf diese Schaltfläche, um die Haken aus allen Kontrollkästchen zu entfernen. `Alle Wochen markieren` | Klicken Sie auf diese Schaltfläche, um Haken vor allen Kalenderwochen zu setzen.
`Jede 1. Woche markieren` | Mit dieser Schaltfläche erreichen Sie, dass jede erste Woche ausgehend von der ersten angezeigten Kalenderwoche markiert wird.
`Jede 2. Woche markieren` | Mit dieser Schaltfläche bewirken Sie, dass jede zweite Woche ausgehend von der zweiten angezeigten Kalenderwoche aktiviert wird.  
`Wochen markieren` | Diese Schaltfläche markiert alle Kalenderwochen entsprechend Ihrer Eingaben in den Feldern `Alle X Wochen` und `Jede X. Woche`. Die Angabe im erstgenannten Feld legt fest, in welchem Wochenabstand die Markierung erfolgt. Mit der Eingabe im letztgenannten Feld definieren Sie ausgehend von welcher Kalenderwoche die Markierung vorgenommen wird. Auf diese Weise können Sie komplexere Wochenschemata automatisch eintragen lassen. Mithilfe dieser Funktion können Sie bestimmte häufig auftretende Wochenmuster sehr leicht zu erzeugen, z.B. eine Periode, die jede 4. Woche ausgehend von der ersten Kalenderwoche umfasst. Klicken Sie `OK` und die Nummern der ausgewählten Kalenderwochen werden nun im Feld "Wochen" der zugehörigen Periode eingetragen.

## Räume

![Stammdaten Räume](/assets/images/stundenplan/stammdaten.Räume.png)

Geben Sie in der Registerkarte „Räume“ die Räume ein. Sie haben des Weiteren die Möglichkeit, diese Räume genauer zu spezifizieren, d.h. sie unter „Raumart“ z.B. als Fachräume zu bezeichnen und später auf der Registerkarte „Fächer“ den einzelnen Fächern zuzuordnen. Die Raumarten können unter `Extras > Schlüsselverzeichnisse > Raumarten` frei editiert werden. Außerdem können Sie die Zuständigkeit der Abteilungen genau bezeichnen, bei Außenstellen das jeweilige Gebäude angeben und die Kapazität des einzelnen Raumes eintragen. Unter „Betreuer“ kann ein Raumbetreuer eingegeben werden. Dieser erscheint in DAVINCI Look und kann im Raumplan mit ausgedruckt werden.

Spalte | Inhalt
--|--
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

## Aufsichtsbereiche

![Aufsichtsbereiche](/assets/images/stundenplan/stammdaten.aufsichtsbereiche.png)

Aufsichtsbereiche definieren Sie mit einem Kürzel, z.B. Hof 1, Hof 2, Flur 1, Flur 2, usw. Im Dialogfenster „Räume“ können Sie dann diejenigen Räume auswählen, die in oder an dem definierten Aufsichtsbereich liegen. So können Sie bei der Aufsichtsplanerstellung berücksichtigen, welcher Lehrer vor der Pause in welchem Raum ist, d.h. die Aufsichten so besetzen, dass Wegzeiten möglichst gering gehalten werden.

Die Aufsichtsbereichsplanung selbst erfolgt für jeden Bereich unter `Stundenplan > Aufsichtsplan`.

Spalte | Inhalt
--|--
Kürzel | Kürzel des Aufsichtsbereichs
Bezeichnung |  Bezeichnungstext
Zeitrahmen |  Zeitrahmen für die Aufsichten, siehe `Extras > Zeitrahmen`
Räume |  die an den Aufsichtsbereich angrenzenden Räume, Stammdatenregister "Räume"
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

## Fächer

![Stammdaten Fächer](/assets/images/stundenplan/Stammdaten.Fächer.png)

Die Fächer müssen mit Kürzel und optional mit Langnamen eingegeben werden. Bei der Oberstufenstundenplanung können Sie den Fachstatus, z.B. Grund- oder Leistungskurs, bestimmen. Unter „Schlüssel“ können Sie jedem Fach einen Statistikschlüssel zuweisen. Für die Jahresstatistik wird dann dieser Statistikschlüssel anstelle des Kürzels verwendet.


Spalte | Inhalt
--|--
Kuerzel | Fachkürzel
Bezeichnung |  Freies Bezeichnungsfeld
Kategorie | In der Spalte "Kategorie" (weitere Informationen im Abschnitt Kursplanung) machen Sie Angaben, die von der Fachwahlüberprüfung benutzt werden
Aufgabenbereich | In der Spalte "Aufgabenbereich" machen Sie Angaben, die von der Fachwahlüberprüfung benutzt werden
Farbe | Kann im Stundenplan eingeblendet werden, siehe `Plan > Eigenschaften> Stundenplan > Planeinträge`
Hintergrund | Macht die gewählte Farbe im Stundenplan als Hintergrundfarbe sichtbar
Bemerkung | Bemerkungstext
Fachstatus | siehe ``Extras > Schlüsselverzeichnisse > Fachstatus``
Team | Teamzughörigkeit des Fachs, siehe ``Stammdaten > Teams``
Zeitkonto | Konto auf das Stunden des Fachs verbucht werden, siehe ``Extras > Schlüsselverzeichniss > Lehrer Soll-Schlüssel``
Fachräume | Fächern, die in Fachräumen unterrichtet werden, kann ein bestimmter Raum oder eine Auswahl an Räumen zugeordnet werden. Diese Räume werden beim Kopieren der Stundentafel automatisch in die Raumvorgabeliste des jeweiligen Fachs übernommen.
Vertretung | Vertretungsoptionen ``Präsenz``, ``Keine Vertretung`` und ``keine Anrechenstunden``
Schlüssel | Bundeslandspezifische Kennzeichnung des Fachs
Details | Zusätzliche Optionen für den MAGELLAN Abgleich `nicht statistikrelevant` und `kein MAGELLAN-Abgleich`


!!! info "Hinweis"

    Mit `Bearbeiten > Inhalte kopieren` und `Bearbeiten > Inhalte einfügen` können Sie die Fachräume eines Fachs auf andere Fächer kopieren.

!!! warning "Wichtig"

    Im Gegensatz zu anderen Stundenplanprogrammen brauchen Sie für die Kurse D1, D2, d1, d2 usw. lediglich das Fach „D“ einzugeben, d.h. die Kurse selbst brauchen nicht in den Stammdaten definiert zu werden. Sie können in der Veranstaltungsliste in der Spalte Fach dann die o.g. Kursbezeichnungen eingeben.

!!! info "Hinweis"

    In der Spalte „F“ können Sie eine Farbe angeben, in der ein Termin dieses Faches im Planungsfenster dargestellt werden soll. Wenn Sie das Kästchen in der Spalte „H“ anklicken, wird der Hintergrund des Fachtermins farbig dargestellt. Auf diese Weise können Sie mit zwei verschiedenen Arten der farbigen Darstellung arbeiten. Welche Art der farbigen Darstellung für die Eintragung in Spalte „F“ gewählt wird, hängt davon ab, was Sie unter `Extras > Optionen > Termineinträge > Farbe anzeigen als` eingetragen haben. Damit überhaupt eine Fachfarbe angezeigt wird, müssen Sie jedoch zunächst hier die entsprechende Auswahl bei `Farbe für Termine im Plan“` treffen.

## Stundentafeln

![Stammdaten Stundentafeln](/assets/images/StammdatenStundentafel.png)

In der Registerkarte "Stundentafeln" legen Sie klassen- bzw. jahrgangsbezogene Fächerlisten an, d.h. die Fächer mit den dazugehörigen Sollstundenzahlen, welche die offizielle Unterrichtsverpflichtung der zugehörigen Klassen- bzw. Jahrgangsstufen wiederspiegeln. Sie bilden die Vorlage für die Veranstaltungslisten der Klassen. In der Spalte "Stundentafel" der Registerkarte "Klassen" können Sie jeder Klasse eine Stundentafel zuweisen.

### So können Sie die Fächer einer Stundentafel übernehmen

Klicken Sie auf eine Stundentafel. Klicken Sie auf `Bearbeiten > Inhalte kopieren`. Klicken Sie dann auf die Stundentafel, in die Sie die Fächer übertragen möchten. Klicken Sie dort auf ` Bearbeiten > Inhalte einfügen`. Die Fächer werden in die Stundentafel übertragen.

Spalte | Inhalt
--------|-------------------------------------------
Kürzel | Kürzel der Stundentafel
Bezeichnung | Freies Textfeld
Fächer | Bearbeiten Sie die Fächer in dem Sie auf die ``…`` Schaltfläche klicken
Stufe | Jahrgangsstufe
Bildungsgang | Verknüpft mit dem `Schlüsselverzeichnis > Bildungsgänge`
Profil | Freies Feld (schulspezifisch)
Team | Teams zu denen die Stundentafel gehört
Externe ID | ID für Fremdprogramme
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

Klicken Sie auf die Schaltfläche ``…`` in der Spalte „Fächer“. Es öffnet sich das Dialogfenster „Stundentafel“.
![Stammdaten Stundentafeln](/assets/images/stundenplan/stammdaten.stundentafel.öffnen.png)

Klicken Sie auf `Neues Fach`, um ein neues Fach hinzuzufügen. Tragen Sie unter „Soll“ die vorgeschriebene Sollstundenzahl ein. Zudem können Sie eine Unterrichtsart, -kategorie, -form und einen Lehrbereich je Fach zuweisen.  Die Spalte Wertfaktor wird z.B. für die Umsetzung des Hamburger Lehrerarbeitszeitmodells benötigt. Der Wertfaktor wird bei der Berechnung der Lehrerstunden wie folgt berücksichtigt: Summe = Dauer/W x Lehrerfaktor x Wertfaktor Damit der Wertfaktor auch bei den entsprechenden Summenbildungen berücksichtigt wird, müssen Sie unter `Extras > Zeitrahmen` auf der Registerkarte „Statistik“ die Option `Lehrer - Ist mit Wertfaktoren aus Stundentafel` anklicken. In der Spalte „Bemerkung“ können Sie eine beliebige Bemerkung erfassen. Klicken Sie wieder auf oder die `Pfeil-Ab-Taste`, um in der nächsten Zeile ein neues Fach einzugeben. Verfahren Sie so mit allen Fächern der Stundentafel.

Spalte| Inhalt
--|--
Angleichung| Angleichung der Stundenzahl an dieser Schule. Der Eintrag in der Spalte "Soll (W)" der Veranstaltungsliste ist die Summe aus den Werten "Soll" und "Angleichung" der Stundentafel
Bemerkung |Freitext für Bemerkung
Differenz | 
Doppelstd |Anzahl der Doppelstunden für die Automatik, z.B. ``1-2`` gibt der Automatik mindestens eine und höchstens zwei Doppelstunden vor
Fach| Kürzel des Fachs
Fachstatus| Fachstatus z.B. "1. Prüfungsfach" (nur für Oberstufe) gemäß `Extras > Schlüsselverzeichnis > Fachstatus`, standardmäßig ausgeblendet
Gruppe | Gruppe
Kategorie | Veranstaltungskategorie, siehe `Plan < Schlüsselverzeichnis > Veranstaltungskategorien`. Eine Besonderheit ist, dass diese Eigenschaft auf die Klassen mit dieser Stundetafel übernommen wird, d.h. Sie können hier zentral die Eigenschaft für alle Klassen mit dieser Stundentafel einstellen.
Lehrbereich| Lehrbereich gemäß `Extras > Schlüsselverzeichnis > Lehrbereiche`', standardmäßig ausgeblendet
Pflichtkurse| Anzahl der Pflichtkurse (nur für Oberstufe)
Schlüssel | Fachschlüssel siehe `Stammdaten > Fächer > Schlüssel`
Soll| Stundenanzahl, mit der dieses Fach unterrichtet werden soll
Soll 1|
Soll 2|
Soll 3|
Soll 4|
Sollkonto | Stundenanzahl, mit der dieses Fach unterrichtet werden soll über eine Zeitspanne die über eine Planungsdatei hinausgeht (BFW)
Stufensumme |
Termine| Termine, z.B. ``2-2-1`` für zwei Doppelstunden und eine Einzelstunde, entspricht der Angabe "Termine" in der Veranstaltungsliste
Unterrichtsform| Unterrichtsform gemäß ``Extras > Schlüsselverzeichnis > Unterrichtsformen``, standardmäßig ausgeblendet
Unterrichtsart| Unterrichtsart gemäß ``Extras > Schlüsselverzeichnis > Unterrichtsarten`', z.B. für die Unterscheidung Leistungs- und Grundkurse in der Oberstufe
Wertfaktor| Wertfaktor für die Statistik mit Wertfaktoren, standardmäßig ausgeblendet
Wiederholung | Periodisch/Einmalig


!!! info "Hinweis"

    Einige Spalten sind standardmäßig ausgeblendet. Wenn Sie auf `Spalten ein-/ausblenden` klicken, werden Ihnen die nicht sichtbaren Spalten angeboten. Mit der Maus können Sie sie anklicken und auf die Spaltenposition in der Liste ziehen, um sie dauerhaft einzublenden. Alternativ können Sie dazu auch das Sternchen-Symbol links oben in der Stundentafel tabell nutzen.

## Lehrer

![Stammdaten Lehrer](/assets/images/stundenplan/stammdaten.lehrer.png)

In der Registerkarte "Lehrer" erfassen Sie die Lehrkräfte, die an Ihrer Schule unterrichten.

!!! info "Hinweis"

    Den Lehrerplan können Sie direkt aus der Liste "Lehrer" heraus aufrufen. Klicken Sie dazu einen Lehrer an und wählen `Start > Gehe zu Stundenplan`, `Rechtsklick > Gehe zu Stundenplan` oder benutzen Sie die Funktionstaste `F9`.

!!! info "Hinweis"

    Über `Stammdaten > Bearbeiten > Lehrer-Zeitkonto bearbeiten` öffnen Sie das Zeitkonto-Fenster für den aktuellen Listeneintrag. Dort können Sie die Ermäßigungs- und Mehrarbeitsstunden eingeben.

Spalte | Inhalt
--|--
Kürzel | Lehrer werden mit Ihrem Kürzel eingegeben
Titel | Titel des Lehrers
Nachname | Nachname des Lehrers
Mittelname | Zweitname
Vorname | Vorname des Lehrers
Farbe | Kann im Stundenplan eingeblendet werden, siehe "Plan > Einstellungen > Stundenplan` > Planeinträge"
Symbol | Hier können Sie den Lehrern von STÜBER SYSTEMS mitgelieferte Symbole zuweisen. Um ein Bild/Symbol zu laden, gehen Sie über die  `Rechte-Maustaste > Laden`. Die Symbole können im Plan angezeigt werden. Damit diese sichtbar sind, müssen Sie unter `Plan > Einstellungen > Stundenplan > Planeinträge > Lehrersymbole anzeigen` aktiviert haben. 
Geschlecht | Geschlecht des Lehrers
Geb. Datum | Geburtsdatum
Fächer | Um die Fächer einzutragen, die der Lehrer unterrichtet, klicken Sie auf die Spalte „Fächer“ in der Zeile des entsprechenden Lehrers. Im Dialogfenster „Fächer“ wählen Sie aus den verfügbaren Fächern diejenigen aus, die der entsprechende Lehrer unterrichtet und übertragen sie entweder per Drag&Drop oder indem Sie sie markieren und dann auf `Hinzufügen` klicken in das Feld „gewählte Fächer“. Diese erscheinen dann auf der Registerkarte in der Spalte „Fächer“.
Teams | Sollten Ihre Lehrer Teams bzw. Fachbereichen angehören, so können Sie diese im Dialogfenster „Teams“ auswählen und zuordnen, indem Sie auf Teams klicken, das entsprechende Team im Feld „Verfügbare Teams“ markieren und dann auf `Hinzufügen` klicken. Sie können auch per `Drag&Drop` die Teams aus `Verfügbare Teams` in „Gewählte Teams“ ziehen. Die ausgewählten Teams erscheinen auf der Registerkarte unter Teams.
E-Mail | E-Mail des Lehrers
Mobil | Handynummer des Lehrers
Schule | Schulnummer oder Mandantennummer aus MAGELLAN
Bemerkung | Freies Bemerkungsfeld
Details | Zusätzliche Optionen für den MAGELLAN Abgleich ("nicht statistikrelevant" und "kein MAGELLAN Abgleich") und die Option "inaktiv"
Zeitrahmen | siehe "Extras > Zeitrahmen" erstellten Zeitrahmen zuweisen
Benutzername | Benutzername für den Serverbetrieb, kennzeichnet den Plan des Benutzers/Lehrers
Personalnr. | Personalnummer
Stundensatz | Stundensatz, z.B. 50 für 50EUR, kann in Zeitkonto mit "Normierter Stunde" multipliziert werden (siehe `Plan > Eigenschaften > Statistik`)
Eintritt / Austritt | Eintritts- und Austrittsdatum
Externe ID | ID für ein Fremdprogramm
ID   | Eindeutige DAVINCI-ID, wird automatisch erzeugt

### Die Lehrer Soll-Berechnung

Bei der Lehrereinsatzplanung mit DAVINCI wird für jeden Lehrer die Sollvorgabe benötigt, die sich aus den vom Kultusministerium vorgegebenen Pflichtstunden abzüglich Ermäßigungsstunden und zuzüglich Mehrstunden ergibt.

Zur Eingabe des Soll-Berechnungschemas stehen Ihnen die Lehrer-Soll-Berechnungsschlüssel zur Verfügung, die Sie unter `Extras > Schlüsselverzeichnisse > Lehrer-Soll-Schlüssel` eingeben können. Mit Hilfe dieser Schlüssel können Sie für jeden Lehrer die Pflichtstunden und die individuellen Ermäßigungs- und Mehrstunden angeben, aus denen sich die Sollvorgabe für jeden Lehrer berechnet. Die Sollberechnung kann nach Ihren Vorgaben beliebig detailliert sein.

![Schlüsselverzeichnis Lehrer-Soll-Schlüssel](/assets/images/Lehrer-Soll-Schlüssel.png)

#### Bundeslandspezifische Lehrer-Soll-Schlüssel importieren

Für verschiedene Bundesländer bzw. Schularten werden über die Landesanpassung diese Schlüssel schon vorinstalliert. In diesem Fall können Sie die Schlüssel über `Extras > Schlüsselverzeichnisse> Lehrer-Soll-Schlüssel` über den Aufruf "Importieren“ aus dem Ordner „Schlüssel“ importieren, um sich die Eingabearbeit zu ersparen.

So importieren Sie die Lehrer-Soll-Ist-Schlüssel

1. Öffnen Sie über `Extras > Schlüsselverzeichnisse > Lehrer-Soll-Schlüssel` das entsprechende Verzeichnis

![Lehrer-Soll-Schlüssel](/assets/images/stundenplan/stammdaten.lehrer.soll.schluessel.png)

2. Wählen Sie hier die Schalftläche `Importieren`.
3. Wählen Sie über die Schaltfläche `Datei auswählen` die Datei „LehrerSollIstSchlüssel <Bundesland>.txt“ im Ordner „Schlüssel“ und klicken Sie auf `OK`.
Sollten Sie in diesem Ordner keine Datei dieses Namens vorfinden, so sind für Ihr Bundesland keine Lehrer-Soll-Ist-Schlüssel verfügbar. Tragen Sie in diesem Fall die Schlüssel selbst ein.

![Lehrer-Soll-Schlüssel](/assets/images/stundenplan/stammdaten.lehrer.soll.schluessel01.png)

!!! info "Hinweis"

    Für bestimmte Bundesländer werden in DAVINCI bereits die offiziellen Schlüssel mitgeliefert. Sie können Sie im Dialogfenster `Lehrer-Soll-Schlüssel `über die Schaltfläche `Importieren` einlesen.

#### Soll-Berechnungsschlüssel eingeben

Im `Schlüsselverzeichnis > Lehrer-Soll-Schlüssel` erfassen Sie die entsprechenden Berechnungsschlüssel mit Kürzel, Bezeichnung und Typ ein. Der Typ (Operator) legt fest, wie DAVINCI den Schlüssel zu interpretieren hat.

Typ| Beschreibung
-|-
`P` | Pflicht- oder Regelstunden, die einem Lehrer aufgrund rechtlicher Vorgaben als allgemeine Unterrichtsverpflichtung auferlegt sind. Geben Sie in der Spalte „Stunden“ die betreffende Stundenzahl an. Einen Standardwert können Sie unter `Extras > Optionen > Einstellungen > Lehrer-Pflichtstunden standardmäßig` eingeben.
`-` | Ermäßigungsstunden, um welche die allgemeine Unterrichtsverpflichtung des Lehrers gemindert wird. Geben Sie in der Spalte „Stunden“ die betreffende Stundenzahl an.
`+` |Ergänzungs- bzw. Mehrarbeitsstunden, um welche die allgemeine Unterrichtsverpflichtung des Lehrers erhöht wird
`D` |Differenz aus Soll und Ist vom Vorjahr. Die Stundenanzahl in der Spalte „Stunden“ wird in beim Erstellen eines neuen Stundenplans über den Planvorbereitungsassistenten automatisch aus dem vorhergehenden Plan übernommen. Sie können sie hier auch manuell eingeben.
`A` |Stundenplan-Zeitkonto: In der Ansicht `Stammdaten > Fächer`  können Sie in der Spalte „Zeitkonto“ für einem Fach einen Lehrer-Soll-Schlüssel als Zeitkonto zuweisen. Die Stundenanzahl in der Spalte „Stunden“ wird in diesem Fall automatisch aufgrund des Lehrerplans berechnet.
`C` |Kalender-Zeitkonto: In der Ansicht „Kalender“ können Sie im Ereignis-Fenster bei „Zeitkonto“ einem Ereignis einen Lehrer-Soll-Schlüssel als Zeitkonto zuweisen. Die Stundenanzahl in der Spalte „Stunden“ wird in diesem Fall automatisch aufgrund des der entsprechenden Kalendereinträge berechnet.
`Leer` | Bemerkung, geht nicht in die Berechnung ein

#### Zeitkonto bearbeiten

Um das Zeitkonto zu bearbeiten, öffnen Sie im Stammdatenfenster die Registerkarte „Lehrer“. Klicken Sie in die entsprechende Zeile des Lehrer über `rechte Maustaste > Zeitkonto bearbeiten` oder `Strg+X`. Das Zeitkonto des Lehrers wird geöffnet und kann nun bearbeitet werden. 

![Zeitkonto bearbeiten](/assets/images/ZeitkontoBearbeiten.png)

Um das Dialogfenster zu bearbeiten, also diese Grunddaten um die individuellen Daten zu erweitern, wählen Sie die Schaltfläche `Neuer Schlüssel`. Es erscheint das Dialogfenster `Soll-Änderungsschlüssel auswählen` mit den Schlüsseln, die Sie im `Schlüsselverzeichnis > Lehrer-Soll-Schlüssel` eingetragen haben.

![Soll-Berechnung bearbeiten](/assets/images/stundenplan/stammdaten.lehrer.soll.schluessel02.png)

Markieren Sie den gewünschten Schlüssel und klicken Sie auf `Ok`. Die Soll-Berechnung für den Lehrer wird um ausgewählten Schlüssel erweitert. Für jeden Ermäßigungs- bzw. Mehrarbeitsgrund geben Sie in der Spalte `Stunden` die entsprechende Stundenzahl ein.

Möchten Sie einen Schlüssel verändern, seine Dauer verändern oder ihn durch einen anderen Schlüssel ersetzen, gehen Sie wie folgt vor:

Schlüssel löschen: Klicken Sie auf die zu löschende Zeile und dann auf `löschen`.

Stunden, Bemerkung ändern: Klicken Sie auf den entsprechenden Eintrag und ändern Sie die Eintragungen in den entsprechenden Spalten. 

#### Zeitkonto Summen

![Zeitkonto](/assets/images/stundenplan/stammdaten.lehrer.soll.schluessel03.png)

Im Zeitkonto des Lehrers werden noch folgende Werte ausgegeben/angezeigt:

Summe |Beschreibung
-|-
Soll | Summe aus Pflichtstunden, Ermäßigungs- und Mehrarbeitsstunden
Ist | Ist-Stunden des Lehrers, die sich aus den geleisteten Unterrichtsstunden entsprechend dem individuellen Stundenplan des Lehrers ergeben
Anrechnungen | Summe der Ermäßigungs- und Mehrarbeitsstunden
Diff (Ist+Anrch.-Pflicht) | Differenz zwischen Soll und Ist

#### Lehrer-Pfichtstundenwert standardmäßig vorbelegen

Die Pflichtstunden können Sie für jeden Lehrer gesondert festlegen. Einen Standardwert können Sie unter `Extras > Optionen > Einstellungen > Lehrer-Pflichtstunden standardmäßig` eingeben.

Alle Lehrer die Sie nun im Stammdatenfenster hinzufügen (neu erfassen), erhalten automatisch den eingetragenen Lehrer-Pfichtstundenwert standardmäßig. Lehrer die bereits im Stammdatenfenster gelistet sind, bleiben von diesem eingetragenen Standardwert unberührt.

![DAVINCI Optionen, Bereich "Einstellungen"](/assets/images/stundenplan/stammdaten.lehrer.soll.schluessel04.png)

## Klassen

In der Liste "Klassen" erfassen Sie die Klassen, die an Ihrer Schule unterrichtet werden. Für jeden Eintrag, den Sie in der Liste "Klassen" vornehmen, wird im Bereich `Stundenplan` ein eigener Klassenplan angelegt. 

!!! info "Hinweis"

    Den Plan einer bestimmten Klasse können Sie direkt aus der Stammdatenliste „Klassen“ heraus aufrufen. Klicken Sie dazu eine Klasse an und wählen `Start > Gehe zu Stundenplan`, `Rechtsklick > Gehe zu Stundenplan` oder benutzen Sie die Funktionstaste `F9`.

In der Stammdatenliste "Klassen" können Sie verschiedene Einstellungen vornehmen, die für die weitere Stundenplanung relevant sind. Außerdem stehen Ihnen zahlreiche Spalten zur Verfügung.

![Stammdaten Klassen](/assets/images/stundenplan/stammdaten.klassen.png)

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

# Ressourcen

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

## Zeiträume

Diese Registerkarte ist standardmäßig ausgeblendet, da Eintragungen in DAVINCI 6 keine Bedeutung finden.
