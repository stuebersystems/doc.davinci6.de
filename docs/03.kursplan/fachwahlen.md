# Fachwahlen eingeben

[1]:/assets/images/KP/fachwahlen_01.png
[2]:/assets/images/KP/fachwahlen_02.png
[3]:/assets/images/KP/fachwahlen_03.png
[4]:/assets/images/KP/fachwahlen_04.png
[5]:/assets/images/KP/fachwahlen_05.png
[6]:/assets/images/KP/fachwahlen_06.png
[7]:/assets/images/KP/fachwahlen_07.png
[8]:/assets/images/KP/fachwahlen_08.png
[9]:/assets/images/KP/fachwahlen_09.png
[10]:/assets/images/KP/fachwahlen_10.png
[11]:/assets/images/KP/fachwahlen_11.png
[12]:/assets/images/KP/fachwahlen_12.png
[13]:/assets/images/KP/fachwahlen_13.png

Die Fachwahlen der Schüler werden in der Ansicht `Kursplan > Fachwahlen` erfasst und ggf. auch entsprechend der bundeslandspezifischen Fachwahlüberprüfung geprüft. Damit eine Fachwahlüberprüfung aufgrund eines Fachwahlskriptes erfolgen kann, sind gewisse Voreinstellungen im Stammdatenfenster erforderlich.

## Voreinstellungen Stammdatenfenster

### Stammdaten Klassen

In DAVINCI definieren Sie in den DAVINCI-Stammdaten die Klassen. Sie können eine Jahrgangsstufe in Klassen aufteilen (11a, 11b usw.) oder pro Klassenstufe nur eine Klasse eingeben - wichtig ist, dass über das Feld Stufe der Jahrgang zugeordnet wird. Damit sind klassenübergreifende Kurse innerhalb eines Jahrgangs und auch jahgangsüerbgreifende Kurse abbildbar. Des Weiteren geben Sie das Fachwahlskript an, nach dem die Fachwahl überprüft werden soll.

Bitte beachten Sie dazu folgende notwendige Eingaben:

| Spalte        | Bedeutung                                                                                                          |
| -------------- | ------------------------------------------------------------------------------------------------------------------ |
| Stufe          | Angaben für den Jahrgang (11, 12, 13)                                                                              |
| Modus          | Stellen Sie hier „Kurse“ ein, dann kann zwischen diesen Klassen in der Ansicht „Kursplan“ geblättert werden.       |
| Skript         | Geben Sie hier das Fachwahlskript für Ihr Bundesland an, das für die Fachwahlüberprüfung sorgt.                    |
| Schüler        | Die Schülerzahl wird automatisch berechnet                                                                         |
| Verordnungstyp | Machen Sie hier ggf. weitere Angaben für das Fachwahlskript, z.B. „G8“ falls es sich um einen G8-Jahrgang handelt. |

Hinzu kommen ggf. weitere Angaben, welche insbesondere für Fachwahlüberprüfungen notwendig sind, die mehrere
Halbjahre überprüfen, wie es aktuell in Berlin der Fall ist:

| Spalte    | Bedeutung                                                                                                                                                                                                                                                                        |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Startjahr | Tragen Sie hier ausgehend vom Jahrgang das Startjahr für den Eintritt in die gymnasiale Oberstufe ein. Startjahr der Klasse                                                                                                                                                      |
| Halbjahr  | Nummer des Halbjahres, in dem sich die Klasse aktuell für diesen Planungszeitraum befindet, d.h. 1, 2, 3, 4, 5, 6 (E1=1, E2=2....Q3=5, Q4=6). Aus Startjahr und Halbjahresindex errechnet sich, welche Fächer der Schüler in diesem Zeitraum bzw. in diesem Halbjahr belegt hat. |

[![Liste der Klassen bzw. Jahrgänge][1]][1]

!!! warning "Wichtig"

    In den KURSPLAN-Ansichten wird immer mit der Jahrgangsstufe (Spalte „Stufe“) gearbeitet. Wenn Sie z.b den Jahrgang 12 als eine Klasse „12" eingegeben haben, sind Jahrgangstufe und Klasse gleichbedeutend. Wenn Sie den Jahrgang 12 in Klassen 12A, 12B, 12C aufteilen, werden alle Schüler dieser Klassen angezeigt.

