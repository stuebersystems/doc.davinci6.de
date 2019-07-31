# Zeitvorgaben

Die Unterrichtsplanung mit DAVINCI 6 basiert auf verschiedenen Zeitvorgaben, die Sie zu Beginn der Planerstellung an Ihre spezifischen Gegebenheiten anpassen sollten.  

* **Planungszeitraum**: Die Eckdaten des Planungszeitraums umfassen zum einen die Kalenderdaten z.B. des ganzen oder halben Schuljahrs. Zum anderen aber auch die Wochentage, an denen Unterricht verplant werden soll.
* **Ferien und Feiertage**: Damit an den bundeslandspezifischen Ferien- und Feiertagen kein Unterricht verplant wird, müssen die Kalenderdaten dieser Ereignisse importiert werden.
* **Zeitrahmen/Stundenraster**: Damit der Unterricht später in ein verbindliches Stundenraster eingefügt werden kann, muss die Anzahl und Dauer der verfügbaren Planpositionen festgelegt werden.Die im Stundenraster definierten Planpositionen müssen mit konkreten Tageszeiten verknüpft werden, um die täglichen Unterrichts- und Pausenzeiten zu definieren.
* **Aufsichtszeiträume**: Um Aufsichtspläne zu erstellen, benötigen Sie ein eigenes Positions- und Zeitraster.
* **Unterrichtswochen**: Die Planung mit Perioden erfordert eine Festlegung darauf, welche Kalenderwochen des Planungszeitraums für den wochenbezogenen Unterricht zur Verfügung stehen In den folgenden Abschnitten werden Sie erfahren, wie Sie die entsprechenden Einstellungen vornehmen können.

## Ferien und Feiertage importieren

DAVINCI 6 unterstützt das iCalender-Format für den Austausch von Kalenderdaten. Kalenderdaten, die in diesem Format vorliegen, können Sie nach DAVINCI importieren. Um im Programmbereich „Kalender“ einen Kalender (z.B.: einen DAVINCI Ferienkalender) zu importieren, wählen Sie in der Kalenderansicht `Start > Importieren` und wählen den entsprechenden Kalender aus.

Die offiziellen Feier- und Ferientage Ihres Bundeslandes finden Sie hier:

| Betriebssystem | Pfad                                                                     |
| -------------- | ------------------------------------------------------------------------ |
| Windows 8 / 10 | `C:\Users\Public\Documents\Stueber Systems\daVinci 6\Beispiele\Kalender` |

## Planungszeitraum festlegen

Mit dem Planungszeitraum legen Sie fest, auf welchen übergeordneten Zeitraum sich die Angaben in Ihrer Plandatei beziehen, z.B. ein Schuljahr oder ein Semester.
Ein Planungszeitraum kann mehrere Plandateien umfassen. Sollten Sie über einen gewissen Planungszeitraum hinweg mit mehreren Plandateien arbeiten, so müssen Sie jeweils angeben auf welchen Teilzeitraum sich die einzelne Plandatei bezieht. Außerdem erhält jede Teildatei eine eigene Versionsnummer.

Im Dialogfenster `Eigenschaften > Zeitraum` können Sie die Zeitraumdaten Ihrer Plandatei bearbeiten. Rufen Sie dazu das Dialogfenster `Plan > Eigenschaften` auf und gehen Sie auf die Registerkarte `Zeitraum`.

![Eigenschaften > Zeitraum](/assets/images/Eigenschaften.Zeitraum.png)

| Ansichten                  | Bedeutung                                                                                                                                                |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Planungszeitraum           | Der Planungszeitraum beschreibt den Zeitraum indem sich die Stammdaten nicht grundlegend verändern (z.B.: ein Schuljahr)                                 |
| Hauptzeitraum dieser Datei | Die Planversion beschreibt einen Teilabschnitt des angegebenen Planungszeitraums.(z.B.: ein Halbjahr). Start- und Enddatum - die Gültigkeit der Planung. |
| Woche                      | Hier können Sie die Unterrichtstage der Woche festlegen.                                                                                                 |
| Standard-Zeitrahmen        | Mit der Schaltfläche `Standard-Zeitrahmen bearbeiten...` gelangen Sie direkt zum Hauptzeitrahmen und können ihn hier auch bearbeiten.                    |

