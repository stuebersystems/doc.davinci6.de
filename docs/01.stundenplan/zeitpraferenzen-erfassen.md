# Zeitpräferenzen erfassen

Zeitpräferenzen geben an, ob bestimmte Zeitpositionen im Plan für eine Klasse, einen Lehrer, einen Raum, ein Fach oder eine Veranstaltung verfügbar sein soll oder nicht. Dabei unterscheidet DAVINCI zwischen Sperrungen und Kernzeiten:

* **Sperrung:** Mit einer Sperrung legen Sie fest, dass an einer Stundenplanposition kein Unterricht verplant werden darf oder soll. Für jede Sperrung können Sie vier Gewichtungsstufen vergeben. Diese Gewichtungsstufen werden von der Setzautomatik abgestuft berücksichtigt. Eine Sperrung der Stufe „1“ genießt für die Automatik absoluten Charakter, d.h. die Automatik darf an die gesperrten Stellen keinen Unterricht platzieren. Sperrungen der Rangstufen „2“ bis „4“ besitzen für die Automatik bedingt normativen Charakter, d.h. die Automatik versucht an die gesperrten Termine keinen Unterricht zu platzieren. Falls die Automatik aber keine andere Lösung findet den Unterricht zu verplanen, als diesen an die bedingt gesperrten Positionen zu setzen, werden diese Positionen in die Unterrichtsplanung mit einbezogen. Je niedriger dabei die zugewiesene Zahl, desto höher ist das Gewicht der eingetragenen Sperrung und desto weniger ist die Automatik geneigt gegen eine Sperrung zu verstoßen.

* **Kernzeit:** Mit einer Kernzeit legen Sie fest, dass an einer Stundenplanposition bevorzugt Unterricht verplant werden soll. Für jede Kernzeit können Sie wiederum vier Gewichtungsstufen vergeben. Diese Gewichtungsstufen werden von der Setzautomatik abgestuft berücksichtigt. Kernzeiten der verfügbaren Rangstufen „1“ bis „4“ genießen grundsätzlich keinen absoluten, sondern nur bedingt normativen Charakter; d.h. die Automatik versucht an die gekennzeichneten Termine bevorzugt Unterricht zu platzieren. Je niedriger dabei die zugewiesene Zahl, desto höher ist das Gewicht der eingetragenen Kernzeit und desto eher ist die Automatik geneigt den Unterricht an die so ausgewiesenen Planpositionen zu platzieren.

!!! info "Hinweis"

    Kernzeiten und Sperrungen genießen für das manuelle Planen grundsätzlich nur informativen Charakter, d.h. der individuelle Planer kann an eine gesperrte Planposition egal welcher Rangstufe z.B. per Drag & Drop Unterricht platzieren. Sperrungen der Kategorie „1“ werden im Rahmen der Überschneidungsprüfung beim manuellen Setzen als absolute Sperrungen angesehen und als Zeitkonflikt angezeigt. 

## Zeitpräferenzen eingeben

Rufen Sie in der Ansicht „Stundenplan“ den gewünschten Plan der Klasse, des Lehrers, des Fachs oder des Raums auf. Um Positionen für eine Klassen, einen Lehrer, einen Raum oder ein Fach zu sperren:

* Klicken Sie auf `Start > Zeitpräferenzen` und das Dialogfenster „Zeitpräferenzen“ aufzurufen oder gehen Sie wie in den folgenden Abschnitten beschrieben vor.

Um Positionen für eine Veranstaltung zu sperren:

1. Rufen Sie in der Ansicht „Stundenplan“ den gewünschten Plan der Klasse, des Lehrers, des Fachs oder des Raums auf und klicken Sie auf `Start > Veranstaltung bearbeiten` , um das Veranstaltungsfenster aufzurufen.

2. Klicken Sie im Veranstaltungsfenster auf „Zeitdetails“. In dieser Ansicht sehen Sie die Liste der Zeitpräferenzen für die betreffende Veranstaltung. Über die Schaltflächen `Neu` und ``Bearbeiten`` können Sie das Dialogfenster „Zeitpräferenzen“ aufzurufen. Über `Löschen` können Sie Zeitpräferenzen löschen.

!!! info "Hinweis"

    Das Eintragen von Kernzeiten/ Sperrungen nur für bestimmte Kalenderwochen bzw. Tage erfordert eine Lizenz für das DAVINCI Zusatzmodul JAHRESTERMINE.

## Sperrung für einen Plan eintragen