DAVINCI wird mit Fachwahlskripten für verschiedene Bundesländer und Schularten ausgeliefert. Ein Fachwahlskript hat die Dateiendung „.js“. Technisch gesehen ist ein Fachwahlskript eine JavaScript-Datei. Die ersten drei Buchstaben kennzeichnen das Bundesland, die Jahreszahl informiert über die Ausgabe des Skripts bzw. die zugrundeliegende Verordnung.

Namensanfang der Fachwahlskripte:

| Abkürzung | Bundesland             |
| --------- | ---------------------- |
| BAY       | Bayern                 |
| BAW       | Baden-Württemberg      |
| BER       | Berlin                 |
| BRA       | Brandenburg            |
| BRE       | Bremen                 |
| HES       | Hessen                 |
| HAM       | Hamburg                |
| NIE       | Niedersachen           |
| NRW       | Nordrhein-Westfalen    |
| MVP       | Mecklenburg-Vorpommern |
| SAA       | Sachsen-Anhalt         |
| SAC       | Sachsen                |
| SAR       | Saarland               |
| SHL       | Schleswig-Holstein     |
| RLP       | Rheinland-Pfalz        |
| THÜ       | Thüringen              |

!!! info "Hinweis"

    Sollte für Ihr Bundesland bzw. Ihre Schulform kein Fachwahlskript vorhanden sein, fragen Sie bei uns nach, wir erstellen ständig neue Skripte gemäß neuer Verordnungen.

