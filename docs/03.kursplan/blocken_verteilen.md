# Blocken und Verteilen

[1]:/assets/images/KP/blocken_01.png
[2]:/assets/images/KP/blocken_02.png
[3]:/assets/images/KP/blocken_03.png
[4]:/assets/images/KP/blocken_04.png
[5]:/assets/images/KP/blocken_05.png
[6]:/assets/images/KP/blocken_06.png
[7]:/assets/images/KP/blocken_07.png
[8]:/assets/images/KP/blocken_08.png
[9]:/assets/images/KP/blocken_09.png
[10]:/assets/images/KP/blocken_10.png
[11]:/assets/images/KP/blocken_11.png
[12]:/assets/images/KP/blocken_12.png
[13]:/assets/images/KP/blocken_13.png
[20]:/assets/images/KP/blocken_20.png
[21]:/assets/images/KP/blocken_21.png
[22]:/assets/images/KP/blocken_22.png
[23]:/assets/images/KP/blocken_23.png
[24]:/assets/images/KP/blocken_24.png

[![Blöckefenster][1]][1]

In der Ansicht `Kursplan > Blöcke` können Sie per Automatik und manuell:

1. Blöcke einrichten
2. Kurse Blöcken zuweisen (Kurse blocken)
3. Schüler auf Kurse verteilen

Die Zahl vor der Kursbezeichnung in der Tabelle gibt die Anzahl der Kursteilnehmer an. Ggf. gibt eine weitere Zahl die Abweichung zur optimalen Schülerzahl an. Eine Erläuterung gibt das Kapitel "Zur Theorie der Kursblockung". Die Bedeutung der Zellen-Hintergrundfarben entspricht der der Ansicht `Kursplan > Schüler` (siehe Kapitel "Fachwahlen eingeben").

Im Dashboard unten werden wichtige Angaben zur Qualität der aktuellen Blockung und Verteilung gemacht:

[![Dashboard][21]][21]

Angabe               | Beschreibung
-------------------- | ------------
Kurs(e) ungeblockt   | Die Anzahl der nicht geblockten Kurse. Unter dem Strich wird die Anzahl aller Kurse angezeigt.
Kurswahl(en) offen   | Die Anzahl der Kurswahlen (Fachwahlen) die noch offen sind, d.h. denen kein Kurs zugewiesen wurde. Unter dem Strich wird die Anzahl aller Kurswahlen angezeigt.
Abweichung           | Die Summe der absoluten Standardabweichung über alle Kurse.
Teilnehmer Konflikte | Die Anzahl der Konflikte aufgrund von Schülern mit Kursen in gleichem Block.
Min/Max Konflikte    | Die Anzahl der Konflikte aufgrund von nicht eingehaltenen Minimal- und Maximalteilnehmeranzahlen.
Kurs(e) ohne Band    | Anzahl der Kurse ohne Bandnummer (mit Bandnummer Null). Wird nur angezeigt, wenn die Anzahl größer als Null ist.

Eine Zeile repräsentiert einen Block. Jeder Block enthält in der Spalte „Band“ die jeweilige Bandnummer. Von der Automatik können nur Kurse derselben Bandnummer dem betreffenden Block zugeordnet werden.

Die Spalten auf der Registerkarte `Blöcke` in der Ansicht `Kursplan > Blöcke`:

[![Blockzeile][22]][22]