Um für einen bestimmten Einzelplan eine Sperrung erfassen, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie den gewünschten Einzelplan in der Ansicht „Stundenplan“ auf.
2. Markieren Sie den zu sperrenden Zeitraum, indem Sie mit der linken Maustaste auf die Startposition klicken und den Mauszeiger bei gedrückter linker Maustaste bis zur Endposition des Zeitraums bewegen.
3. Lassen Sie die linke Maustaste los und klicken Sie anschließend auf die rechte Maustaste. Wählen Sie den Befehl `Neue Sperrung` aus dem Kontextmenü.
4. Lassen Sie im Feld „Art/ Kategorie“ des erscheinenden Dialogfensters den Eintrag „Sperrung“
voreingestellt.
5. Stellen Sie im Gewichtungsfeld neben „Art/ Kategorie“ die gewünschte Rangstufe der Sperrung
ein.
6. Wählen Sie im Feld „Wiederholung“ den Eintrag „Periodisch“ aus dem Aufklappmenü, um festzulegen, dass die Sperrung für alle Unterrichtswochen des Planungszeitraums gilt.

Oder

Wählen Sie im Feld „Wiederholung“ den Eintrag „Einmalig“ aus dem Aufklappmenü, um festzulegen, dass die Sperrung nur für die aktuelle Kalenderwoche gilt. Lassen Sie in den Tages- bzw. Datums sowie Positions- und Uhrzeitfeldern neben ``Beginnt`` und ``Endet`` den Start und Endzeitpunkt gemäß der gewählten Markierung voreingestellt.

!!! info "Hinweis"

    Das Eintragen von Kernzeiten bzw. Sperrungen für bestimmte Tage bzw. Kalenderwochen erfordert eine Lizenz für das DAVINCI Zusatzmodul JAHRESTERMINE.

Oder

Korrigieren Sie den Start- und Endzeitpunkt des Sperrzeitraums durch manuelle Eingabe in den genannten Feldern neben „Beginnt“ und „Endet“ bzw. durch das Setzen des Hakens im Kontrollkästchen vor „Ganztägig“. Bestätigen Sie Ihre Angaben mit `OK`.

![Sperrung anlegen](/assets/images/sperrung.png)

Im Dialogfenster "Neue Zeitpräferenz" können Sie Sperrungen eintragen. Die eingetragene Sperrung wird nun im Planungsfenster angezeigt. Gesperrte Planpositionen werden durch eine Schraffur sowie ein X links oben im zugehörigen Terminfeld markiert. Sperrungen der Rangstufe 1 werden dabei durch ein allein stehendes X, Sperrungen der Rangstufen 2 bis 4 zusätzlich durch den Wert der Rangstufe neben dem X gekennzeichnet.

![Sperrung anzeigen](/assets/images/sperrung1.png)

## Kernzeit für einen Plan eintragen

Zum Eingeben von Kernzeiten gehen Sie analog zum Eingeben von Sperrungen vor, indem Sie im Stundenplan die gewünschten Positionen markieren und im  Kontextmenü ``Rechte Maus > Neue Kernzeit`` auswählen.

!!! info "Hinweis"

    Das Eintragen von Kernzeiten/Sperrungen nur für bestimmte Kalenderwochen erfordert eine Lizenz für das DAVINCI Zusatzmodul JAHRESTERMINE.

![Kernzeit anlegen](/assets/images/kernzeit.png)

Im Dialogfenster "Neue Zeitpräferenz" können Sie Kernzeiten eintragen. Die eingetragene Kernzeit wird mit einem Unterstrich gefolgt von der Kategorieangabe im Stundenplan angezeigt.

![Kernzeit anzeigen](/assets/images/kernzeit1.png)

### Sperrung eintragen

Um für einen bestimmten Einzelplan eine Sperrung erfassen, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie den gewünschten Einzelplan auf.
2. Markieren Sie den zu sperrenden Zeitraum, indem Sie mit der linken Maustaste auf die Startposition klicken und den Mauszeiger bei gedrück-ter linker  Maustaste bis zur Endposition des Zeitraums bewegen.
3. Lassen Sie die linke Maustaste los und klicken Sie anschließend auf die rechte Maustaste.
4. Wählen Sie den Befehl Neue Sperrung aus dem Kontextmenü.
5. Lassen Sie im Feld „Art/ Kategorie“ des erscheinenden Dialogfensters den Eintrag „Sperrung“ voreingestellt.
6. Stellen Sie im Gewichtungsfeld neben „Art/ Kategorie“ die gewünschte Rangstufe der Sperrung ein.
7. Wählen Sie im Feld „Wiederholung“ den Eintrag „Periodisch“ aus dem Auf-klappmenü, um festzulegen, dass die Sperrung für alle Unterrichtswochen des Planungszeitraums gilt.

**Oder**
Wählen Sie im Feld „Wiederholung“ den Eintrag „Einmalig“ aus dem Auf-klappmenü, um festzulegen, dass die Sperrung nur  für die aktuelle Kalenderwoche gilt

!!! info "Hinweis"

    Das Eintragen von Sperrungen nur für bestimmte Kalenderwochen erfordert eine Lizenz für das Zusatzmodul JAHRESTERMINE.