!!! info "Hinweis"

    Wenn Sie im Laufe des Schuljahres verschiedene Planversionen einsetzen, so handelt es sich dabei um unterschiedliche Plandateien mit gleichem Planungszeitraum aber aufeinanderfolgenden Gültigkeitszeiträumen und Versionsnummern. Über das Modul DAVINCI ANALYTICS können Sie Ihren Gesamtjahresplan bestehend aus aufeinanderfolgenden Planversionen, statistisch auswerten. So können Sie mit diesem Modul z.B. die Summe der Unterrichtsstunden den Unterrichtsausfall und die Lehrer-Fehlstunden Datei übergreifend aber für einen Planungszeitraum berechnen. 

## Unterrichtswochen definieren

Wenn Sie mit wochenbezogenem Unterricht planen, so müssen Sie später im Programmbereich
`Stammdaten` für jede Periode angeben, in welchen Kalenderwochen kein Unterricht stattfindet. Die Ferienwochen werden dabei nicht automatisch ausgeklammert.

Damit Sie die Ferienwochen nicht beim Anlegen jeder Periode erneut als unterrichtsfrei definieren müssen, haben Sie Gelegenheit die Auswahl der Unterrichtswochen im Vorfeld für alle Perioden/Planungswochen zu begrenzen.
Um die Kennzeichnung der Kalenderwochen, in denen kein Unterricht stattfindet vorzunehmen, öffnen Sie die ``Plan Eigenschaften`` mit `Start > Eigenschaften > Statistik` und wählen Sie hier die ganzen unterrichtsfreien Wochen mit einem Haken an.

!!! info "Hinweis"

    In den ``Plan Eigenschaften`` unter `Start > Eigenschaften > Statistik` dürfen Sie nur ganze unterrichtsfreie Wochen mit einem Haken versehen. 

![Plan Eigenschaften, Register Statistik](/assets/images/PlanEigenschaften.Statistik.png)

## Summierung und Zeitdauer

In der Registerkarte "Statistik" des Dialogfensters `Eigenschaften` können Sie neben der Zeitdauerangabe auch die Verrechnungsart festlegen.

| Verrechnungsart | Beschreibung                                                                                                                                                                                                                                                                                                                                                         |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tagesbezogen    | Es wird jeden Tag die Anzahl der Stunden gezählt, wobei unterrichtsfreie Tage laut Kalender wie z.B. Ferien und Feiertage nicht mitgezählt werden. Das Resultat ist eine genaue Stundensumme über die Wochen und das Schuljahr, z.B. „2h je Woche in 20 Wochen des Schuljahres = 2h x 20 = 40h [im Schuljahr] => 40h / 40 Wochen = 1h/Woche [als Wochenmittelwert]“. |
| Wochenbezogen   | Es wird jeden Tag die Anzahl der Stunden gezählt, wobei die in „Wochenbezogene Summe“ ausgenommenen Wochen nicht mitgezählt werden. Das Resultat ist eine gemittelte Stundensumme über die Wochen des Schuljahres, z.B. „2h x 20 Wochen / 40 Wochen = 1h [je Woche als Mittelwert]“                                                                                  |
| Faktorbezogen   | Die jeweilige Stundendauer einer Veranstaltung wird mit dem Klassenfaktor (aus Klassensicht) bzw. dem Lehrerfaktor (bei Lehrersicht) multipliziert. Klassenfaktor und Lehrerfaktor können je Veranstaltung über das Dialogfenster „Veranstaltung“ manuell eingegeben werden oder errechnen sich automatisch aus dem Faktor der ggf. zugewiesenen Periode.            |

## Zeitrahmen definieren