Spalte               | Bemerkung
-------------------- | ------------
Block                | Blockname. Kann frei gewählt werden, muss aber eindeutig über den gesamten Plan sein.
Band                 | Bandnummer. Automatik kann nur Kurse gleicher Bandnummer in diesem Block zuordnen. In der Ansicht „Kurse“ sollten Sie jedem Kurs eine  Bandnummer zuweisen.
Automatik            | Ja: Kurse können von der Automatik dem Block zugewiesen werden, andernfalls nicht.
Min.                 | Stunden Automatik kann nur Kurse gleicher Bandnummer in diesem Block zuordnen, die mindestens die angegebene Stundenzahl habe.
Max.                 | Stunden Automatik kann nur Kurse gleicher Bandnummer in diesem Block zuordnen, die maximal die angegebene Stundenzahl habe.
Schüler              | Summe der Kursteilnehmer über alle Kurse des Blocks. Der Wert in dieser Spalte sollte den Wert in der Spalte „Optimal“ nicht wesentlich überschreiten, um eine möglichst optimale Verteilung zu gewährleisten.
Optimal              | Summe der optimalen Durchschnittswerte über alle Kurse des Blocks.
Abweichung           | Summe der Standardabweichungen vom Optimalwert über alle Kurse des Blocks.
1, 2, 3 …            | Kursangaben: Teilnehmeranzahl, ggf. +-Abweichung zum Optimalwert, Kursbezeichnung

## Alle Blöcke erzeugen

Wechseln Sie in die Ansicht `Kursplan > Blöcke`. Wählen Sie den Befehl `Blöcke erzeugen` in der Menüleiste. Es öffnet sich das Dialogfenster `Blöcke erzeugen`, in dem Sie einstellen können für welche Unterrichtsart wie viele Blöcke erstellt werden sollen. Stellen Sie je Band die Anzahl der gewünschten Blöcke ein und klicken Sie auf `OK`.

[![Blöcke erzeugen][20]][20]

!!! info "Hinweis"

    Je mehr Blöcke Sie erzeugen, umso einfacher ist das Blocken der Kurse und die Verteilung der Schüler auf Kurse auf Blöcke umso schwieriger wird es aber für den Stundenplanmacher einen Oberstufenplan zu erstellen. Unter „Blöcke minimal“ wird die minimal notwendige Blockanzahl angezeigt. Sie sollte nicht unterschritten werden, da andernfalls keine vollständige Verteilung der Schüler möglich ist.

## Blöcke löschen

In der Ansicht `Kursplan > Blöcke` können Sie per Mehrfachmarkierung Blöcke markieren und löschen. Markieren Sie mit der Maus die Blockzeile bzw. den Block den Sie löschen möchten. Mit "Shift + Mausklick" und "Strg + Mausklick" können Sie auch mehrere Zeilen markieren. Klicken Sie dann auf `Löschen` im Menü `Start`. Ein Dialogfenster fragt Sie, ob auch die entsprechenden Schülern aus den Kursen gelöscht werden sollen oder nicht. Anschließend werden die Blöcke gelöscht.

## Block-Eigenschaften ändern

Eingetragene Blockeigenschaften können Sie in der Ansicht `Kursplan > Blöcke` wie folgt ändern:

* mit einem Mausklick eine Blockzeile und wählen Sie `Start > Bearbeiten` oder
* `Doppelklick` auf die Blockzeile oder
* `Rechtsklick` auf die Blockzeile, im Aufklappmenü `Block bearbeiten wählen`

In dem Dialog `Block-Eigenschaften ändern` können Sie alle Eigenschaften des Blocks ändern. Der Name ist die eindeutige Blockbezeichnung im Plan. Das Feld `Band` gibt an, dass nur Kruse derselben Bandnummer von der Blockungsautomatik diesem Block zugeordnet werden dürfen. In den Feldern `Minimale Std` (minimale Stundenzahl) und `Maximale Std` (maximale Stundenzahl) können Sie für die Blockungsautomatik vorgeben, dass nur Kurse mit der entsprechenden Stundenzahl diesem Block zugewiesen werden dürfen.

[![Block-Eigenschaften ändern][23]][23]

## Kurse automatisch blocken und Schülern zuordnen

Die Automatik blockt die Kurse und verteilt die Schüler auf Kurse, d.h. sie weist jedem Fach aus der Fachwahl eines Schülers eine Kursnummer zu. Sie können die Automatik sukzessive für bestimmte Jahrgänge und Bänder aufrufen. Z.B. kann es sinnvoll sein, zuerst die Leistungskurse eines Jahrgangs und danach die Grundkurse zu blocken und zu verteilen. Gegebenenfalls müssen Sie die Blockung bzw. die Verteilung löschen (siehe Abschnitt Blockung und Verteilung zurücksetzen) und die Fachwahlen einiger Schüler ändern, da sie nicht ohne Überschneidung verteilt werden konnten. Anschließend können Sie die Automatik erneut blocken bzw. verteilen lassen. Entscheiden Sie selbst, welche Vorgehensweise für Ihre Bedingungen am besten zutrifft.