8. Lassen Sie in den Tages- bzw. Datums sowie Positions- und Uhrzeitfeldern neben „Beginnt“ und „Endet“ den Start und Endzeitpunkt gemäß der ge-wählten Markierung voreingestellt.  **Oder** Korrigieren Sie den Start- und Endzeitpunkt des Sperrzeitraums durch manuelle Eingabe in den genannten Feldern neben „Beginnt“ und „Endet“ bzw. durch das Setzen des Hakens im Kontrollkästchen vor „Ganztägig“.

![Im Dialogfenster "Neue Zeitpräferenz" können Sie Sperrungen eintragen.](/assets/images/Sperrung.png)

9. Bestätigen Sie Ihre Angaben mit ``OK``.

Die eingetragene Sperrung wird nun im Planungsfenster angezeigt. Gesperrte Planpositionen werden durch eine Schraffur sowie ein X links oben im zugehörigen Terminfeld markiert. Sperrungen der Rangstufe 1 werden dabei durch ein allein stehendes X, Sperrungen der Rangstufen 2 bis 4 zusätzlich durch den Wert der Rangstufe neben dem X gekennzeichnet.

![Anzeige von Sperrungen](/assets/images/Sperrung01.png)

### Kernzeit eintragen

Um für einen bestimmten Einzelplan eine Kernzeit zu erfassen, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie den gewünschten Einzelplan auf.
2. Markieren Sie den zu sperrenden Zeitraum, indem Sie mit der linken Maustaste auf die Startposition klicken und den Mauszeiger bei gedrückter linker  Maustaste bis zur Endposition des Zeitraums bewegen.
3. Lassen Sie die linke Maustaste los und klicken Sie anschließend auf die rechte Maustaste.
4. Wählen Sie den Befehl ``Neue Kernzeit`` aus dem Kontextmenü.
5. Lassen Sie im Feld ``Art/ Kategorie`` des erscheinenden Dialogfensters den Eintrag ``Kernzeit`` voreingestellt.
6. Stellen Sie im Gewichtungsfeld neben ``Art/ Kategorie`` die gewünschte Rangstufe der Kernzeit ein.
7. Wählen Sie im Feld ``Wiederholung`` den Eintrag ``Periodisch`` aus dem Aufklappmenü, um festzulegen, dass die Kernzeit für alle Unterrichtswochen des Planungszeitraums gilt.
**Oder** Wählen Sie im Feld ``Wiederholung`` den Eintrag ``Einmalig`` aus dem Aufklappmenü, um festzulegen, dass die Kernzeit nur  für die aktuelle Kalenderwoche gilt.

!!! info "Hinweis"

    Das Eintragen von Kernzeiten nur für bestimmte Kalenderwochen erfordert eine Lizenz für das Zusatzmodul JAHRESTERMINE.

8. Lassen Sie in den Tages- bzw. Datums sowie Positions- und Uhrzeitfeldern neben ``Beginnt`` und ``Endet`` den Start und Endzeitpunkt gemäß der gewählten Markierung voreingestellt.  **Oder** Korrigieren Sie den Start- und Endzeitpunkt des Kernzeitraums durch manuelle Eingabe in den genannten Feldern neben ``Beginnt`` und ``Endet`` bzw. durch das Setzen des Hakens im Kontrollkästchen vor ``Ganztägig``.

![Im Dialogfenster "Neue Zeitpräferenz" können Sie neben Sperrungen auch Kernzeiten eintragen](/assets/images/Kernzeit.png)

9. Bestätigen Sie Ihre Angaben mit ``OK``.

Die eingetragene Kernzeit wird nun im Planungsfenster angezeigt. Kernzeiten werden durch ein grünes Terminfeld sowie den Wert der Rangstufe neben dem _ gekennzeichnet.

![Kernzeit](/assets/images/Kernzeit01.png)

## Räume für ein bestimmtes Team reservieren

Im Rahmen des Erfassens von Kernzeiten für Räume haben Sie außerdem die Option, Räume für ein bestimmtes Team zu reservieren und dadurch gleichzeitig für andere Teams zu sperren.

Erfassen Sie dazu für den gewünschten Raum eine Kernzeit der Rangstufe „1“ und wählen Sie im Dialogfenster „Neue Zeitpräferenz“  das  gewünschte Team aus dem Aufklappmenü des Feldes „Team“. Die eingetragene Kernzeit wird nun im Planungsfenster angezeigt. Das Kürzel des zugewiesenen Teams wird dabei in Klammern neben der Rangstufe der Kernzeit angezeigt.  

![Team](/assets/images/Kernzeit02.png)

## Sammelzuweisung

In den Stammdaten für Klassen, Lehrer, Räume, Fächer haben Sie die Möglichkeit über `Start > Bearbeiten > Zeitpräferenzen` diese auch als Sammelzuweisung für alle zuvor markierten zuzuweisen.