Für die Verplanung Ihrer Unterrichtstermine steht Ihnen ein Stundenraster zur Verfügung. Dieses Stundenraster wird durch die Unterrichtsstunden gebildet, deren Anzahl und Dauer Sie im Zeitrahmen festlegen. Gemeinsam mit den Unterrichts- und Pausenzeiten geben diese Angaben den Zeitrahmen vor, der Ihnen für die Terminplanung in den Wochenstundenplänen zur Verfügung steht. 

Zwei Zeitrahmen sind von DAVINCI bereits vordefiniert:

* Hauptzeitrahmen und
* Aufsichten-Zeitrahmen

Sie können jeder Klasse und jedem Aufsichtsbereich in der Ansicht `Stammdaten` einen eigenen Zeitrahmen zuordnen. Wenn Sie z.B. bei Ihren Klassen zusätzlich zum 45-Minuten-Stundenraster auch Klassen mit 50-Minutenraster haben, brauchen Sie nur mit `Neu` einen weiteren Zeitrahmen mit 50-Minuten-Stunden hinzuzufügen. Wenn kein Zeitrahmen angegeben wurde, gilt stets der Hauptzeitrahmen.

![Zeitrahmen](/assets/images/Zeitrahmen.png)

Um z.B. den Hauptzeitrahmen zu ändern, klicken Sie auf ``Extras > Zeitrahmen``, markieren Sie im Zeitrahmen-Fenster den Eintrag ``Standard`` und klicken Sie auf ``Bearbeiten``.

## Haupteitrahmen

### Allgemein

![Zeitrahmen > Allgemein](/assets/images/Zeitrahmen.Allgemein.png)

In Register "Allgemein" können Sie allgemeine Angaben zu Ihrem Stundenraster eingeben.

| Eingabefeld                                                   | Bedeutung                                                                                                                                                                                                                                      |
| ------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tag besteht aus                                               | Maximale Anzahl der Unterrichtsstunden pro Tag                                                                                                                                                                                                 |
| Dauer einer Position                                          | die übliche Dauer einer Unterrichtsstunde in Minuten.                                                                                                                                                                                          |
| Einheiten je Position                                         | Mit der Eingabe in diesem Feld können Sie Ihre Standard Unterrichtsstunde in kleinere Minuten-Einheiten zerlegen. Wenn Sie hier z.B. 9 eingeben, dann werden die Positionen Ihres 45-Minuten Stundenrasters in 5-Minuten-Einheiten unterteilt. |
| Vormittag bis Position                                        | Bis zu welcher Position im Stundenraster ein Termin als Vormittagstermin gewertet werden?                                                                                                                                                      |
| Standardmäßig sichtbare Positionen                            | Wie viele Positionen sollen standardmäßig beim Öffnen eines Stundenplans im Planfenster angezeigt werden?                                                                                                                                      |
| Termin-Ende beim Verplanen automatisch an Zeitrahmen anpassen | Diese Funktion ermöglicht es Ihnen unterschiedlich lange Stunden zu verwenden (außerhalb der Vorgabe). Beim manuellen Setzen eines Termins wird die Termindauer automatisch auf die Zeilen Zeitspanne angepasst.                               |

### Angaben für die Automatik

Für die Verplanung der Stunden mit Hilfe der Automatik können Sie hier folgende Einstellungen treffen. Was die Automatik beachten soll, muss mit einem gesetzten Haken versehen sein:

* Doppelstunden Positionen beachten
* Termine dürfen nur passgenau in Stunde verplant werden
* Termine dürfen nicht über Pause verplant werden

### Register > Positionen

![Zeitrahmen > Positionen](/assets/images/Zeitrahmen.Positionen.png)

In Register "Positionen" geben Sie an, wann die Stundenpositionen beginnen/enden und wie die einzelnen Stundenpositionen benannt werden sollen (Eintrag in Spalte ``Bezeichnung``)