[![Blockungsautomatik][2]][2]

Wählen Sie zunächst den Befehl `Start > Automatik`. Das Dialogfenster „Blockungsautomatik starten“ öffnet sich. Stellen Sie bei „Band“ das Band ein, dessen Kurse Sie blocken möchten. Alle Kurse mit dieser Bandnummer werden in Blöcke dieser Bandnummer geblockt. Wahlwiese können Sie „alle“ einstellen. Klicken Sie auf OK, um die Automatik entsprechend der Einstellungen zu starten.

Die Optionen im Dialogfenster „Blockungsautomatik starten“:

Option  | Beschreibung
------- | ------------
Kurse blocken | Blockt Kurse des angegebenen Bandes in Blöcke dieser Bandnummer.
Schüler verteilen | Sorgt dafür, dass die Schüler auf Kurse verteilt werden.
Beachte Kursteilnehmerzahl | Beachtet die minimale und maximale Kursteilnehmerzahl, die Sie entweder global unter `Plan-Eigenschaften > Kursplan` oder in der Ansicht `Kursplan > Kurse` in den entsprechenden Spalten „Min. Schüler“ und „Max. Schüler“ je Kurs einstellen können.
Akzeptiere Blockkonflikte | Akzeptiert Blockkonflikte aufgrund von zwei Kursen eines Schülers im gleichen Block, was ja eigentlich nicht vorkommen sollte. Diese Option kann gewählt werden, wenn man danach kollidierende Schüler manuell in andere Kurse setzen möchte.

[![Ergebnis der Automatik][3]][3]

!!! info "Hinweis"

    HINWEIS: Es empfiehlt sich das Blocken der Kurse und die Schülerverteilung gleichzeitig durchzuführen, weil hier die Automatik die Schüler sinnvoller verteilen kann. Dadurch werden Zeitkonflikte und unnötige Kurszuordnungen vermieden.

Die Automatik hält folgende Bedingungen ein:

* Die Kurse werden so geblockt, dass ein Schüler nie zwei Kurse im gleichen Block hat. Sollte das nicht möglich sein, wird für das betreffende Fach der Fachwahl keine Kurszuordnung vorgenommen, es sei denn die Option `Akzeptiere Blockkonflikte` ist aktiviert.

* Die Block-Eigenschaften, die Sie im Dialogfenster `Block-Eigenschaften` in der Ansicht `Kursplan > Blöcke` eingeben können müssen mit den Angaben beim Kurs übereinstimmen, genauer gesagt die Bandnummer und die minimale/maximale Teilnehmerzahl.

## Optimiere Verteilung

Über die Schaltfläche Optimiere Verteilung in der Ansicht Kursplan | Blöcke können Sie jederzeit für
eine gegebene Blockung die Schülerverteilung optimieren. DAVINCI versucht dabei Teilnehmern aus
Kursen mit einer positiven Abweichung, d.h. Kurse bei denen mehr Teilnehmer als optimal zugweisen
wurden in andere Kurse der Kursgruppe zu versetzen, also z.B. aus dem Kurs M1 in den Kurs M2 oder
M3, solange dies zu keinem Konflikt und diese Kurse eine negative Abweichung, d.h. weniger Teilnehmer
als optimal aufweisen.

## Blockung und Verteilung zurücksetzen

[![Blockung und Verteilung zurücksetzen][24]][24]

Mit dem Befehl Zurücksetzen können Sie das Ergebnis eines Automatiklaufs zurücksetzen, d.h. die Blockung der Kurse und die Verteilung der Schüler auf die Kurse wird für den aktuellen Jahrgang und das eingestellte Band zurückgesetzt. Entsprechend der Optionen wird die Blockung und/oder die Verteilung der Schüler zurückgesetzt,

