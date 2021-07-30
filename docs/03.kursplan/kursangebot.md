# Kursangebot erstellen

[1]:/assets/images/KP/kursangebot_01.png
[2]:/assets/images/KP/kursangebot_02.png
[3]:/assets/images/KP/kursangebot_03.png
[4]:/assets/images/KP/kursangebot_04.png
[5]:/assets/images/KP/kursangebot_05.png

Sind die Fachwahlen den entsprechenden Schülern zugeordnet und vom angegebenen Fachwahlskript überprüft, werden im nächsten Schritt die Kurse zu den Fachwahlen erstellt, die später zu Blöcken zusammengefasst werden können.

Für die Kursbildung in DAVINCI müssen Sie vorab wichtige Einstellungen in Ihrer Plandatei treffen. Diese nehmen Sie im Dialogfenster `Plan > Eigenschaften > Kursplan` vor.

[![Plan-Eigenschaften, Vorgaben für den KURSPLAN][1]][1]

Wählen Sie hier Ihre Standard-Unterrichtsart für einen Grundkurs aus den vorgegebenen Möglichkeiten aus. Zur besseren Unterscheidung der Grund- und Leistungskurse können Sie mit den Optionen festlegen, ob diese Unterrichtsart im Programm klein geschrieben wird oder/und alle anderen Kurse groß geschrieben werden. Stellen Sie bei den Vorgaben ein, ab wie vielen Teilnehmern ein neuer Kurs eröffnet werden soll und was die maximale Teilnehmerzahl sein darf.

## Zur Theorie der Kursblockung

Bevor wir mit der Erläuterung der Arbeitsschritte beginnen, wollen wir an dieser Stelle die grundlegende Arbeitsweise von DAVINCI KURSPLAN betrachten und einige Begriffe einführen.

### Fachwahl/Kurswahl

Eine Fachwahl oder Kurswahl bezeichnet den Wunsch eines Schülers in einem bestimmten Fach unterrichtet zu werden. In der Regel ist diese Fachwahl durch das gewünschte Fach, z.B. „Mathematik“ und das gewünschte Unterrichtsniveau bzw. die Unterrichtsart z.B. „Leistungskurs“ bestimmt. Aufgrund der Fachwahlen werden entsprechende Kurse eingerichtet, die eine Kursgruppe bilden, z.B. drei Leistungskurse Mathematik, d.h. MA1, MA2 und MA3. Damit alle Kurse in einer Woche stattfinden können, müssen Kurse zeitgleich stattfinden.

### Blöcke

Ein Block ist eine Menge von Kursen, die zeitgleich stattfinden sollen. Ein Kurs kann sich dabei auch auf mehrere Blöcke aufteilen. Dies kommt z.B. vor, wenn ein fünfstündiger Leistungskurs **MA1** mit Grundkursen **ge2** (3 Stunden Geschichte) und **sp3** (2 Stunden Sport) geblockt werden soll:

| Stunde | 1   | 2   | 3   | 4   | 5   |
| ------ | --- | --- | --- | --- | --- |
|        | MA1 | MA1 | MA1 | MA1 | MA1 |
|        | ge2 | ge2 | ge2 | sp3 | sp3 |

Es liegen also drei Stunden MA1 und ge2 sowie zwei Stunden MA1 und sp3 parallel. In diesem Fall richten wir zwei Blöcke ein:

| Block   |     |     |
| ------- | --- | --- |
| Block 1 | MA1 | ge2 |
| Block 2 | MA1 | sp3 |

## Bänder

Durch die Festlegung, dass wir den Kurs **MA1** mit den Grundkursen **ge2** und **sp3** blocken möchten, haben wir die Stundenzahl implizit mit berücksichtigt. Aufgrund der Stundenzahlen (Leistungskurse werden in der Regel 5-stündig, Grundkurse in der Regel 2- oder 3-stündig unterrichtet) ist es folgerichtig Leistungskurse und Grundkurse jeweils unabhängig voneinander zu blocken. Um von der eigentlichen Stundenzahl unabhängig zu sein, führen wir den Begriff des **Bandes** ein. 

!!! warning "Wichtig"

    Ein Band definiert eine Menge von Fächern oder Kursen, die zusammen geblockt werden sollen oder bereits geblockt sind. Im Beispiel von eben könnte man zwei Bänder einrichten:

| Band   |     |     |
| ------ | --- | --- |
| Band 1 | MA1 | ge2 |
| Band 2 | MA1 | sp3 |

Der Unterschied zur Blockeinteilung liegt darin, dass anhand der Bandeinteilung noch nicht festgelegt werden muss, welche Kurse genau zusammen geblockt werden müssen. Ergänzen wir dazu die beiden Bänder um weitere Kurse:

| Band   |     |     |     |     |
| ------ | --- | --- | --- | --- |
| Band 1 | MA1 | ge2 | la  | ru  |
| Band 2 | MA1 | sp3 | sp1 | sp2 |

Wenn ein Schüler nun in den Kursen **MA1** und **la** ist, müssen beide in unterschiedlichen Blöcken liegen. **MA1** kann daher nur noch mit **ge2** oder mit **ru** geblockt werden. Durch die Festlegung eines Kurses auf ein Band wird also lediglich eine Vorentscheidung getroffen, welche Kurse miteinander geblockt werden sollen. Es ist damit noch nicht festgelegt, welche Kurse des Bandes in einen gemeinsamen Block kommen.

Um

1. alle Leistungskurse und
2. alle Grundkurse ohne Sport und
3. alle Grundkurse Sport

unabhängig voneinander zu blocken, würde man sich für drei Bänder entscheiden:

| Band   |                            |
| ------ | -------------------------- |
| Band 1 | alle Leistungskurse        |
| Band 2 | alle Grundkurse ohne Sport |
| Band 3 | alle Grundkurse Sport      |

Es ergibt sich daraus allerdings eine minimale Anzahl von Blöcken, die je Band eingerichtet werden müssen. Hat jeder Schüler genau zwei Leistungskurse gewählt, müssen mindestens zwei Blöcke für das Band 1 eingerichtet werden, andernfalls hätten die Schüler zwei Kurse in einem Block. In Band 3 genügt ein Block, da jeder Schüler nur maximal einen Sportkurs hat. Die minimale Blockanzahl je Band folgt aus den Fachwahlen der Schüler für die Kurse dieses Bandes. Sie wird im Dialogfenster `Blöcke erzeugen`  angezeigt. Aus diesem Beispiel folgt auch eine weitere Erkenntnis: Eine Menge von Kursen aus denen jeder Schüler maximal einen gewählt hat, kann problemlos zusammen in einem Block zugordnet sein, d.h. sie ist *vollständig parallelisierbar*, z.B.

* Alle Kurse *Mathematik*
* Alle Kurse *Deutsch*
* Alle Kurse *Gemeinschaftskunde*

### Optimale Teilnehmerzahl und Abweichung

Bei der Verteilung der Schüler auf Kurse sollten möglichst alle Kurse einer Kursgruppe gleichverteilt sein. Haben z.B. 60 Schüler Mathematik Leistungskurs gewählt und besteht die entsprechende Kursgruppe aus den drei Kursen MA1, MA2 und MA3, sollte im Idealfall jeder Kurs 20 Schüler haben. Der Durchschnitt aller Kurse der Kursgruppe wird in DAVINCI in der Spalte Optimal angegeben, z.B. im  Dialogfenster `Kurse erstellen` und in der Ansicht `Kursplan > Blöcke`. Der Durchschnitt wird in DAVINCI ganzzahlig angegeben, er kann also um plus/minus Eins von mathematischen Durchschnitt abweichen. Die tatsächliche Schüleranzahl und die Abweichung vom Optimal-Wert wird in DAVINCI in der Regel bei jedem Kurs mit angezeigt:

* 22 +2 MA1
* 18 -2 MA2
* 20 MA3

MA1 hat 22 Schüler, d.h. 2 Kursteilnehmer mehr als das Optimum 20. MA2 hat 18 Teilnehmer, d.h. 2 Teilnehmer zu wenig bezogen auf das Optimum 20 erreichen. MA3 hat das Optimum 20 Schüler. Die Summe der Standardabweichungen (es werden nur die absoluten Beträge gezählt) über alle Kurse (in unserem Drei-Kurse-Beispiel wäre die Abweichung 5) ist das Maß für die Qualität der Verteilung: Je höher die Zahl desto schlechter ist die Verteilung. Im Idealfall ist die Abweichung Null, d.h. jeder Kurs hat seine optimale Schüleranzahl. Natürlich ist dieser Wert in der Praxis nicht zu erreichen, er stellt aber das mathematisch anzustrebende Ziel dar.

