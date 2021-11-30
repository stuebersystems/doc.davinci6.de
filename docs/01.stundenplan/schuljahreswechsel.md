# Schuljahreswechsel

Nachfolgend werden die verschiedenen Optionen erläutert, die Ihnen beim Schuljahreswechsel zur Verfügung stehen:  

## Planvorbereitungsassistent

* **Neues Schuljahr** – Die Klassenkürzel werden von z.B. „8a“ in „9a“ u.s.w. umbenannt bzw. hoch gesetzt und die Klassen-IDs werden gelöscht. Bitte kontrollieren Sie an-schließend die Klassenkürzel.
* **Planwechsel innerhalb des Schuljahres** – Es werden keine weiteren Änderungen an den Stammdaten vorge-nommen.

![Planvorbereitungsassistent](/assets/images/stundenplan/07.png)

Nachdem Sie eine dieser Optionen gewählt haben, klicken Sie auf `Weiter`. Es werden Ihnen nun 2 Auswahlmöglichkeiten gegeben: 

* **Unterrichtsverteilung und Aufsichten löschen** – Wenn Sie diese Option wählen, werden nur die Stammdaten übernommen. Wahlweise können auch die Soll/Ist-Differenzen aus dem Vorjahr übernommen werden. Richten Sie dazu im `Schlüsselverzeichnis > Lehrer-Soll-Schlüssel` einen neuen Schlüssel mit dem Typ „D“ ein, den Sie beispielsweise „Übertrag aus letztem Schuljahr“ nennen. Richten Sie diesen Schlüssel noch im alten Plan, also vor der Datenübernahme, ein.
* **Alles übernehmen** – Wenn Sie diese Option wählen, werden die Stammdaten, die Unterrichtsverteilung, die Aufsichten und die gesetzten Pläne übernommen.

![Planvorbereitungsassistent](/assets/images/stundenplan/08.png)

Nachdem Sie nun eine dieser Optionen gewählt haben, klicken Sie auf `Weiter`. Es werden Ihnen nun 3 Schritte genannt, die Sie durchführen müssen.

![Planvorbereitungsassistent](/assets/images/stundenplan/09.png)

* **Zeitraum eingeben** – Über diese Schaltfläche gelangen Sie zu den Planeigenschaften. Ändern Sie im Register „Zeitraum“ das Anfangs- und Enddatum für Ihren neuen Plan und bearbeiten Sie gegebenenfalls die Registerkarte „Statistik“ die Wochen. 

* **Kalenderdaten importieren** – Über diese Schaltfläche können Sie den Ferienkalender für Ihr Bundesland impor-tieren, der in daVinci zur Verfügung steht. 

* **Zeitrahmen einstellen** - Für die Verplanung Ihrer Unterrichtstermine steht Ihnen ein Stundenraster zur Verfügung. Dieses Stundenraster wird durch die Unterrichtsstunden gebildet, deren Anzahl und Dauer Sie im Zeitrahmen festlegen. Gemeinsam mit den Unterrichts- und Pausenzeiten geben diese Angaben den Zeitrahmen vor, der Ihnen für die Terminplanung in den Wochenstundenplänen zur Verfügung steht. Bitte prüfen Sie die Eintragungen.

Passen Sie dann die Stammdaten an die neuen Gegebenheiten an (z.B. Klassen umbenennen, Klassen löschen oder neu anlegen usw.). Speichern Sie die neue Datei unter einem gewünschten Namen ab (standardmäßig wird von uns der Name "NeuerPlan.daVinci" vorgegeben).

## Gesetzte Termine löschen

Möchten Sie die gesetzten Termine Ihres Planes ganz oder teilweise löschen, können Sie dies wie folgt durchführen:

* **Alle Termine einer/aller Klassen löschen** – Unter der Menügruppe `Automatik > Verplanungen zurücksetzen` oder unter `Start > Veranstaltungen > Löschen > Verplanungen zurücksetzen` können Sie gesetzte Termine aus dem Plan entfernen.
* **Verschiedene Termine aus Plänen löschen** – Um einen bestimmten oder mehrere Termine wieder aus dem Plan zu entfernen, führen Sie bitte folgende Schritte aus:
  
1. Markieren Sie das Terminfeld des zu entfernenden Termins.
2. Betätigen Sie in der Menüleiste `Start > Stundenplan` die Schaltfläche `Eintrag entfernen`. Der Termin wird nun aus dem Planungsfenster entfernt und befindet sich wieder in der Terminliste des „Unverplant“-Fensters.

![Termin entfernen](/assets/images/stundenplan/10.png)

## Veranstaltungen kopieren