## Kurse manuell einem Block zuweisen

So können Sie einen Kurs manuell einem Block zuweisen:

1. Wechseln Sie in die Ansicht `Kursplan > Blöcke`.

2. Öffnen Sie die Detailansicht `Passende Kurse`.

3. Klicken Sie in der Blöcke-Tabelle in die gewünschte Blockzeile. Unter „Passende Kurse“ werden Ihnen alle verfügbaren Kurse angezeigt. Ein gelbes Konfliktsymbol zeigt ggf. Konflikte für den jeweiligen Kurs an, die dadurch entstehen, dass Schüler mehrere Kurse im gleichen Block erhalten. In diesem Fall wird in der Spalte „Schülerkonflikte“ die Anzahl der Schüler mit solchen Konflikten angezeigt.

4. Markieren Sie den Kurs, den Sie in den markierten Block übernehmen möchten und klicken Sie in der Detailansicht Passende Kurse auf Diesen Block zuweisen. Noch einfacher ist es per Doppelklick auf den passenden Kurs. Damit wird der Kurs diesem Block zugewiesen und erscheint in der Blöcke-Tabelle. Vor dem Kurs in der Blöcke-Tabelle wird die Anzahl der Teilnehmer (am Anfang ist sie „0“) angezeigt.

## Kurs manuell einem Block zuweisen

[![Passende Kurse][4]][4]

Markieren Sie in der Ansicht `Kursplan > Blöcke` den Block, in den Sie einen Kurs blocken möchten, indem Sie in die betreffende Blockzeile klicken. Klicken Sie dann auf Passende Kurse und markieren Sie unter Passende Kurse den Kurs, den Sie in den Block setzen möchten und klicken Sie auf Diesem Block zuweisen. Damit wird der Kurs diesem Block zugewiesen. Auf diese Weise können Sie Kurse manuell einem Block zuweisen, die bisher noch nicht geblockt waren wie auch Kurse von einem Block in einen anderen setzen.

Alternativ können Sie auch per Drag & Drop einen Kurs in einen anderen Block verschieben:

* Klicken Sie auf einen Kurs in der Ansicht `Kursplan > Blöcke`, halten Sie die Maustaste gedrückt und ziehen Sie den Kurs in die geünschte Blockzeile und lassen Sie die Maustaste wieder los.

Die Spalten in der Detailansicht „Passende Kurse“ der Ansicht „Kursplan | Blöcke“ Register „Blöcke“:

Spalte                  | Bemerkung
----------------------- | ---------
Kurs                    | Kursbezeichnung
Konflikte               | Anzahl der Schülerkonflikte in diesem Kurs die entstehen, wenn man den Kurs diesem Block zuordnet.
Blockkurse-Schnittmenge | Anzahl der bereits geblockten Kurse aus diesem Block, mit denen mindestens eine Schüler-Überschneidung besteht. Je geringer die Zahl ist desto weniger Probleme mit anderen Kursen des Blocks sind zu erwarten.
Kurse-Schnittmenge      | Anzahl der bereits geblockten Kurse aus allen Blocken, mit denen mindestens eine Schüler-Überschneidung besteht. Je höher die Anzahl ist desto abhängiger ist dieser Kurs von anderen Kursen.
Schüler                 | Anzahl der Schüler im Kurs Unterrichtsart Unterrichtsart des Kurses
Block                   | Block des Kurses
Band                    | Bandnummer
Dauer                   | Stundenanzahl

## Die Ansicht „Kurse-Blöcke“