Wie bereits erwähnt wird der Durchschnitt immer ganzzahlig angegeben. Betrachten wir dazu ein Beispiel aus drei Englisch Kursen wobei insgesamt 35 Schüler des Jahrgangs dieses Fach gewählt haben. Rechnerisch ist das Optimum 11,666 Schüler je Kurs. In DAVINCI wird in folgender Verteilung keine Abweichung angezeigt, da diese weniger als Eins vom rechnerischen Optimum abweicht:

* 12 EN1
* 11 EN2
* 12 EN3

## Kurse erzeugen

[![Die Kursplanansicht für Kurse][2]][2]

Wählen Sie im Bereich `Kurse` zunächst die Jahrgangsstufe aus, für die Sie die Kurse erzeugen möchten. Um die Kurse zu erzeugen wählen Sie den Befehl Kurse erzeugen im Menü `Start`. In dem folgenden Dialogfenster erhalten Sie nun einen Überblick über die erstellten Kurse.

[![Kurse erzeugen][3]][3]

Die Spalte `Kursanzahl` wird als Vorgabe aus den Angaben im Dialog `Plan > Eigenschaften` errechnet. Ändern Sie ggf. die Angaben in dieser Spalte. In der Spalte Schüler können Sie sehen, wie viele Schüler dieses Fach gewählt haben. Die Spalte `Optimal` errechnet sich aus dem Spaltenwerten „Schüler“ geteilt durch die „Kursanzahl“ (nur der ganzzahlige Anteil), d.h. in bei dieser Schülerzahl je Kurs ist die Abweichung der Schülerzahlen in den Kursen des Fachs im Idealfall Null. Die Optimale Schülerzahl gilt es im Folgenden bei der Blockung und Verteilung anzustreben. Wenn Sie die Angabe in der Spalten „Kursanzahl“ ist ein von DAVINCI errechneter Vorgabewert. Sie sollten ihn ggf. ändern.

In der Spalte `Band` können Sie die Bandnummer eingeben. Standardmäßig wird für jede Unterrichtsart eine Bandnummer vorbesetzt.

In der Spalte `Dauer` können Sie die Stundenanzahl der zu erzeugenden Kurse angeben. Sie spielt aber für die weitere Blockung und Verteilung keine Rolle und kann daher auch später vom Stundenplaner nachgetragen werden.

Klicken Sie auf `OK`, um die entsprechenden Kurse zu erzeugen.

Die Spalten in der Ansicht `Kurse` entsprechen der Veranstaltungsliste in der Ansicht `Stundenplan`. Lediglich die Spalte `Band` erscheint hier zusätztlich. Sie können in der Ansicht weitere Angaben zu Lehrern und Räumen machen, jedoch ist es in der Praxis ratsam, diese Angaben später nach der  Blockung und Verteilung zu machen, da sie unnötig einschränken würden. Neben Lehrer und Raumzuweisungen haben Sie die Möglichkeit Kurse hinzuzufügen (rechte Maustaste und Neue Veranstaltung), zu duplizieren (rechte Maustaste Veranstaltung duplizieren oder Block duplizieren) oder zu löschen (markieren Sie eine oder mehrere Veranstaltung in der Liste und klicken Sie rechte Maustaste Veranstaltungen löschen). Siehe dazu auch die folgenden Abschnitte.

