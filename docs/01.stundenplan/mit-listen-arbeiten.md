# Mit Listen arbeiten

Die meisten Listen in DAVINVI (Stammdatenfenster, Veranstaltungsliste im Stundenplanbereich) verfügen über einige sehr nützliche Funktionen, mit denen Sie dieListendarstellung an Ihre situativen Arbeitserfordernisse anpassen können.

Sie können:

* mehrere Einträge einer Liste auswählen
* einzelne Spalten ein- und ausblenden
* einzelne Spalten an eine andere Stelle verschieben
* einzelne Zeilen an eine andere Stelle verschieben

Sie können die ganze Liste:

* nach einer bestimmten Spalte sortieren
* nach bestimmten Spalteninhalten filtern
* nach bestimmten Spalteninhalten gruppieren

## Benutzerdefinierte Filter

Klicken Sie auf das Filtersymbol und wählen Sie aus der Liste den Eintrag „(Benutzerdefiniert…)“`, es erscheint das Dialogfenster „Benutzerdefinierter Filter“, in dem Sie einen Filter erzeugen können.

![die Liste filtern](/assets/images/listefiltern1.png)

Geben Sie in das obere Textfeld den Suchbegriff ein und wählen Sie ein Suchattribut (z.B.: "wie") aus. Sie können einen weiteren Suchbegriff hinzufügen um nach zwei Suchbegriffen gleichzeitig zu filtern. In diesem Fall wählen Sie zwischen der Verknüpfung

* ```UND``` - Beide Suchbegriffe müssen im Zelleninhalt enthalten sein
* ```ODER``` - Mind. einer von beiden Suchbegriffen muss im Zellinhalt enthalten sein

* ```gleich``` - Suchbegriff und Zellinhalt der Spalte müssen identisch sein.
* ```nicht gleich``` -  Suchbegriff und Zellinhalt der Spalte dürfen nicht identisch sein.
* ```ist kleiner als``` -  Der Suchbegriff muss weniger Zeichen bzw. einen geringeren Zahlenwert haben als der Zellinhalt.
* ```ist kleiner oder gleich``` - Der Suchbegriff muss weniger oder dieselbe Anzahl Zeichen bzw. einen kleineren oder den gleichen Zahlenwert haben wie der Zellinhalt.
* ```ist größer als``` - Der Suchbegriff muss mehr Zeichen bzw. einen größeren Zahlenwert haben als der Zellinhalt.
* ```ist größer oder gleich``` -  Der Suchbegriff muss mehr oder dieselbe Anzahl an Zeichen bzw. einen größeren oder gleichen Zahlenwert haben wie der Zellinhalt.
* ```wie``` - Der Zellinhalt enthält dieselbe Zeichenfolge wie der Suchbegriff.
* ```nicht wie``` - Der Zellinhalt enthält nicht dieselbe Zeichenfolge wie der Suchbegriff.
* ```ist leer``` - Die Zelle muss leer sein.
* ```ist nicht leer``` -  Die Zelle darf nicht leer sein

Um den erzeugten Filter zu aktivieren, bestätigen Sie mit ```OK```. Die Liste, für die der Filter erstellt wurde, zeigt nun die zutreffenden Einträge.

![Benutzerdefinierter Filter](/assets/images/Benutzerdefinierter Filter01.png)

## Einträge in die Zwischenablage kopieren

Sie können in allen Listen ganze Zeilen in die Windows-Zwischenablage kopieren. Die in die Zwischenablage kopierten Einträge können in anderen Programmen z.B. Excel oder Word wieder einfügt werden. Markieren Sie die entsprechenden Zeilen und wählen ```In Ablage kopieren```.
  
Sie können umgekehrt auch Zeilen aus der Zwischenablage einfügen. Die Einträge aus der Zwischenablage können z.B. aus Excel oder Word stammen,  müssen jedoch die gleichen Spaltenreihenfolge wie in DaVinci aufweisen, wobei die Felder in der Zeile mit `Tab`getrennt werden müssen.

![In Ablage kopieren](/assets/images/kopieren.png)

Sie können umgekehrt auch Zeilen aus der Zwischenablage einfügen. Die Einträge aus der Zwischenablage können z.B. aus Microsoft Excel oder Microsoft Word stammen müssen jedoch die gleichen Spaltenreihenfolge wie in daVinci aufweisen. Kopieren Sie die Zeilen zunächst und wählen dann die entsprechende Stammdatenliste. Dort wählen Sie `Start > Aus Ablage einfügen`.

Mit der Schaltfläche `Aus Ablage einfügen` können Sie Einträge aus der Zwischenablage
einfügen

![Aus Ablage einfügen](/assets/images/einfügen.png)

!!! info "Hinweis"

    Hinweis: Beim Kopieren aus der Windows-Zwischenablage müssen Sie darauf achten, dass die Reihenfolge der Spalteninhalte die gleiche ist, wie in der DaVinci Tabelle, in die Sie kopieren! Es können nur textbasierte Zellen kopiert werden, also z.B. keine Symbole, Farben, Optionsfelder usw. 

## Eintrag löschen

Um einen Eintrag aus einer Stammdaten-Liste zu entfernen, müssen Sie die zugehörige Zeile löschen. Markieren Sie dazu die Zeile mit einem Linksklick und gehen Sie auf `Start > Löschen` oder klicken Sie mit Rechts in die Zeile und wählen `Zeile löschen`. Mit `Strg+Mausklick` und `Umschalt+Mausklick` können Sie auch mehrere Zeilen gleichzeitig markieren und löschen.

![Eintrag löschen](/assets/images/ListeBearbeitenLöschen.png)

!!! warning "Wichtig"

    Wenn Sie Einräge in DaVinci Löschen, werden Sie immer vom Programm gefragt, ob Sie das gewählte Objekt wirklich löschen möchten. Wenn Sie dieses mit ``OK`` löschen, ist es aus der Datei gelöscht. Eine Rückgängig-Machen Taste gibt es in DaVinci nicht.

## Feldinhalte kopieren

Sie können einen Zelleninhalt einer Tabelle aus einer Zeile auf mehrere andere bzw. alle anderen Zeilen übertragen, solange es sich um dieselbe Spalte handelt. Klicken Sie dazu in die gewünschte Zelle von der Sie den Inhalt kopieren möchten und klicken Sie auf ``Rechte Maustaste`` und dann auf ``Feldinhalt in Ablage kopieren``. Markieren Sie dann eine oder mehrere Zielzeilen (mit ``Strg+A``, ``Strg+ Mausklick`` bzw, ``Shift+Mausklick`` wie oben beschrieben), in die Sie den Wert übernehmen wollen und klicken Sie auf ``Feldinhalt aus Ablage einfügen``.

!!! info "Hinweis"

    Mit ``Feldinhalt in Ablage kopieren`` und ``Feldinhalt aus Ablage einfügen`` können Sie schnell und bequem Serienänderungen in Listen durchführen. 

## Liste bearbeiten

![Aufruf "Liste bearbeiten" aus dem Stammdatenfenster heraus](/assets/images/ListeBearbeiten01.png)

Der Inhalt von Listen in den verschiedenen DaVinci Ansichten kann nur dann verändert werden, wenn die Schaltfläche Liste bearbeiten aktiviert ist. Dies verhindert ungewolltes Verändern des Inhalts. 

## Listen drucken

![Drucken](/assets/images/drucken.png)

Sie können alle Listen in der eingestellten Ansicht (z.B. gruppiert, sortiert) direkt ausdrucken oder daraus ein PDF erstellen. Wählen Sie dazu z.B. ```Start > Drucken`` in der Ansicht "Stammdaten". Verwechseln Sie diese Schaltfläche nicht mit der gleichnamigen unter ``Publizieren``, über die Sie Stundenpläne, Unterrichtsverteilungen und Vertretungslisten drucken können. Um ein PDF-Dokument zu erstellen, klicken Sie auf ``Drucken > Vorschau`` und dann auf ``Nach PDF exportieren```.

## Listen filtern

Sie haben die Möglichkeit eine ganze Liste nach einzelnen oder mehreren Spalten zu filtern. Das Filtern führt dazu, dass nur die Einträge angezeigt werden, auf die der gewählte Filter passt. Dabei stehen Ihnen zwei Wege zur Verfügung, um den Filter an Ihre Bedürfnisse anzupassen.

1. Filtern nach ganzen Zellinhalten
2. Filtern nach einer benutzerdefinierten Kombination von Merkmalen

Sie können beliebig viele Filter auf eine Liste anwenden und miteinander kombinieren. Die aktuell gesetzten Filterparameter erscheinen in einem blauen Balken am unteren Rand des Listenfensters. Um den gesetzten Filter zu entfernen, betätigen Sie einfach die hellblaue Schließen-Schaltfläche (Kreuz links). Um den Filter direkt anzupassen (z.B.: einzelne Spalteninhalte wieder abwählen) können Sie auch die Schaltfläche „Anpassen…“ benutzen.

## Listen sortieren

Sie haben die Möglichkeit, eine gesamte Liste nach einzelnen oder mehreren Spalten zu sortieren. Sortiert wird alphanummerisch, also nach Buchstaben und/oder Zahlen auf- und absteigend.
Um eine Liste nach einer einzelnen Spalte zu sortieren, klicken Sie mit der linken Maustaste auf den Kopf der Spalte, nach der sortiert werden soll. Der erscheinende Pfeil im Spaltenkopf zeigt Ihnen an, nach welcher Spalte sortiert wird und ob die Werte auf- oder absteigend sortiert werden.
Halten Sie die Strg-Taste gedrückt und klicken Sie erneut auf den Spaltenkopf um die Sortierung aufzuheben. Die Liste wird nun wieder nach Ihrer in der Datei gespeicherten Reihenfolge angezeigt.

![Liste](/assets/images/liste1.png)

Um eine Liste nach zwei oder mehr Spalten zu sortieren, halten Sie bei aktiver Sortierung einer Spalte die Shift-Taste gedrückt und klicken Sie auf einen zweiten Spaltenkopf (z.B.: Nachname und dann Vorname)

!!! info "Hinweis"

    Das Anklicken des Spaltenkopfes führt zu einer Sortierung der angezeigten Liste für den angemeldeten Windows-Benutzer und wird nicht in der Datei gespeichert. Die Daten werden im Programm (z.B.: im Auswahldialog) weiterhin in der ursprünglichen Reihenfolge angezeigt. Mit Hilfe des Befehls `Start > Sortieren` erreichen Sie eine Sortierung, die in der Datei gespeichert und auch anderen Benutzern bzw. in anderen Modulen angezeigt wird.

## Mehrere Einträge in einer Liste auswählen

Um mehrere einzelne Zeilen zu markieren halten Sie bitte die ``Strg-Taste`` gedrückt und wählen Sie mit der linken Maustaste die gewünschten Zeilen aus. Um mehrere aufeinanderfolgende Zeilen zu markieren wählen Sie die erste Zeile mit einem Linksklick aus und halten die ``Shift-Taste`` gedrückt. Nun wählen Sie die letzte Zeile mit einem Linksklick aus.

## Nach einer Spalte Gruppieren

Sie können die Inhalte der Tabelle nach einer bestimmten Spalte gruppieren um Teilsummen oder eine bessere Übersicht zu erhalten.

Öffnen Sie dazu zuerst den Gruppierungsbereich oben in der Tagelle, indem Sie im Ribbon oben auf `Gruppieren` klicken. Klicken Sie dann mit der Maus auf den Spaltentitel, den Sie gruppieren wollen, halten sie die Maustaste gedrückt und ziehen die den Titel auf den Gruppierungsbereich und lassen Sie die Maustaste los. Die Gruppierung können Sie mit den Befehlen `Alle expandieren` und `Alle schließen` jeweils aufklappen bzw. wieder zuklappen.

Mit der Schaltfläche „In Ablage kopieren“ können Sie ausgewählte Zeilen in die Zwischenablage
übertragen.

![Gruppieren](/assets/images/gruppieren.png)

## Nach ganzen Zellinhalten filtern

Wenn Sie nach den ganzen Zellinhalten einer Spalte filtern, dann werden Ihnen alle Listeneinträge gezeigt, die den ausgewählten Zellinhalten entsprechen. Dabei stehen Ihnen alle Zellinhalte einer Spalte als möglicher Filter zur Verfügung. Klicken Sie mit der linken Maustaste auf das Filtersymbol und setzen Sie im Aufklappmenü den Haken im Kontrollkästchen vor einem oder mehreren der gewünschten Zellinhalte. Über die Reißzweckenschaltfläche auf dem Spaltenkopf erreichen Sie ein Aufklappmenü, in dem Sie alle Einzelwerte der Spalte für einen Filter auswählen können.

![Liste filtern](/assets/images/ListeFiltern01.png)

## Neuen Eintrag anlegen

Um innerhalb einer Liste einen neuen Eintrag anzulegen, müssen Sie der Liste eine neue Zeile hinzufügen. Klicken Sie auf `Start > Neu` oder klicken Sie in die letzte Zeile und drücken die Nach-UntenTaste auf Ihrer Tastatur. Wenn Sie auf `Start > Neu` klicken wird automatisch die Schaltfläche ``Liste bearbeiten`` aktiviert.

![Neuen Eintrag anlegen](/assets/images/ListeBearbeitenNEU.png)

## Spalten ein- und ausblenden

![Spalten ein/- ausblenden](/assets/images/SpaltenAusblenden.png)

Jede Liste besitzt spezielle Spalten, die Sie vermutlich nicht alle benötigen. Damit Sie eine möglichst übersichtliche Darstellung Ihrer Daten erhalten, empfiehlt es sich, nur die Spalten anzeigen zu lassen, mit denen Sie auch arbeiten, und die überzähligen Spalten auszublenden.

Wählen Sie  `Start > Spalten ein-/ausblenden` um das Anpassen-Fenster zu öffnen. Hier sehen Sie die Spaltenköpfe aller bisher ausgeblendeten Spalten. Per ``Drag & Drop`` (``Linksklick`` auf den Spaltenkopf und Maustaste beim Ziehen gedrückt halten) können Sie nun Spalten in dieses Fenster schieben um diese auszublenden.

![geöffnetes Zusatzfenster "Anpassung"](/assets/images/SpaltenAusblenden01.png)

Die in das Zusatzfenster ``Anpassung`` verschobenen Spalten bleiben in der normalen Listendarstellung ausgeblendet. Informationen, die in einer ausgeblendeten Spalte enthalten sind, bleiben auch beim Ausblenden erhalten und werden nach dem Einblenden wieder sichtbar. Um die Spalten wieder einzublenden können Sie die Spaltenköpfe aus dem Anpassen-Fenster per ``Drag & Drop`` herausziehen und im Tabellenkopf ablegen.

!!! info "Hinweis"

    Alternativ zu dem Aufruf `Start > Spalten ein-/ausblenden` können Sie auch das ``*`` links oben an jeder Stammdatentabelle zum Ein- und Ausblenden der Spalten nutzen.

!!! info "Hinweis"

    Zwei kleine grüne Pfeile oberhalb und unterhalb des Spaltenkopfs zeigen jeweils an, wo die Spalte eingefügt werden kann. Lassen Sie die linke Maustaste los, sobald die grünen Pfeile an Ihrer Wunschposition erscheinen.

## Spalten verschieben

Sie können die Reihenfolge der Spalten verändern, indem Sie einzelne Spalten mittels ``Drag&Drop`` an eine neue Position verschieben. Klicken Sie dazu mit der linken Maustaste auf den Spaltenkopf und halten Sie die Maustaste beim Ziehen gedrückt. Die grünen Pfeile markieren für Sie die Position, an der Sie die Spalte einfügen, wenn Sie die Maustaste los lassen.

![grünen Pfeile zum Verschieben von Spalten](/assets/images/SpaltenAusblendenGrünePfeile.png)

## Zeilen verschieben

Sie können die Reihenfolge der Zeilen ändern. Um eine Zeile nach oben oder unten zu verschieben, markieren Sie diese mit einem Linksklick und wählen `Start > Hoch bewegen` oder `Start > Ab bewegen`.