!!! info "Hinweis"

    Welche Angabe das jeweilige Skript verlangt, können Sie in unserer Dokumentation [Landesanpassungen](https://doc.la.stueber.de/) nachlesen.

### Stammdaten Fächer

Im Falle Sie nutzen das von uns mitgelieferte Fachwahlskript, müssen Sie jedem Fach, dass Sie in der Oberstufe verwenden, unter `Stammdaten > Fächer` ein Fachkategorie zuweisen. Welche Fachkategorien das Fachwahlskript für Ihr Bundesland verwendet, finden Sie unter [Fachkategien](https://doc.la.stueber.de/fachwahlen/). Bitte wählen Sie in diesem Kapitel Ihr Bundesland aus und verwenden Sie nur die gekennzeichneten Fachkategorien.

[![Stammdatenfenster Fächer mit Hinterlegung Kategorien je Fach, die für die Fachwahlüberprüfung erforderlich sind][1]][1]

### Schüler eingeben

Wechseln Sie in die Ansicht `Kursplan > Schüler`. Hier werden alle Schüler des jeweiligen Oberstufenjahrgangs angezeigt. Sie können die Schüler (der Oberstufenjahrgänge) über den Befehl `Neu` eingeben. In der Ansicht `Kursplan > Schüler` wird der Schüler automatisch dem eingestellten Jahrgang zugeordnet.

[![Ansicht `Kursplan > Schüler" im Jahrgang 11][3]][3]

Alternativ dazu können Sie die Schüler auch in der Ansicht `Stammdaten > Schüler` eingeben. Dort werden Ihnen sämtliche Schüler aller Klassen angezeigt. In dieser Ansicht muss jeder Schüler in der Spalte „Klasse“ einem Jahrgang zugeordnet werden. Jahrgang und Klasse ist in diesem Fall gleichbedeutend.

[![Ansicht `Stammdaten > Schüler`][4]][4]

Wenn Sie in der Schulverwaltung MAGELLAN einsetzen, können Sie u.a. auch Schülerdaten nach DAVINCI übergeben. Weitere Informationen finden Sie dazu im Abschnitt [Fachwahl aus MAGELLAN importieren](https://doc.davinci6.stueber.de/03.kursplan/fachwahlen/#fachwahl-aus-magellan-importieren).

!!! info "Hinweis"

    In der Ansicht `Stammdaten > Schüler` können Sie die Schülerdaten mit Cut & Paste aus der Windows Zwischenablage übernehmen. Damit können Sie sehr schnell Ihre Schülerdaten aus Excel oder Word nach DAVINCI importieren.

## Fachwahl aus MAGELLAN importieren

Falls Sie MAGELLAN einsetzen, können Sie über den Befehl `Plan > Importieren und Exportieren` die
Schüler aus MAGELLAN übernehmen. Sie können die Schüler von MAGELLAN importieren, die Fachwahlen eingeben und die Fachwahlen der Schüler dann wieder nach MAGELLAN exportieren.

[![Datenimport von MAGELLAN starten][5]][5]

!!! info "Hinweis"

  Die Fachwahleingabe ist auch in MAGELLAN möglich, allerdings ohne Stundenzahlen. Die Fachwahlen aus MAGELLAN können per Import nach DAVINCI übernommen werden. MAGELLAN verwendet zur Fachwahlüberprüfung das gleiche Fachwahlskript wie DAVINCI. DAVINCI bietet mehr Funktionen zur Fachwahleingabe. So dass Sie im Zweifelsfall die Fachwahl in DAVINCI erfassen sollten.

## Fachwahlen in DAVINCI KURSPLAN eingeben

### Fachwahl direkt eintippen in der Ansicht `Kursplan > Fachwahlen`

Wechseln Sie in die Ansicht `Kursplan > Fachwahlen`. Hier können Sie für jeden Schüler dessen Fachwahl bestimmen. Wenn Sie bei der betreffenden Klasse des Schülers unter `Stammdaten > Klassen` in der Spalte „Skript“ das betreffende Fachwahlskript angegeben haben, wird die Eingabe entsprechend der durch das Skript geprüften Oberstufenverordnung überprüft. Der Name des jeweilige Skripts wird rechts oben in der Ansicht angezeigt. Ggf. werden Fehlermeldungen, Fachwahlkombinationsnummer oben in der Ansicht angezeigt. Geben Sie die gewünschten Fächer über `Start > Neu` ein und machen Sie die entsprechenden Angaben in den Spalten „Unterrichtsart“, „Fachstatus“ und „Stunden“.

[![Die Fachwahlen eines Schülers][6]][6]

Mit der Markieren-Schaltflächen können Sie alle Halbjahre eines Fachs markieren (Hintergrund Weiß) oder demarkieren (Hintergrund Grau). Indem Sie eine Halbjahreszelle in der Tabelle anklicken, können Sie einzelne Halbjahre markieren bzw. demarkieren. Das aktuelle Halbjahr “Q1“ (siehe Spalte „Halbjahr“ in der Ansicht `Stammdaten > Klassen`) ist durch die Hintergrundfarbe markiert. Im Bereich „Kurswahl“ ist der jeweils gewählte Kurs durch den hervorgehobenen Zellenrahmen markiert.

Die Fachwahlangaben:

| Spalte         | Bemerkung |
| -------------- |--------------------------------- |
| Fach | Gewähltes Fach, das mit der Angabe von `Unterrichtsart` und `Fachstatus` näher spezifiziert werden muss. |
| Kursnr | Kursnummer |
| Unterrichtsart | Unterrichtsart, z.B. „LK“ oder „GK“ oder „Kurs“, abhängig von Fachwahlskript. Geben Sie die Unterrichtsarten ggf. über `Extras > Schlüsselverzeichnisse > Unterrichtsarten` ein. Ausschlaggebend sind dort die Angaben in der Spalte „Schlüssel“. Diese Angabe wird von der Blockungsautomatik mit der Vorgabe „Unterrichtsart“ in der Ansicht `Kursplan > Blöcke` abgeglichen. |
| Fachstatus     | Prüfungsfach z.B. „1PF“, „2PF“, „3PF“, „4PF“ oder „5PF“, abhängig von Fachwahlskript. Geben Sie die Fachstatus ggf. über `Schlüsselverzeichnisse > Fachstatus` ein. Ausschlaggebend sind dort die Angaben in der Spalte „Schlüssel“.|
| Stunden | Geben Sie hier die Stundenzahl ein. Sie wird automatisch auf die Halbjahre 1 bis 6 übertragen. Diese Angabe wird von der Blockungsautomatik mit der Vorgabe „Min. Std“ und „Max. Std“ in der Ansicht `Kursplan > Blöcke` abgeglichen. Sie können diese Angabe auch leer lassen. |
| Schwerpunkt    | Fachschwerpunkt. Geben Sie die Fachschwerpunkte ggf. über `Schlüsselverzeichnisse > Fachschwerpunkte` ein, |
| Details        | Textfeld für Details. Diese Angabe ist abhängig vom jeweiligen Bundesland.|
| Merkmal        | Textfeld für Merkmale. Diese Angabe ist abhängig vom jeweiligen Bundesland. |
| Pflichtkurse   | Anzahl der Pflichtkurse  |
| Stunden        | Stundenanzahl des Kurses |
| E1…Q4          | Die Halbjahre der Oberstufe mit der jeweiligen Stundenanzahl, die sich aus der Spalte „Stunden“ ergibt. Sie können mit einem Mausklick in die betreffende Zelle Halbjahre für ein Fach markieren (weiß) oder demarkieren (grau). Wenn Sie unter „Stunden“ keine Stundenanzahl eingegeben haben, bleiben die Zellen der Tabelle leer.  |
| Kurswahl       | Mögliche Kurse zur Fachwahl. Dieser Bereich wird erst gefüllt, wenn bereits Kurse für ein Fach angelegt wurden. Per Mausklick können Sie dann manuell einen anderen Kurs wählen. Der aktuelle Kurs ist durch die Rahmenfarbe hervorgehoben. Kurse mit gelbem Hintergrund können überschneidungsfrei gewählt werden, andernfalls hat der Schüler eine Überschneidung, d.h. zwei Kurse in einem Block. |

### Fachwahl direkt eintippen in der Ansicht `Kursplan > Schüler`

Sie können Sie die Fachwahlen auch direkt in der Ansicht `Kursplan > Schüler` eintippen. Klicken Sie dazu in der Schülerzeile auf die betreffende Zelle. Achten Sie darauf, dass dabei Liste bearbeiten markiert ist.

[![Ansicht `Kursplan > Schüler`, Fachwahl direkt eingeben in Spalten 1-hier 11)][10]][10]

!!! info "Hinweis"

    Damit DAVINCI erkennen kann, welche Kurse welche Unterrichtsart erhalten sollen, also z.B. die Kurse der ersten beiden Spalten sollen die Leistungskurse, die anderen die Grundkurse sein, richtet sich DAVINCI nach den Angaben des ersten Schülers in der Liste. Sie sollten daher den ersten Schüler in der Ansicht `Kursplan > Fachwahl` eingeben. Die weiteren Fachwahlen der Schüler können Sie dann in der Ansicht `Kursplan > Schüler` eintippen.

Die Zellen-Hintergrundfarben ändern sich in der Ansicht `Kursplan > Schüler` sobald weitere Vorgaben in der Planung vorgenommen wurden.

Hier finden Sie eine kurze Erklärung.

| Hintergrundfarbe | Bemerkung |
| ---------------- |-------------- |
| Keine Farbe      | Reine Fachwahl, d.h. es wurde noch kein Kurs zugeordnet |
| Grün             | Eine Fachwahl bzw. Kurswahl, der ein Kurs zugeordnet wurde       |
| Rot              | Bei einem oder mehreren Schülern liegt ein Konflikt vor, weil zwei Kurse eines oder mehrerer Schüler im gleichen Block liegen. |
| Grau             | Kurs mit zu geringer Teilnehmerzahl, siehe Spalte „Min. Schüler“ in der Ansicht `Kursplan > Kurse`.  |
| Gelb             | Kurs mit zu hoher Teilnehmerzahl, siehe Spalte „Min. Schüler“ in der Ansicht `Kursplan > Kurse`. |

Eine Erklärung der Farben können Sie jederzeit über die DAVINCI-Optionen nachlesen. Öffnen Sie diese über `Extras > Optionen`, wechseln Sie in der Navigation auf "Farben" und dann in die Registerkarte "Kursplan". Sie können diese Farben nach Belieben verändern und jederzeit über die Schaltfläche `Standardangabe wiederherstellen` auf den Standard zurücksetzen.

[![DAVINCI-Optionen, Farben im Bereich Kursplan][11]][11]

### Fachwahl durch Anlegen einer Stundentafel in der Ansicht `Kursplan > Schüler` zuweisen

Eine Alternative für das manuelle Erfassen der Fachwahl pro Schüler bieten Ihnen Stundentafeln, die Sie als Vorlagen verwenden können. Mit einer Stundentafel legen Sie klassen- bzw. jahrgangsbezogene Fächerlisten an, welche die offizielle Unterrichtsverpflichtung der zugehörigen Klassen- bzw. Jahrgangsstufen wiederspiegeln.

Stundentafeln geben Sie in der Ansicht `Stammdaten > Stundentafeln` ein. Klicken Sie auf die Schaltfläche in der Spalte „Fächer“, um die Fächer der Stundentafel einzugeben. Genauere Informationen dazu finden Sie im [Abschnitt STUNDENPLAN > Stammdaten > Stundentafeln](https://doc.davinci6.stueber.de/01.stundenplan/stammdaten/#stundentafeln).

Mit der Schaltfläche `Start > Fachwahl erzeugen` können Sie für den aktuell markierten Schüler bzw. mehrere markierte Schüler oder alle Schüler des Jahrgangs die Fachwahl aufgrund dieser Stundentafel erzeugen.

Standardmäßig ist die Stundentafel des Jahrgangs eingestellt, Sie können aber auch eine andere wählen, wenn z.B. die Schüler nur aus einer von wenigen Fachkombinationen wählen können, weil an Ihre Schule nur diese Kombinationen angeboten werden.

[![Die Fachwahlen eines Schülers über Zuweisung einer Stundentafel hinterlegen][7]][7]

[![Ansicht `Stammdaten > Stundentafeln`, Liste möglicher Stundentafeln aller Jahrgänge inkl. Oberstufe][8]][8]

[![Fachliste einer Stundentafel][9]][9]

Die Bedeutung der Stundentafelspalten:

| Spalte         | Bemerkung   |
|----------------- |----------|
| Fach           | Gewähltes Fach, das mit der Angabe „Unterrichtsart“ näher spezifiziert werden muss.  |
| Unterrichtsart | Unterrichtsart, z.B. „LK“ oder „GK“ oder „Kurs“, wird in die gleichnamige Spalte der Fachwahl übernommen. Geben Sie hier z.B. als Standardvorgabe „GK“ oder „Kurs“ ein, das erspart Ihnen die Eingabe in der Ansicht „Fachwahl“. Für die Leistungskurse können Sie dann in der Fachwahl anstatt „GK“ die Angabe „LK“ machen. Geben Sie die Unterrichtsarten ggf. über `Schlüsselverzeichnisse > Unterrichtsarten` ein. Ausschlaggebend sind dort die Angaben in der Spalte „Schlüssel“. |

Die weiteren Spalten sind in diesem Zusammenhang nicht relevant.

## Fachwahlen löschen

Wechseln Sie in die Ansicht `Kursplan > Schüler` und markieren Sie den bzw. die gewünschten Schüler. Mit `Strg+Mausklick` und `Shift+Mausklick` können Sie mehrere Zeilen in der Tabelle markieren. Klicken Sie oben im Menüleiste auf `Löschen`, um die entsprechenden Zeilen zu löschen.

[![Ansicht KURSPLAN > Schüler][12]][12]

Das Dialogfenster `Schülerdaten löschen` öffnet sich und gibt Ihnen folgende Optionen:

* Schüler löschen
* Fachwahlen löschen
* Nur die Fachwahlen die nicht belegt wurden Belegung löschen
  
Bitte wählen Sie hier die Option `Fachwahlen löschen`.

[![Schülerdaten löschen-Dialog][13]][13]

!!! info "Hinweis"

    Wenn Sie eine Stundentafel allen Schülern des Jahrgangs zugewiesen haben, um anschließend die Fachwahlen einzugeben, sind je Schüler unbenutzte Fächer als graue Zeilen in der Ansicht `Schüler > Fachwahlen` übrig geblieben. Das Dialogfenster `Schülerdaten löschen` gibt Ihnen die Möglichkeit nur die Fachwahlen ohne Belegung zu löschen. Wählen Sie dort die Option `Nur die Fachwahlen die nicht belegt wurden Belegung löschen`.