Spalte | Inhalt
-|-
Unverplant | Anzahl der unverplanten Stunden einer Unterrichtsveranstaltung
Block | Blockkürzel, gleiche Blockkürzel geben an, dass alle Veranstaltungen dieses Blocks zu gleichen ‚Zeit parallel stattfinden. Das Blockkürzel ist eindeutig für den gesamten Plan.
Fach | Unterrichtsfach der Veranstaltung
Dauer | Dauer der Veranstaltung je Woche, standardmäßig die der Soll-Stunden-Wert aus der Stundentafel. Sollte der Soll-Sunden-Wert nicht der Unterrichtsdauer entsprechen, z.B. bei geteiltem oder periodischem Unterricht, muss dieser Wert im Nachhinein angepasst werden.
Termine | Terminserien der Veranstaltungen, z.B. „2-2-1“ für zwei Doppelstunden und eine Einzelstunde
Lehrer | Kürzel des Lehrers, der den Fachunterricht in einer Veranstaltung halten soll.
Raum | Ein Raum oder ein Raum-Platzhalter oder eine Liste von Räumen. In einer Block werden unterschiedliche Räume durch Raum-Platzhalter z.B. #R1 oder #R2 spezifiziert. Ein Platzhalter ist ein beliebiger Name beginnend mit ``#``.
Räume | Kürzel der Unterrichtsräume, die als Vorgabe für die Planung der Termine dient. Beim Kopieren der Stundentafel wird hier standardmäßig der Klassenraum eingetragen. Wurde dem Unterrichtsfach in den Stammdaten ein Fachraum zugeordnet, wird statt des Klassenraums der Fachraum eingetragen.
Soll (W) | Durchschnittlichen Wochenstunden-Soll-Wert der Veranstaltung. Beim Kopieren der Stundentafel wird hier der Wert des Fachs in der Spalte „Soll“ der zugehörigen Stundentafel eingetragen. Falls bei einem Fach in der Spalte „Angleichung“ der Stundentafel ein Wert eingetragen ist, so wird dieser zu dem Eintrag in der Spalte „Soll“ der Stundentafel hinzuaddiert. Der Eintrag in der Spalte „Soll (W)“ bildet also die Summe aus den Werten „Soll“ und „Angleichung“ der Stundentafel
Ist (W) | Stellt den durchschnittlichen Wochenstunden-Ist-Wert einer Veranstaltung dar. Dieser ermittelt sich als Produkt aus dem Eintrag im Feld „Dauer“ der Veranstaltungsliste und dem zugehörigen wochenbezogenen Berechnungsfaktor. Bei diesem Faktor handelt es sich um einen Wert zwischen „1“ und „0“. Der Wert„1“ bedeutet, dass eine Veranstaltung in allen Unterrichtswochen des Planungszeitraums stattfindet. Der Wert in der Spalte „Ist (W)“ entspricht in diesem Beispiel dem Wert in der Spalte „Dauer“. Ein Wert kleiner als „1“ bedeutet, dass eine Veranstaltung nicht in allen Unterrichtswochen des Planungszeitraums stattfindet. Die Anzahl der Unterrichtswochen einer bestimmten Veranstaltung wird dabei durch den allgemeinen Wochenfaktor geteilt. Der allgemeine Wochenfaktor steht als statistischer Kennwert für die Anzahl aller Unterrichtswochen des Planungszeitraums und wird vom Planer im Vorfeld definiert.
Ist/J | Ist Stunden als Jahressumme.
Soll/J | Stunden Soll als Jahressumme.
Periode | Kürzel der Periode an, die einer Veranstaltung zugewiesen ist. Ist dieses Spalte leer, so findet die Veranstaltung in allen Unterrichtswochen des Planungszeitraums statt. Falls bei der Klasse in den Stammdaten eine Periode angegeben wurde, wird diese Spalte bereits beim Erzeugen der Veranstaltung aus der Stundentafel mit dem entsprechenden Periodenkürzel gefüllt.
Bemerkung | Beliebiger Bemerkungstext, der im Ausdruck, im HTML-Export sowie in der Bildschirmausgabe des Stundenplans bei den Terminen der zugehörigen Veranstaltung eingeblendet werden kann.
Wochen | Kalenderwochen, in denen der Unterricht stattfindet. Beim Kopieren der Stundentafel wird hier standardmäßig der Eintrag „Jede Woche“ eingetragen. Wurde einer Klasse in den Stammdaten eine Periode zugewiesen, erscheinen in dieser Spalte die Kalenderwochen der Periode. Wird nur einzelnen Unterrichtsveranstaltungen eine Periode zugewiesen, dann erscheinen an dieser Stelle in den betroffenen Veranstaltungszeilen ebenfalls die zugehörigen Periodenwochen.
Wochenanzahl | Anzahl der Woche gemäß zugwiesener Periode
Klassen | Kürzel der Klassen an, die einer Unterrichtsveranstaltung als Teilnehmer zugewiesen sind. Beim Kopieren der Stundentafeln wird pro Klassenplan die zugehörige Klasse eintragen.
Unterrichtsart | siehe  `Extras > Schlüsselverzeichnisse > Unterrichtsarten`, wichtige Differenzierung z.B. für Leistungs- und Grundkurse sowie Profilfächer für die gymnasiale Oberstufe
Gültig von/bis | Mit diesen beiden Feldern können Sie die Veranstaltung befristen.
Nr | Veranstaltungsnummer, z.B. Vorlesungsnummer. Diese Angabe hat keine direkte Funktion für die weitere Stundenplanung und besitzt ausschließlich informativen Charakter. 
Schiene | Die Spalte „Schiene“ zeigt die Zeitschiene an, auf der eine Veranstaltung angesiedelt ist. Standardmäßig ist hier die Zeitschiene „A“ hinterlegt. Darüber hinaus stehen die Zeitschienen „B“, „C“, „D“, „E“ und „X“ zur Verfügung. Durch die Platzierung von Veranstaltungen auf unterschiedliche Zeitschienen, können Sie der Setzautomatik differenzierte Vorgabenmachen, welche Veranstaltungen sich im Plan überschneiden dürfen und welche nicht.
Schüler | Anzahl der Schüler, die einer Unterrichtsveranstaltung zugewiesen sind. Beim Kopieren der Stundentafel wird hier die Schüleranzahl eingetragen die in den Stammdaten der Klasse angegeben wurde. Wurden in DAVINCI Schüler einer Veranstaltung zugewiesen, z.B. in der Oberstufe, wird die entsprechende Schüleranzahl automatisch ausgewiesen und ist nicht mehr manuell eingebbar.
intern | -
Kategorie | -
Raumart | -
Doppelstd |-
gesperrt | -
Fachfolge | Fachfolgekürzel, gibt an welche Veranstaltungen direkt aufeinanderfolgend und welche Veranstaltungen möglichst nicht direkt aufeinanderfolgend verplant werden sollen. Diese Angabe ist nur für das Planen mit der Automatik relevant.
Zeitraum | -
Zeitkonto | -
Ressourcen | -
URL | Verlinkung

