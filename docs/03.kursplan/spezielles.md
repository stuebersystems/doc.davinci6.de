
# Spezielles

[1]:/assets/images/KP/spezielles_01.png
[2]:/assets/images/KP/spezielles_02.png
[3]:/assets/images/KP/spezielles_03.png
[4]:/assets/images/KP/spezielles_04.png
[5]:/assets/images/KP/spezielles_05.png

## Aufgestockte Grundkurse

Aufgestockte Grundkurse werden dann eingerichtet, wenn die Schüleranzahl für einen Leistungskurs zu gering ist. Nehmen wir an, im Latein Grundkurs „la1“ sind 10 Schüler und im Leistungskurs „LA1“ sind nur 5 Schüler. Der Leistungskurs muss wegen zu geringer Schülerzahl mit dem Grundkurs zusammengelegt werden, d.h. der Grundkurs „la1“ wird zum aufgestockten Grundkurs. Der Grundkurs wird 3stündig und der Leistungskurs 5stündig unterrichtet. Geben Sie einen 3stündigen Grundkurs „la1“ mit 15 Schülern (Leistungs- und Grundkursschüler) ein und markieren Sie den Kurs als aufgestockten Grundkurs, indem Sie in der Ansicht `Kursplan > Kurse` den Grundkurs in Spalte "Fachstatus" mit dem Eintrag "AufgstGK" versehen. Grundlage bildet das Schlüsselverzeichnis "Fachstatus", hier muss "AufgstGK" definiert sein. Dem dazugehörigen Leistungskurs muss die Unterrichtsart "LK" zugewiesen sein.

!!! info "Hinweis"

    Unter `Extras > Schlüsselverzeichnis > Fachstatus` können Sie beim „Fachstatus“ für das Kürzel „AufgstGK“ eine Farbe einstellen. Der aufgestockte Grundkurs wird dann in der Ansicht `Kursplan > Schüler` entsprechend farblich dargestellt.

[![Schlüsselverzeichnis "Fachstatus"][1]][1]

!!! info "Hinweis"

    Sie müssen den Leistungskursschülern sowohl den Leistungskurs „LA1“ 2stündig als auch den aufgestockten Grundkurs „la1“ 3stündig zuordnen. Diesen Grundkurs weisen Sie über die Ansicht `Kursplan > Fachwahlen` zu.

Der Grundkurs liegt dann ganz normal mit seinen 3 Stunden parallel zu anderen Grundkursen in einem bestimmten Band, der zugehörige Lk mit seinen 2 Stunden in einem Band der Leistungskurse.
Durch die Markierung des Grundkurses als aufgestockter Grundkurs und durch die gleiche Kursnummer achtet die Automatik darauf, dass Grundkurs und Leistungskurs am Tag nicht doppelt verplant werden. Zudem werden die Schülerzahlen für Statistikzwecke entsprechend dem Leistungskurs- bzw. dem Grundkursbereich zugeordnet (abhängig von den Vorgaben der Landesstatistik).

## Neues Schuljahr mit Oberstufe

Die Kursplanung der Oberstufenschüler soll in die Plandatei für das neue Schuljahr übernommen werden. Bitte beachten Sie dazu folgende Vorgehensweise in der Planneuerstellung. 

1. Rufen Sie dazu über `Plan > Neu` den Planvorbereitungsassistenten auf.
2. Ihnen stehen drei Wege zur Verfügung. Wählen Sie bitte ``Neuen Plan erstellen und Daten übernehmen`` und wählen Sie Ihre Vorjahresplandatei aus.

[![Neuen Plan erstellen und Daten übernehmen][2]][2]

3. Klicken Sie auf `Weiter`.

4. Wählen Sie hier bitte `Neues Schuljahr`. Ihre Klassenkürzel werden umbenannt und die Klassenstufe wird erhöht.

[![Option "Neues Schuljahr"][3]][3]

5. Im nächsten Fenster wählen Sie unbedingt `Alles übernehmen`. Veranstaltungen, gesetzte Pläne, Aufsichten und die Kurszuweisung in der gymnasialen Oberstufe werden übernommen. 
6. Klicken Sie auf `Weiter`. Es wird Ihnen eine Liste aufgezeigt, die Sie bitte Schritt für Schritt durchgehen.
7. Speichern Sie die neue Datei unter einem gewünschten Namen ab.

### Stammdatenfenster

Passen Sie im Stammdatenfenster Ihre Stammdaten an die neuen Gegebenheiten an. Die Klassenkürzel wurden bereits umbenannt, die Klassenstufe erhöht. Bitte kontrollieren Sie noch einmal Ihre Klassenkürzel.

!!! info "Hinweis"

    Eintragungen in den Felder "Lehrer 1", "Lehrer 2" sowie "Raum" müssen ggf. auch aktualisiert werden.

[![Menü Stammdaten][4]][4]

#### Stammdatenfenster "Schüler"

Löschen Sie hier die Schüler der Klasse "14", diese haben bereits Ihre Schule verlassen.

[![Stammdatenfenster "Schüler"][5]][5]

#### Stammdatenfenster "Klassen"

Löschen Sie anschließend im Stammdatenfenster "Klassen" die Klasse 14.

### Bereich Stundenplan

#### Gesetzte Termine löschen

Haben Sie im Planvorbereitungsassistenten die Daten aus der Vorjahresplandatei übernommen, können Sie die gesetzten Termine Ihres Planes ganz oder teilweise löschen.

Gehen Sie dazu wie folgt vor:

**Alle Termine einer/aller Klassen löschen**

Unter der Menügruppe `Automatik > Verplanungen zurücksetzen` oder unter `Start > Veranstaltungen > Löschen > Verplanungen zurücksetzen` können Sie gesetzte Termine aus dem Plan entfernen.

**Verschiedene Termine aus Plänen löschen**

Um einen bestimmten oder mehrere Termine wieder aus dem Plan zu entfernen, führen Sie bitte folgende Schritte aus:

1. Markieren Sie das Terminfeld des zu entfernenden Termins.
2. Betätigen Sie in der Menüleiste `Start > Stundenplan`  die Schaltfläche `Eintrag entfernen`.
3. Der Termin wird nun aus dem Planungsfenster entfernt und befindet sich wieder in der Terminliste des „Unverplant“-Fensters.

### Bereich Kursplan

Im Bereich  `Kursplan > Kurse` und `Kursplan > Blöcke` wurden die Blockbezeichnungen automatisch an die neue Klassenstufe angepasst. Der Block ``12#01`` wurde auf Block ``13#01`` hochgesetzt.