In der Regel wird für eine Klasse eine Stundentafel angelegt und in den Stammdaten auf der Registerkarte `Klassen` in der Spalte „Stundentafel“ zugewiesen. Danach wird im Planungseditor `Start > Stundenplan` die Funktion `Neu > Aus Stundentafel erzeugen` durchgeführt.

Sie haben aber auch die Möglichkeit lediglich die Stundentafel in den Stammdaten zuzuweisen und ausgewählte Veranstaltungen einer Klasse in die Veranstaltungsliste einer anderen Klasse zu kopieren.

Gehen Sie dazu bitte folgendermaßen vor: 

1. Markieren Sie die gewünschten Veranstaltungen in der Veranstaltungsliste.
2. Klicken Sie in der Menügruppe `Start > Veranstaltungen` auf die untere Hälfte der Schaltfläche `Neue Veranstaltung`.
3. Wählen Sie den Befehl `Veranstaltungen kopieren` aus dem Aufklappmenü.
4. Wählen Sie im Dialogfenster `Veranstaltungen kopieren` die Klasse, in deren Veranstaltungsliste kopiert werden soll, aus dem Aufklappmenü des Feldes `In folgende Klasse kopieren`.
5. Setzen Sie den Haken in den Kontrollfeldern vor „Ohne Lehrer“ bzw. „Ohne Raum“ um die Veranstaltung mit der vorgenommenen Lehrer- und/ oder Raumzuweisung zu übernehmen.
6. Aktivieren Sie ggf. für geblockte Veranstaltungen die gewünschte Option für das Kopieren der Blockinformationen:
   
* **Gleiche Blöcke** - Kopiert die ausgewählten Veranstaltungen mit dem gleichen Blockkürzel in die Zielklasse
   
* **Neue Blöcke** - Kopiert die ausgewählten Veranstaltungen mit dem gleichen Blockkürzel in die Zielklasse
  
* **Ohne Blocknummer** - Kopiert die ausgewählten Veranstaltungen ohne Blockkürzel in die Zielklasse

Bestätigen Sie Ihre Einstellungen mit OK. 
Die ausgewählten Veranstaltungen werden nun in die Zielklasse übertragen. 

![Blockinformationen](/assets/images/stundenplan/11.png)

## Änderungen in der Stundentafel

Wenn sich die Stundentafel einer Klasse von einem zum nächsten Schuljahr nur geringfügig verändert, müssen Sie nicht zwingend die Funktion `Aus Stundentafel erzeugen` nutzen und eine neue Unterrichtsverteilung für die Klasse erstellen. Sie haben auch die Möglichkeit in den Stammdaten die Stundentafel umzubenennen (wenn das nötig ist) und zu verändern. Die Zuordnung zur Klasse geht dadurch nicht verloren. In der Unterrichtsverteilung werden die Änderungen dann in der Spalte „Soll/Ist“ sichtbar. Nun müssen Sie in der Unterrichtsverteilung entsprechend Ihrer Veränderungen die Dauer anpassen, Fächer hinzufügen oder löschen. Der Vorteil an dieser Variante ist, dass die Lehrer- und Raumzuweisungen, die Blockungen usw. nicht verloren gehen.

## Perioden

Zunächst müssen Sie in den `Plan-Eigenschaften > Statistik` unter `Wochenbezogene Summen` die Wochen bearbeiten und eingeben welche Wochen Unterrichtswochen und welche Ferienwochen im neuen Schuljahr sind.
Danach bearbeiten Sie die Perioden in den Stammdaten und passen diese an die neuen Gegebenheiten an.
Wenn Sie bereits Perioden in den Unterrichtsverteilungen zugewiesen haben, sollten Sie als nächstes im Stammdatenfenster unter `Start > Bearbeiten > Wochen aktualisieren…` durchführen. Bitte führen Sie anschließend unter `Extras > Plandatei aufräumen` durch und speichern Sie die Datei ab. Dadurch werden die evtl. entstandenen Überschneidungen entfernt.

## Weitere nützliche Optionen im Planfenster

In der Menügruppe `Start > Veranstaltungen > Löschen` stehen Ihnen folgende Optionen zur Auswahl:

![Löschen](/assets/images/stundenplan/12.png)

* **Raumvorgabelisten löschen** - Die Raumvorgabelisten der ausgewählten Veranstaltungen werden nun aus der Veranstaltungsliste entfernt.
* **Raumzuweisungen entfernen** - Die Raumzuweisungen der ausgewählten Veranstaltungen werden nun aus dem gesetzten Plan entfernt.
* **Lehrerzuweisungen entfernen** - Die zugewiesenen Lehrer werden bei den ausgewählten Veranstaltungen aus dem Plan entfernt.
* **Zeitzuweisungen entfernen** – Ein verplanter Termin wird aus dem Planfenster entfernt und muss nun wieder neu in den Plan gesetzt werden