## Kursen Bandnummer zuweisen

Markieren Sie in der Ansicht `Kursplan > Kurse` die gewünschten Kurse und klicken Sie auf rechte Maustaste und Bandnummer ändern und geben Sie im folgenden Dialogfenster die neue Bandnummer ein und klicken Sie auf `OK`.

## Einen neuen Kurs erzeugen

Um einen Kurs zu erzeugen wählen Sie den Befehl Neue Veranstaltung aus der Menüleiste oder nutzen Sie die Taste "Einfg" auf Ihrer Tastatur. Es wird daraufhin eine leere Zeile in der Veranstaltungsliste erzeugt. Standardmäßig ist die Tabelle nicht editierbar, um unbeabsichtigte Fehleingaben zu vermeiden. Klicken Sie im Menü oben auf `Bearbeiten`, um den „Bearbeiten-Modus“ zu aktivieren und die Tabelle bearbeiten zu können. 

## Einen Kurs duplizieren

Wenn Sie einen Kurs duplizieren wollen, markieren Sie den betreffende Kurs in der Ansicht `Kursplan > Kurse` mit einem Mausklick und wählen unter Neue Veranstaltung den Befehl Veranstaltung duplizieren oder klicken Sie mit Rechts auf den gewünschten Kurs. Das Tastenkürzel "Strg + C" können Sie ebenfalls verwenden um eine Veranstaltung zu duplizieren. Wenn Sie den Befehl ausführen wird ein neuer Kurs mit den gleichen Daten erzeugt. Eine eventuell eingetragene Blockung wird ebenfalls übernommen.

## Kurse löschen

Um einen Kurs zu löschen wählen Sie den Kurs in der Veranstaltungsliste aus und wählen Sie `Löschen` in der Menüleiste oder im Kontextmenü, welches Sie mit einem Rechtsklick auf den Kurs öffnen können. Mit "Strg + Mausklick" und "Shift + Mausklick" können Sie mehrere Zeilen markieren und so mehrere Kurse gleichzeitig löschen.

!!! info "Hinweis"

    Das Löschen von Kursen kann nicht rückgängig gemacht werden.

## Mehrfachzuweisungen

[![Mehrfachzuweisung][5]][5]

Mit Hilfe des Befehls `Start > Mehrfachzuweisung` können Sie mehreren Schülern ein neues Fach bzw.
einen neuen Kurs zuweisen.