In der Ansicht "Kurse-Blöcke" werden am Schnittpunkt einer Block Spalte mit einer Kurszeile der jeweilige Kurs mit Teilnehmerzahl und ggf. der Abweichung zum Optimum angezeigt. Sie können auch in dieser Ansicht manuell blocken, indem Sie in der jeweiligen Zeile auf die Zelle des gewünschten Blocks klicken: Der Kurs wird dem betreffenden Block zugewiesen. Wie gewohnt zeigt eine grüne Hintergrundfarbe an, dass keine Konflikte bei den Teilnehmern eines Kruse vorliegen. Die roten Zahlen in den anderen Zellen geben an, bei wie vielen Teilnehmern Konflikte auftreten würden, wenn der Kurs in diesem Block zugeordnet werden würde. Bei Zellen ohne Anzahl würden keine Konflikte auftreten, sie werden daher durch eine gelbe Hintergrundfarbe hervorgehoben. In der Spalte Optimal wird die optimale Teilnehmerzahl, in der Spalte Schüler die tatsächliche Teilnehmerzahl des Kurses angezeigt, in der Spalte Abweichung die jeweilige Abweichung.

[![Ansicht Kurse-Blöcke][5]][5]

## Die Ansicht „Schüler-Blöcke“

In der Ansicht „Schüler-Blöcke“ werden je Schüler deren Kurse nach Blöcken geordnet dargestellt.

## Schüler manuell einem Kurs zuordnen

Alternativ zur Blockungsautomatik über `Start > Automatik`, die optional gleich die Schüler auf die Kurse verteilt, können Sie Schüler auch manuell Kursen zuzuordnen.

Vorgehensweise:

1. Rufen Sie die Ansicht `Kursplan > Schüler` auf. Sie sehen eine Übersicht über der den Schülern zugewiesenen Kursen (grün hinterlegt) und die Fachwahlen ohne Kurszuweisung (weiß hinterlegt). Je nach Einstellungen in den Datei-Eigenschaften werden die Grundkurse kleingeschrieben oder die Leistungskurse mit einer Klammerbemerkung versehen.

[![`Kursplan > Schüler`][12]][12]

* Öffnen Sie die Ansicht `Passende Kurse` in der Detailansicht. Klicken Sie in der Schüler-Tabelle auf den gewünschten Schülerkurs. Unter `Passende Kurse` werden alle Alternativkurse für die Fachwahl bzw. den markierten Kurs angezeigt. Alternativkurse, die zu einem Konflikt bei diesem Schüler führen würden, weil er dann zwei Kurse in einem Block hätte, werden mit dem gelben Konfliktsymbol vor der Kursbezeichnung gekennzeichnet. Je Alternativkurs werden die aktuellen Teilnehmeranzahl (Spalte Schüler) und die Anzahl der Schüler mit Konflikten (Spalte Schülerkonflikte), weil sie noch einen anderen Kurs im gleichen Block haben, angezeigt.

[![`Kursplan > Schüler`][13]][13]

* Wählen Sie `Kurs zuweisen`, wenn Sie den markierten Kurs zuweisen wollen oder doppelklicken Sie auf den gewünschten Kurs. Der Kurs wird nun grün hinterlegt beim Schüler angezeigt. Hat der Schüler bereits einen Kurs im gleichen Block, werden die Konfliktkurse des Schülers rot hinterlegt angezeigt.

In der folgenden Abbildung kann nur noch der Kurs „kr“ (Katholische Religion) konfliktfrei (er hat als einziger kein Konfliktsymbol) dem Block „12#6“ zugeordnet werden:

[![Kurs einem Block zuweisen][6]][6]

## Kursteilnehmer anzeigen

In den folgenden Ansichten können Sie sich in der Detailansicht Kursteilnehmer die Teilnehmer des aktuell markierten Kurses anzeigen lassen:

* In der Ansicht `Kursplan > Schüler`
* In der Ansicht `Kursplan > Kurse`
* In der Ansicht `Kursplan > Blöcke`

Sind bei Teilnehmern Konflikte vorhanden, weil sie zwei Kurse im gleichen Block haben, werden diese Teilnehmer durch ein gelbes Konfliktsymbol vor dem Namen gekennzeichnet. In der Spalte „Konflikte“ werden in diesem Fall die betreffenden Kurse ausgewiesen, die den Konflikt verursachen, d.h. die im gleichen Block sind. Sie können die Konflikte auflösen, indem Sie die betreffenden Kursteilnehmer aus dem Kurs entfernen oder indem sie einen Alternativkurs zuweisen. Die folgenden beiden Abschnitte beschreiben das Vorgehen dazu.

