# Fachwahlen eingeben

Die Fachwahlen der Schüler werden in der Ansicht `Kursplan > Fachwahlen` erfasst und ggf. auch entsprechend der bundeslandspezifischen Fachwahlüberprüfung geprüft. Die Fachwahlüberprüfung erfolgt aufgrund des Fachwahlskriptes, das Sie bei jeder Klasse in der Ansicht `Stammdaten > Klassen` in der Spalte „Skript“ eingeben können.

## Angaben für den Jahrgang

![Liste der Klassen bzw. Jahrgänge](/assets/images/courseplan1.png)

In der Ansicht `Stammdaten > Klassen` weisen Sie die Klassen bzw. Jahrgänge mit Kurssystem (Modus
„Kurse“) aus und geben das Fachwahlskript an, nach dem die Fachwahl überprüft werden soll. Hinzu
kommen ggf. weitere Angaben, welche insbesondere für Fachwahlüberprüfungen notwendig sind, die mehrere
Halbjahre überprüfen, z.B. in Berlin. Welche Angabe das jeweilige Skript verlangt, können Sie in unserer Dokumentation ["Landesanpassung"](https://doc.la.stueber.de/) nachlesen.

!!! warning "Wichtig"

    In den „Kursplan“ Ansichten wird immer mit der Jahrgangsstufe (Spalte „Stufe“) gearbeitet. Wenn Sie z.b den Jahrgang 12 als eine Klasse „12“ eingegeben haben, sind Jahrgangstufe und Klasse gleichbedeutend. Wenn Sie den Jahrgang 12 in Klassen 12A, 12B, 12C aufteilen, werden alle Schüler dieser Klassen angezeigt. Sie wählen den Jahrgang aus, indem Sie über Plan | Auswahl eine Klasse auswählen. Angezeigt wird daraufhin der betreffende Jahrgang.

Die relevanten Spalten in der Ansicht `Stammdaten > Klassen`:

Spalte         | Beschreibung
-------------- | ------------
Modus          | Stellen Sie hier „Kurse“ ein, dann kann zwischen diesen Klassen in der Ansicht „Kursplan“ geblättert werden.
Stufe          | Jahrgangsstufe. In den Kursplan-Ansichten wird immer mit der Stufe gearbeitet, nicht mit Klassen.
Startjahr      | Startjahr der Klasse
Halbjahr       | Nummer des Halbjahres, in dem sich die Klasse aktuell für diesen Planungszeitraum befindet, d.h. 1, 2, 3, 4, 5, 6 (E1=1, E2=2....Q3=5, Q4=6). Aus Startjahr und Halbjahresindex errechnet sich, welche Fächer der Schüler in diesem Zeitraum bzw. in diesem Halbjahr belegt hat.
Schüler        | Die Schülerzahl wird automatisch berechnet.
Skript         | Geben Sie hier das Fachwahlskript an, das für die Fachwahlüberprüfung sorgt.
Verordnungstyp | Machen Sie hier ggf. weitere Angaben für das Fachwahlskript, z.B. „G8“ falls es sich um einen G8-Jahrgang handelt.

DAVINCI wird mit Fachwahlskripten für verschiedene Bundesländer und Schularten ausgeliefert. Ein Fachwahlskript hat die Dateiendung „.js“. Technisch gesehen ist ein Fachwahlskript eine JavaScript-Datei. Die ersten drei Buchstaben kennzeichnen das Bundesland, die Jahreszahl informiert über die Ausgabe des Skripts bzw. die zugrundeliegende Verordnung.

Namensanfang der Fachwahlskripte:

Abkürzung | Bundesland
--------- | ----------
BAY       | Bayern
BAW       | Baden-Württemberg
BER       | Berlin
BRA       | Brandenburg
BRE       | Bremen
HES       | Hessen
HAM       | Hamburg
NIE       | Niedersachen
NRW       | Nordrhein-Westfalen
MVP       | Mecklenburg-Vorpommern
SAA       | Sachsen-Anhalt
SAC       | Sachsen
SAR       | Saarland
SHL       | Schleswig-Holstein
RLP       | Rheinland-Pfalz
THÜ       | Thüringen

!!! info "Hinweis"

    Sollte für Ihr Bundesland bzw. Ihre Schulform kein Fachwahlskript vorhanden sein, fragen Sie bei uns nach, wir erstellen ständig neue Skripte gemäß neuer Verordnungen.

## Schüler eingeben

![Schüler im Jahrgang 12 mit vollständiger Blockung und Verteilung](/assets/images/courseplan2.png)

In der Ansicht `Kursplan > Schüler` werden alle Schüler des jeweiligen Oberstufenjahrgangs angezeigt. Sie können die Schüler (der Oberstufenjahrgänge) über den Befehl `Neu` eingeben. Alternativ dazu können Sie die Schüler auch in der Ansicht `Stammdaten > Schüler` eingeben. Dort werden Ihnen sämtliche Schüler aller Klassen angezeigt. In dieser Ansicht muss jeder Schüler in der Spalte „Klasse“ einem Jahrgang zugeordnet werden. Jahrgang und Klasse ist in diesem Fall gleichbedeutend. In der Ansicht `Kursplan > Schüler` wird der Schüler automatisch dem eingestellten Jahrgang zugeordnet. Setzen Sie MAGELLAN ein, können Sie u.a. auch Schülerdaten nach DAVINCI übergeben. Weitere Informationen finden Sie dazu im Abschnitt „Fachwahl aus MAGELLAN importieren“.

!!! info "Hinweis"

    In der Ansicht `Stammdaten > Schüler` können Sie die Schülerdaten mit Cut & Paste aus der Windows Zwischenablage übernehmen. Damit können Sie sehr schnell Ihre Schülerdaten aus Excel oder Word nach DAVINCI importieren.

Die Bedeutung der Zellen-Hintergrundfarben in der Ansicht `Kursplan > Schüler`:

Hintergrundfarbe | Bemerkung
---------------- | ---------
Keine Farbe      | Reine Fachwahl, d.h. es wurde noch kein Kurs zugeordnet
Grün             | Eine Fachwahl bzw. Kurswahl, der ein Kurs zugeordnet wurde 
Rot              | Bei einem oder mehreren Schülern liegt ein Konflikt vor, weil zwei Kurse eines oder mehrerer Schüler im gleichen Block liegen.
Grau             | Kurs mit zu geringer Teilnehmerzahl, siehe Spalte „Min. Schüler“ in der Ansicht `Kursplan > Kurse`.
Gelb             | Kurs mit zu hoher Teilnehmerzahl, siehe Spalte „Min. Schüler“ in der Ansicht `Kursplan > Kurse`.

## Fachwahl aus MAGELLAN importieren

Falls Sie MAGELLAN einsetzen, können Sie über den Befehl `Plan > Importieren und Exportieren` die
Schüler aus MAGELLAN übernehmen. Sie können die Schüler von MAGELLAN importieren, die
Fachwahlen eingeben und die Fachwahlen der Schüler dann wieder nach MAGELLAN exportieren.

![Datenimport von MAGELLAN starten](/assets/images/courseplan3.png)

!!! info "Hinweis"

    Die Fachwahleingabe ist auch in MAGELLAN möglich, allerdings ohne Stundenzahlen. Die Fachwahlen aus MAGELLAN können per Import nach DAVINCI übernommen werden. MAGELLAN verwendet zur Fachwahlüberprüfung das gleiche Fachwahlskript wie DAVINCI. DAVINCI bietet mehr Funktionen zur Fachwahleingabe. So dass Sie im Zweifelsfall die Fachwahl in DAVINCI erfassen sollten.

## Die Fachwahlen eingeben

![Die Fachwahlen eines Schülers](/assets/images/courseplan4.png)

In der Ansicht `Kursplan > Fachwahlen` können Sie für jeden Schüler dessen Fachwahl bestimmen. Wenn Sie bei der betreffenden Klasse des Schülers unter `Stammdaten > Klassen` in der Spalte „Skript“ das betreffende Fachwahlskript angegeben haben, wird die Eingabe entsprechend der durch das Skript geprüften Oberstufenverordnung überprüft. Der Name des jeweilige Skripts wird rechts oben in der Ansicht angezeigt. Ggf. werden Fehlermeldungen oben in der Ansicht angezeigt. Geben Sie die gewünschten Fächer ein und machen Sie die entsprechenden Angaben in den Spalten „Unterrichtsart“, „Fachstatus“ und „Stunden“.

Mit den „Markieren“ Schaltflächen können Sie alle Halbjahre eines Fachs markieren (Hintergrund Weiß) oder demarkieren (Hintergrund Grau). Indem Sie eine Halbjahreszelle in der Tabelle anklicken, können Sie einzelne Halbjahre markieren bzw. demarkieren. Das aktuelle Halbjahr “Q1“ (siehe Spalte „Halbjahr“ in der Ansicht „Stammdaten | Klassen“) ist durch die Hintergrundfarbe markiert. Im Bereich „Kurswahl“ ist der jeweils gewählte Kurs durch den hervorgehobenen Zellenrahmen markiert.

Die Fachwahlangaben:

Spalte | Bemerkung
------ | ---------
Fach           | Gewähltes Fach, das mit der Angabe von Unterrichtsart und „Fachstatus“ näher spezifiziert werden muss.
Kursnr         | Kursnummer
Unterrichtsart | Unterrichtsart, z.B. „LK“ oder „GK“ oder „Kurs“, abhängig von Fachwahlskript. Geben Sie die Unterrichtsarten ggf. über `Extras > Schlüsselverzeichnisse > Unterrichtsarten` ein. Ausschlaggebend sind dort die Angaben in der Spalte „Schlüssel“. Diese Angabe wird von der Blockungsautomatik mit der Vorgabe „Unterrichtsart“ in der Ansicht `Kursplan > Blöcke` abgeglichen.
Fachstatus     | Prüfungsfach z.B. „1PF“, „2PF“, „3PF“, „4PF“ oder „5PF“, abhängig von Fachwahlskript. Geben Sie die Fachstatus ggf. über `Schlüsselverzeichnisse > Fachstatus` ein. Ausschlaggebend sind dort die Angaben in der Spalte „Schlüssel“. 
Stunden        | Geben Sie hier die Stundenzahl ein. Sie wird automatisch auf die Halbjahre 1 bis 6 übertragen. Diese Angabe wird von der Blockungsautomatik mit der Vorgabe „Min. Std“ und „Max. Std“ in der Ansicht `Kursplan > Blöcke` abgeglichen. Sie können diese Angabe auch leer lassen.
Schwerpunkt    | Fachschwerpunkt. Geben Sie die Fachschwerpunkte ggf. über `Schlüsselverzeichnisse > Fachschwerpunkte` ein,
Details        | Textfeld für Details. Diese Angabe ist abhängig vom jeweiligen Bundesland.
Merkmal        | Textfeld für Merkmale. Diese Angabe ist abhängig vom jeweiligen Bundesland.
Pflichtkurse   | Anzahl der Pflichtkurse
Stunden        | Stundenanzahl des Kurses
E1…Q4          | Die Halbjahre der Oberstufe mit der jeweiligen Stundenanzahl, die sich aus der Spalte „Stunden“ ergibt. Sie können mit einem Mausklick in die betreffende Zelle Halbjahre für ein Fach markieren (weiß) oder demarkieren (grau). Wenn Sie unter „Stunden“ keine Stundenanzahl eingegeben haben, bleiben die Zellen der Tabelle leer.
Kurswahl      | Mögliche Kurse zur Fachwahl. Per Mausklick können Sie manuell einen anderen Kurs wählen. Der aktuelle Kurs ist durch die Rahmenfarbe hervorgehoben. Kurse mit gelbem Hintergrund können überschneidungsfrei gewählt werden, andernfalls hat der Schüler eine Überschneidung, d.h. zwei Kurse in einem Block.

## Fachwahl aufgrund von Stundentafeln erzeugen

Sie können sich viel Eingabearbeit ersparen, indem Sie mit Stundentafeln als Vorlagen arbeiten. Mit der Schaltfläche `Fachwahl erzeugen` können Sie für den aktuell markierten Schüler bzw. mehrere markierte Schüler oder alle Schüler des Jahrgangs die Fachwahl aufgrund einer Stundentafel, die als Vorlage dient, erzeugen.

![Die Fachwahlen eines Schülers](/assets/images/courseplan5.png)

Standardmäßig ist die Stundentafel des Jahrgangs eingestellt, Sie können aber auch eine andere wählen, wenn z.B. die Schüler nur aus einer von wenigen Fachkombinationen wählen können, weil an Ihre Schule nur diese Kombinationen angeboten werden.

## Stundentafeln als Fachwahlvorlage anlegen

![Liste der Stundentafeln](/assets/images/courseplan6.png)

Stundentafeln geben Sie in der Ansicht `Stammdaten > Stundentafeln` ein. Klicken Sie auf die Schaltfläche in der Spalte „Fächer“, um die Fächer der Stundentafel einzugeben.

![Fächerliste der Stundentafel](/assets/images/courseplan7.png)

Die Bedeutung der Stundentafelspalten:

Spalte         | Bemerkung
-------------- | ---------
Fach           | Gewähltes Fach, das mit der Angabe „Unterrichtsart“ näher spezifiziert werden muss.
Unterrichtsart | Unterrichtsart, z.B. „LK“ oder „GK“ oder „Kurs“, wird in die gleichnamige Spalte der Fachwahl übernommen. Geben Sie hier z.B. als Standardvorgabe „GK“ oder „Kurs“ ein, das erspart Ihnen die Eingabe in der Ansicht „Fachwahl“. Für die Leistungskurse können Sie dann in der Fachwahl anstatt „GK“ die Angabe „LK“ machen. Geben Sie die Unterrichtsarten ggf. über `Schlüsselverzeichnisse > Unterrichtsarten` ein. Ausschlaggebend sind dort die Angaben in der Spalte „Schlüssel“.

Die weiteren Spalten sind in diesem Zusammenhang nicht relevant.

## Fachwahl direkt eintippen in der Ansicht `Kursplan > Schüler`

Alternativ können Sie die Fachwahlen auch direkt in der Ansicht `Kursplan > Schüler` eintippen. Klicken
Sie dazu auf die betreffende Zelle. Achten Sie darauf, dass dabei Liste bearbeiten markiert ist.

!!! info "Hinweis"

    Damit DAVINCI erkennen kann, welche Kurse welche Unterrichtsart erhalten sollen, also z.B. die Kurse der ersten beiden Spalten sollen die Leistungskurse, die anderen die Grundkurse sein, richtet sich DAVINCI nach den Angaben des ersten Schülers in der Liste. Sie sollten daher den ersten Schüler in der
Ansicht `Kursplan > Fachwahl` eingeben. Die weiteren Fachwahlen Schüler können Sie dann in der Ansicht `Kursplan > Schüler` eintippen.

![Fachwahl direkt eingeben](/assets/images/KP/KP_Fachwahl.png)

## Fachwahlen nach MAGELLAN übertragen

Wenn Sie die Fachwahl für alle Schüler eingegeben haben, können Sie mit der Kurserstellung und Blockung fortfahren. Über `Plan > Importieren und Exportieren > Nach MAGELLAN exportieren` können Sie die Schülerfachwahlen inklusiv der zugeordneten Kurse wieder nach MAGELLAN übertragen.

![Datenexport nach MAGELLAN starten](/assets/images/courseplan9.png)

## Fachwahlen löschen

![Schülerdaten löschen](/assets/images/courseplan10.png)

Wechseln Sie in die Ansicht `Kursplan > Schüler` und markieren Sie klicken Sie die gewünschten Schüler. Sie können mit Strg+Mausklick und Shift+Mausklick mehrere Zeilen in der Tabelle markieren. Klicken Sie oben im Menü auf Löschen, um die entsprechenden Zeilen zu löschen. Das Dialogfenster `Schüler löschen` gibt Ihnen die Option die Schüler oder nur die Fachwahlen der markierten Schüler zu löschen. Wählen Sie dort die Option `Nur Fachwahlen löschen`.

!!! info "Hinweis"

    Wenn Sie eine Stundentafel allen Schülern des Jahrgangs zugewiesen haben, um anschließend die Fachwahlen einzugeben, sind je Schüler unbenutzte Fächer als graue Zeilen in der Ansicht `Schüler > Fachwahlen` übrig geblieben. Das Dialogfenster `Schüler löschen` gibt Ihnen die Möglichkeit nur die Fachwahlen ohne Belegung zu löschen. Wählen Sie dort die Option `Nur Fachwahlen ohne Belegung löschen`.