| Feld                              | Bedeutung                                                                                                                                                                                                                                                  |
| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Differenz                         | Gibt die Pausenzeiten an und wird von DAVINCI automatisch berechnet.                                                                                                                                                                                       |
| Trennlinie                        | Eine Farbangabe sorgt dafür, dass im Stundenplan an dieser Position eine Trennline in der entsprechenden Farbe erscheint. Sie können so z.B. den Nachmittag grafischen vom Vormittag trennen. Diese Farbe können Sie über die `entf`-Taste wieder löschen. |
| Doppelstunde                      | Markieren Sie insbedondere die Position, die als Anfangsposition einer Doppelstunde zulässig ist. Wenn sie z.B. die erste, dritte, fünfte usw. markieren, verhindert dies, dass eine Doppelstunde in der zweiten Stunde beginnt und in der dritten endet.  |
| Schaltfläche `Zeiten vorbesetzen` | Wenn Sie auf diese klicken, wird der Zeitrahmen ab dem zuletzt bearbeiteten Beginn oder Ende Pausenlos bis zur letzten Position automatisch vorbesetzt.                                                                                                    |

### Register > Zeilen-Trennlinien

![Zeitrahmen > Zeilen-Trennlinien](/assets/images/Zeitrahmen.Zeilen-Trennlinien.png)

In Register "Zeilen-Trennlinien" können Sie farbige Trennlinien zwischen Unterrichtseinheiten im Planraster bestimmen. Der Unterschied zu den Trennlinien unter ``Positionen`` besteht darin, dass Sie hier auch für Untereinheiten von Stunden Trennlinen angeben können, z.B. falls eine Unterrichtstunde zu 60 Minuten in vier Untereinheiten zu 15 Minuten aufgeteilt ist.

### Register > Positionsschemata

![Zeitrahmen > Positionsschemata](/assets/images/Zeitrahmen.Positionsschemata.png)

Unter "Positionsschemata" können Sie Startzeitpunkte für Termine mit vom Standard abweichender Dauer festlegen. Auf der Registerkarte Positionsschemata können Sie explizit angeben, auf welchen Startzeitpunkten Termine einer bestimmten Dauer je Tag verplant werden sollen. Diese Angaben sind nur dann relevant, wenn Angabe der Doppelstundenpositionen auf der Registerkarte "Positionen" nicht ausreichen sollten.

## Aufsichten-Zeitrahmem

Damit Sie für verschiedene Aufsichtsbereiche später eigene Aufsichtspläne erstellen können, müssen Sie mindestens einen Zeitrahmen erstellen, der speziell Anzahl und Dauer der Aufsichtspositionen sowie die zugehörigen Aufsichtszeiten festlegt.

Das Erstellen des Stunden- und Zeitrasters für die Aufsichtsplanung funktioniert genauso wie das Erstellen eines neuen Zeitrahmens für die Unterrichtsplanung.

![Aufsichten-Zeitrahmen](/assets/images/Aufischten-Zeitrahmen.png)

In Register "Allgemein" sind folgende Eingaben entscheidend:

| Eingabefeld                        | Bedeutung                                |
| ---------------------------------- | ---------------------------------------- |
| Tag besteht aus                    | Maximale Anzahl der Aufsichten pro Tag   |
| Dauer einer Position               | unrelevant                               |
| Einheiten je Position              | unrelevant                               |
| Vormittag bis Position             | unrelevant                               |
| Standardmäßig sichtbare Positionen | Anzahl gemäß "Tag besteht aus" eintragen |

!!! info "Hinweis"

    Sollten Sie auch Aufsichtslehrer für Ihre Buszeiten einteilen, die abweichend zu den Pausenzeiten sind, empfehlen wir Ihnen einen weiteren Zeitrahmen für die Buszeiten anzulegen.

Die speziellen Zeitrahmen für die Aufsichtsplanung müssen Sie Bereich [``Stammdaten > Aufsichtsbereiche``](/davinci-stundenplan/stammdaten/aufsichtsbereiche.md) den Bereichen zuweisen.

![Stammdaten Aufsichtsbereiche, Zuweisung Zeitrahmen](/assets/images/Stammdaten.Aufsichtsbereiche.png)