## Kursteilnehmer aus Kurs entfernen

So entfernen Sie einen oder mehrere Schüler aus einem Kurs:

* Rufen Sie eine der Ansichten `Kursplan > Schüler`, `Kursplan > Kurse` oder `Kursplan > Blöcke` auf.

* Öffnen Sie die Detailansicht `Kursteilnehmer`.

* Klicken Sie in der Ansicht auf den gewünschten Kurs. In der Detailansicht `Kursteilnehmer` werden die Kursteilnehmer des Kurses angezeigt.

* Markieren Sie einen oder mit "Strg + Mausklick" oder "Shift + Mausklick" mehrere Kursteilnehmer in der Detailansicht `Kursteilnehmer` und klicken Sie dann auf `Aus Kurs entfernen` und bestätigen Sie anschließend mit `Ja`. Die Teilnehmer werden aus dem Kurs entfernt.

## Kursteilnehmern Alternativkurse zuweisen

Sie können in der Ansicht `Kursplan > Blöcke` mit Hilfe von DAVINCI auf andere Kurse umverteilen. Sie können dabei die Umwahlmöglichkeiten aus der Sichtweise des Alternativkurses oder aus der Sichtweise eines Schülers betrachten.

![](/assets/images/KP/KP_Welche Kursteilnehmer passen in den Alternativkurs de2.png)

In diesem Beispiel wurde der Kurs „de1“ angeklickt. In der Detailansicht „Kursteilnehmer“ werden alle Kursteilnehmer angezeigt. Klicken Sie z.B. auf einen Alternativkurs, hier im Beispiel ist dies der Kurs „de2“. Jedes Mal wenn Sie einen Alternativkurs anklicken, werden die Kursteilnehmer markiert (siehe die vier markierten Teilnehmer oben), die problemlos in den Alternativkurs verschoben werden können. Klicken Sie auf In Kurs versetzen, wenn Sie diese Schüler in den Kurs „de2“ versetzen möchten.

So weisen einem oder mehreren Schüler einen Alternativkurs zu:

* Rufen Sie eine der Ansichten `Kursplan > Schüler`, `Kursplan > Kurse` oder `Kursplan > Blöcke` auf.

* Öffnen Sie die Detailansicht `Kursteilnehmer`.

* Klicken Sie in der Ansicht auf den gewünschten Kurs. In der Detailansicht `Kursteilnehmer` werden die Kursteilnehmer des Kurses angezeigt.

* Markieren Sie einen oder mit "Strg + Mausklick" oder "Shift + Mausklick" mehrere Kursteilnehmer in der Detailansicht Kursteilnehmer. Darunter werden Ihnen die entsprechenden Alternativkurse angezeigt. Kurse, die einen Schülerkonflikt verursachen (ein Schuler hat zwei Kurse im gleichen Block) werden durch das gelbe Konfliktsymbol gekennzeichnet. Die Anzahl der Konflikte werden in der Spalte „Schülerkonflikte“ ausgewiesen.

* Klicken auf den gewünschten Alternativkurs und dann auf In Kurs versetzen. Der bzw. die Schüler werden in den Alternativkurs versetzt. Aus der Sichtweise eines Schülers funktioniert das analog. Wenn man z.B. auf die Schülerin „Chet Baker“ klickt, werden die Alternativkurse markiert, die konfliktfrei zugeordnet werden können. In diesem Fall sind die beiden Alternativkurse „de2“ und „de3“ mit einem Widerspruchsymbol versehen, d.h. es gibt keinen möglichen Alternativkurs mehr.

[![Welche Alternativkurse kommen für Chet Baker in Frage?][8]][8]

!!! info "Hinweis"

    Dieses Verfahren können Sie auch auf den Registerkarten `Kurse-Blöcke` und `Schüler-Blöcke` anwenden. Alternativ, dann aber ohne Konflikthinweise, können Sie auch über `Start > Mehrfachzuweisung` mehreren Schülern einen neuen Kurs zuweisen.

## Kursteilnehmern einen weiteren Kurse zuweisen

In seltenen Fällen kann es Sinn machen, dem Schüler einen weiteren Kurs zuzuweisen, z.B. wenn Sie
einen Kurs dupliziert haben, der Kurs also aus zwei Veranstaltungszeilen bzw. zwei Kurszeilen besteht.
Gehen Sie dazu wie in Abschnitt 4.14 Kursteilnehmern Alternativkurse zuweisen beschrieben vor,
allerdings mit folgendem Unterschied: Klicken auf den gewünschten Alternativkurs und dann auf Kurs
zuordnen. Der bzw. die Schüler erhalten einen weiteren Kurs zugeordnet.

## Kursschnittmengen anzeigen

Kursschnittmengen bzw. Fachschnittmengen geben Hinweise darauf, welche Kurse eher zusammen geblockt werden, nämlich die mit kleiner oder möglichst leerer Schnittmenge bzw. wie viele Schüler ggf. umwählen müssen. Zu Anzeige der Kurs- bzw. Fachschnittmenge stehen Ihnen zwei Dialogfenster und die Ansicht `Kursplan > Blöcke` zur Verfügung. Über den Befehl Kursschnittmenge öffnet sich ein Dialogfenster, indem Sie mit "Strg + Maustaste" mehrere Kurse bzw. Fächer markieren können: die jeweilige Schnittmenge, also die Schüler die die gewählten Fächer bzw. Kurse gemeinsam in ihrer Fachwahl bzw. als Kurse haben, wird rechts angezeigt.

[![Kursschnittmenge]][9]][9]

Alternativ lässt sich über den Befehl Schnittmengen ein Dialogfenster öffnen, indem die Fächer bzw. Kurse an beiden Achsen gelistet sind. In den Tabellenzellen werden ggf. die Schnittmengen zwischen den beiden betreffenden Fächern bzw. Kursen angezeigt. Wenn sie die Option nur Schüleranzahl markieren, werden Ihnen nur die Teilnehmeranzahlen in der jeweiligen Schnittmenge angezeigt.

[![Schnittmengen]][10]][10]

[![Schnittmengen mit jeweiliger Anzahl der Schüler in der Schnittmenge]][11]][11]

Schnittmengen zwischen Kursen können Sie auch in der Ansicht `Kursplan > Blöcke` anzeigen. Voraussetzung dafür ist, dass die Kurse geblockt und die Schüler auf die Kurse verteilt sind.
Klicken Sie in der Ansicht `Kursplan > Blöcke` auf einen beliebigen Kurs und dann `Strg` auf einen beliebigen anderen Kurs. Im Zusatzfenster "Kursteilnehmer" werden für diese beiden gewählten Kurse die Schnittmenge der Schüler angezeigt.

[![Kursteilnehmer][7]][7]

So zeigen Sie die Teilnehmer der Kursschnittmenge an:

* Rufen Sie die Ansicht `Kursplan > Blöcke` auf.

* Öffnen Sie die Detailansicht `Kursteilnehmer`.

* Klicken Sie mit der Maus auf die gewünschten Kurse, deren Schnittmenge Sie anzeigen möchten. Die Kurse werden in der Detailansicht Kursteilnehmer als Komma getrennte Liste über der Teilnehmerliste angezeigt. Halten Sie während des Mausklicks die Strg-Taste gedrückt, um einen weiteren Kurs hinzuzufügen. Gleiches erreichen sie auch mit `Strg + Eingabe` oder `Shift + Eingabe` auf dem aktuell fokussierten Kurs. Die Kursschnittmenge, d.h. die Teilnehmer, die in allen gewählten Kursen sind, werden in der Detailansicht Kursteilnehmer angezeigt. Mit Mausklick auf einen anderen Kurs oder mit Eingabe-Taste können Sie die Kursliste wieder auf einen einzigen Kurs zurücksetzen.
