# Mit der Automatik planen

Um die Automatik zu starten, klicken Sie bitte auf die obere Hälfte der Schaltfläche Automatik in der Menügruppe `Start > Automatik`.

![Im Dialogfenster `Automatik starten` stehen Ihnen unterschiedliche Optionen für den Automatikdurchlauf zur Verfügung](/assets/images/Automatik.png)

Die Automatik von DaVinci besteht aus einer Raum-, Setz- und Lehrerzuordnungsautomatik, die in den folgenden Abschnitten gesondert beschrieben werden. Bevor die Automatik gestartet wird, legen Sie Automatikvorgaben fest:

* Veranstaltungsbezogene Automatikvorgaben
* Allgemeine Automatikvorgaben
* Positionsschemata für Unterrichtstermine

Erst wenn Sie diese Vorgaben definiert haben, sollten Sie die Automatik starten.

* Automatik starten

## Veranstaltungsbezogene Automatikvorgaben

DaVinci bietet Ihnen die Möglichkeit für jede Veranstaltung individuelle Einstellungen zu treffen, die von der Automatik beim Setzen dieser Veranstaltungen berücksichtigt werden. Diese Einstellungen können Sie im Veranstaltungsfenster in der Ansicht `Zeitdetails` vornehmen. Die Automatikspezifischen Optionen, die Sie hier einstellen können, stehen Ihnen im Bereich `Automatikvorgaben der Veranstaltung zur Verfügung`.

![In der Ansicht `Zeitdetails` des Dialogfensters `Veranstaltung` können Sie veranstaltungsbezogene Vorgaben für den Automatikdurchlauf einstellen.](/assets/images/VeranstaltungDetailAutomatikvorgaben1.png)


| Automatikvorgaben der Veranstaltung | Bedeutung                                                                                                                                                                                                                                                                                                                                                                                                               |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tagesposition                       | In diesem Feld können Sie einstellen, ob eine Veranstaltung nur am Vormittag, nur am Nachmittag oder sowohl als auch stattfinden soll. Die Automatik benutzt dabei als Kriterium für Unterscheidung zwischen Vormittag und Nachmittag die Angebe im Feld ``Vormittag bis Position`` auf der Registerkarte ``Allgemein`` des zugehörigen [Zeitrahmens](/davinci-stundenplan/zeitvorgaben/zeitrahmen/hauptzeitrahmen.md). |
| Eckstunde                           | An dieser Stelle können Sie entscheiden, ob eine Veranstaltung bevorzugt nur am Anfang oder nur am Ende oder bevorzugt entweder am Anfang oder am Ende des Unterrichtstages verplant werden soll.                                                                                                                                                                                                                       |
| Fachfolge                           | Mit der Angabe im Feld `Fachfolge` können Sie festlegen, ob eine Veranstaltung direkt aufeinanderfolgende bzw. nicht direkt aufeinanderfolgend mit bestimmten anderen Veranstaltungen verplant werden sollen.                                                                                                                                                                                                           |
| Doppelstunde                        | Durch Eintrag z.B. einer "1" oder "2" können Sie der Automatik mitteilen, wie viele Doppelstunden verplant werden sollen.                                                                                                                                                                                                                                                                                               |
| Ignoriere Automatik                 | Mit dem Haken im Kontrollkästchen vor dieser Option legen Sie fest, dass die Termine dieser Veranstaltung von der Automatik nicht verplant werden.                                                                                                                                                                                                                                                                      |

!!! info "Hinweis"

    Veranstaltungen die durch die Automatik ignoriert werden sollen, erkennen Sie in der Veranstaltungsliste in Spalte "Unverplant" durch geklammerte unverplant Werte.

![Ignoriere Automatik](/assets/images/AusgenommenAusAutomatik.png)

**Zeitpräferenzen** 
Im Listenfenster unter Zeitpräferenzen können Sie Sperrungen und Kernzeiten für eine Veranstaltung erfassen, siehe Abschnitt [Zeitpräferenzen erfassen](/davinci-stundenplan/stundenplan-erstellen/zeitpraferenzen-erfassen.md).

## Automatikvorgaben

DaVinci bietet Ihnen die Möglichkeit allgemeinverbindliche Einstellungen für alle Veranstaltungen zu treffen, die von der Automatik berücksichtigt werden. Diese Einstellungen können Sie im Dialogfenster `Automatikvorgaben` in verschiedenen Registerkarten treffen. Außerdem haben Sie die Möglichkeit einige Vorgaben für Klassen, Lehrer und Fächer zu treffen. Dafür stehen Ihnen die Registerkarten `Klassenvorgaben`, `Lehrervorgaben` und `Fächervorgaben` zur Verfügung.

Das Dialogfenster `Automatikvorgaben` können Sie aufrufen, indem Sie in der Menügruppe `Start > Automatik` auf die untere Hälfte der Schaltfläche Automatik klicken und den Eintrag `Automatikvorgaben` aus dem Aufklappmenü wählen.

![Aufruf "Automatikvorgaben"](/assets/images/Automatik.Vorgaben.png)

### Allgemeine Automatikvorgaben - Register "Allgemein"

Auf der Registerkarte "Allgemein" können Sie für alle Veranstaltungen allgemeinverbindliche Einstellungen treffen.

![Automatikvorgaben "Allgemein"](/assets/images/Automatikvorgaben.Allgemein.png)

Auf der Registerkarte „Allgemein“ des Dialogfensters ``Automatikvorgaben`` können Sie verschiedene Ziele auf einer 10-stufigen Skala von 0-9 gewichten. (0=NICHT beachten...9=unbedingt beachten)

#### Hauptvorgaben

| Vorgabe                                  | Bedeutung                                                                                                                                                                   |
| ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Klassenspringstunden beachten            | Die Klassenspringstundenangaben auf der dahinterliegenenden Registerkarte `Klassenvorgaben` des Dialogfensters `Automatikvorgaben` müssen nach Möglichkeit beachtet werden. |
| Lehrerspringstunden beachten             | Die Lehrerspringstundenangaben auf der dahinterliegenenden Registerkarte `Lehrervorgaben` des Dialogfensters `Automatikvorgaben` müssen nach Möglichkeit beachtet werden.   |
| Springstundenzählung bis                 | Geben Sie hier die Uhrzeit an, bis zu der Lehrerspringstunden gezählt werden sollen.                                                                                        |
| Vormittag bis                            | Geben Sie hier die Uhrzeit an, die als Übergang zwischen Vormittag und Nachmittag gewertet werden soll                                                                      |
| Termine nicht mehrfach am Tag            | Die Automatik versucht Fächer am gleichen Tag zu vermeiden, z.B. Mathematik nicht Montag 1. Stunde und Montag 3. Stunde.                                                    |
| Fächer in gleicher Stunde vermeiden      | Die Automatik versucht Fächer in gleicher Stunde zu vermeiden, z.B. Mathematik nicht Montag und Dienstag und Mittwoch in erster Stunde.                                     |
| Mehrstündige Termine nicht am Nachmittag | Mehrstündige Termine sollen nicht am Nachmittag verplant werden                                                                                                             |
| Doppelstunden beibehalten                | Doppelstunden sollen nach Möglichkeit beibehalten werden                                                                                                                    |
| Mehrstündige Termine nicht in Tagesfolge | Mehrstündige Termine eines Fachs dürfen nicht an unmittelbar aufeinander folgenden Tagen verplant werden.                                                                   |

#### Weitere Vorgaben

| Vorgabe                                      | Bedeutung                                                                     |
| -------------------------------------------- | ----------------------------------------------------------------------------- |
| 1-stündige Termine nicht samstags            | 1stündige Fächer dürfen nicht samstags verplant werden.                       |
| 2-stündige Termine nicht samstags            | 2stündige Termine dürfen nicht samstags verplant werden.                      |
| 2-3-stündige Fächer nicht Samstag auf Montag | 2- und 3-stündige Fächer dürfen nicht von Samstag auf Montag verplant werden. |
| 1-stündige Fächer nicht in 6. Stunde         | 1-stündige Fächer dürfen nicht in der 6. Stunde verplant werden.              |

#### Teilzeitklassen

| Vorgabe                                     | Bedeutung                                                                                                                                                                                                                                   |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Bei Teilzeitklassen Termine mehrfach am Tag | Bei Teilzeitklassen können Ausnahmen eingeräumt werden für mehrere Termine eines Fachs an einem Tag erlauben.                                                                                                                               |
| Wochentage je Teilzeitklasse maximal        | Anhand der hier eingegebenen Zahl werden Teilzeitklassen erkannt. Teilzeitklassen sind Klassen, die nur an bestimmten Tagen der Woche unterrichtet werden. Für diese Klassen gilt die Option `Bei Teilzeitklassen Termine mehrfach am Tag`. |

## Klassenbezogene Automatikvorgaben - Register "Klassenvorgaben"

Auf der Registerkarte "Klassenvorgaben" können Sie klassenbezogene Einstellungen treffen.

Hier können Sie die maximale Anzahl der Unterrichtstage einer Klasse pro Woche sowie die maximale Anzahl der Unterrichtsstunden pro Tag festlegen.

![Auf der Registerkarte ``Klassenvorgaben`` des Dialogfensters ``Automatikvorgaben`` legen Sie klassenbezogene Einstellungen für den Automatikdurchlauf fest.](/assets/images/Klassenvorgaben.png)

## Lehrerbezogene Automatikvorgaben - Register "Lehrervorgaben"

Auf der Registerkarte "Lehrervorgaben" können Sie lehrerbezogene Einstellungen treffen.

Hier können Sie die maximale Anzahl der Unterrichtstage einer Klasse pro Woche sowie die maximale Anzahl der Unterrichtsstunden pro Tag festlegen. Außerdem geben Sie hier an, wie viele Springstunden ein Lehrer maximal erhalten soll.

![Auf der Registerkarte ``Lehrervorgaben`` des Dialogfensters ``Automatikvorgaben`` legen Sie lehrerbezogene Einstellungen für den Automatikdurchlauf fest.](/assets/images/Lehrervorgaben.png)

## Fächerbezogene Automatikvorgaben - Register "Fächervorgaben"

Auf der Registerkarte "Fächervorgaben" können Sie fachbezogene Einstellungen klassenübergreifend treffen.

Mit der Fachfolge legen Sie fest, welche Fächer direkt aufeinanderfolgend bzw. nicht direkt aufeinanderfolgend verplant werden sollen.

![Fächervorgaben](/assets/images/Fächervorgaben.png)

| Fachfolge   | Bedeutung für die Automatik                                                             |
| ----------- | --------------------------------------------------------------------------------------- |
| 0           | keine Bedeutung                                                                         |
| 1 bis 9     | Fächer mit gleicher Zahl müssen am Tag unmittelbar hintereinander verplant werden       |
| -9 bis -1   | Fächer mit gleicher Zahl dürfen am Tag nicht unmittelbar hintereinander verplant werden |
| -19 bis -10 | Fächer mit gleicher Zahl dürfen nicht am gleichen Tag verplant werden                   |

## Vorgaben bei der Zuweisung von Lehrern und Räumen - Registerkarte „Optionen“

Für die Verplanung Ihrer Unterrichtstermine können Sie im Dialogfenster `Automatikvorgaben` auf der Registerkarte „Optionen“ festlegen, wie sich die DaVinci Automatik bei der Zuweisung von Lehrern und Räumen verhalten soll.

![Register "Optionen"](/assets/images/Automatikoptionen.png)

| Option       | Beschreibung      |
| ------------------------------------------------- | - |
| Keine Angebe in Spalte "Raum" ohne Raum verplanen | Es wird nur denjenigen Terminen ein Raum neu zugewiesen, bei deren Veranstaltung in der Spalte „Raum“ ein Vorgaberaum eingegeben wurde bzw. wenn dort eine Angabe gemacht wurde |
| Termine nur verplanen, wenn Lehrer verfügbar ist  | Der Termin wird nur dann zeitlich verplant, wenn dann auch ein der Lehrer verfügbar ist, d.h. keinen Unterricht und keine absolute Sperrung zu diesem Zeitpunkt hat             |
| Termine nur verplanen, wenn Raum verfügbar ist    | Der Termin wird nur dann zeitlich verplant, wenn dann auch ein Raum verfügbar ist, d.h. dieser keinen Unterricht und keine absolute Sperrung zu diesem Zeitpunkt hat            |

* Wie soll die Raumautomatik die Räume der Termine behandeln?

| Auswahl  | Beschreibung |
| --------------------------- | ----------------------- |
| Neu zuweisen oder verändern   | Die Automatik weist Terminen neue Räume zu bzw. verändert Räume  |
| Neu zuweisen, aber bereits zugewiesene nicht verändern | Die Automatik weist bei Terminen nur dann Räume zu, wenn noch kein Raum zugewiesen wurde. Bestehende Raumzuweisungen werden nicht verändert. |
| Keine neu zuweisen                                     | Die Automatik weist Terminen keine neue Räume zu bzw. verändert keine Räume                                                                  |
| Keine zuweisen und zugewiesene entfernen               | Die Automatik weist Terminen keine neue Räume zu und entfernt bereits zugewiesene Räume## Positionsschemata für Unterrichtstermine anlegen   |

Das Dialogfenster [`Zeitrahmen`](/davinci-stundenplan/zeitvorgaben/zeitrahmen/hauptzeitrahmen.md), in dem Sie die Stunden- und Zeitraster für die Unterrichtsplanung erstellen, bietet die Möglichkeit Positionen festzulegen, an die die Automatik den Beginn einer Doppelstunde platzieren darf. Diese Einstellung können Sie auf der Registerkarte "Positionen“ in der Spalte „Doppelstunde“ vornehmen. 

![``Extras > Zeitrahmen``](/assets/images/Zeitrahmen.Doppelstunde.png)

Positionen, die an dieser Stelle nicht mit einem Haken versehen sind, werden von der Automatik nicht für den Beginn von Doppelstunden genutzt. Darüber hinaus können Sie im Dialogfenster für Termine, deren Dauer sich jenseits des Schemas Einzelstunde/ Doppelstunde bewegt, spezifische Zeitkorridore hinterlegen. Die Setz-Automatik darf Termine einer bestimmten Dauer in der Folge nur an diese explizit definierten Stellen im Planraster setzen. Um für Termine unterschiedlicher Dauer fixe Zeitkorridore für die Setzautomatik festzulegen, gehen Sie bitte folgendermaßen vor:

1. Öffnen Sie DaVinci 6 und blättern Sie zum Menüregister `Extras`.
2. Klicken Sie in der Menügruppe `Extras > Verwalten` auf die Schaltfläche `Zeitrahmen`.
3. Markieren Sie im erscheinenden Dialogfenster `Zeitrahmen` den gewünschten Zeitrahmen
4. Blättern Sie im Dialogfenster `Zeitrahmen` zur Registerkarte "Positionsschemata".
5. Klicken Sie auf die Schaltfläche `Neue Zeile`.
6. Geben Sie im erscheinenden Dialogfenster im Feld `Termindauer` die Dauer der Termine in Minuten an, für die Sie einen bzw. mehrere fixe Zeitkorridore definieren wollen.
7. Tragen Sie im darunterliegenden Eingabefeld die Startzeiten der Unterrichtspositionen ein, die für die vorgegebene Termindauer in Frage kommen.
8. Bestätigten Sie die hinterlegten Startzeiten mit `OK`
9. Legen Sie ggf. weitere Positionsschemata für andere Termindauern an.
10. Bestätigen Sie Ihre Änderungen am Unterrichtszeitrahmen abschließend mit `OK`.

Die Automatik setzt in der Folge Ihre unverplanten Termine gemäß Ihrer Vorgaben zu den zulässigen Zeitkorridoren.

## Automatik starten

Die Automatik können Sie wie folgt starten:

* `Start > Automatik`- oberer Bereich der Schaltfläche `blaues Dreieck`
  ODER
* `Start > Automatik`- Aufklappmenü `Automatik starten`
  ODER
* Tastenkombination `Ctrl+Y`

![Automatik Starten](/assets/images/Automatik.Starten.png)

## Setzstrategien

Sie können die Automatik mit verschiedenen Filterangaben starten, um z.B. zuerst die Oberstufe setzen zu lassen (Gymnasium) oder um zuerst bestimmte Fachräume verplanen zu lassen. Sie können die Automatik so mehrfach starten. Automatisches und manuelles Setzen können sich auch ergänzen. Sie können z.B. bestimmte Stunden manuell im Planfenster setzen und dann erst die Automatik starten.

Welche Vorgehensweise und welche Vorgaben zum besten Ergebnis führen, hängt von Ihren Plandaten und Ihren Engpässen ab. Legen Sie eine Kopie Ihrer Plandatei an und starten Sie die Automatik mit anderen Vorgaben. So können Sie den Effekt verschiedener Vorgaben vergleichen und dann mit der Datei weiterarbeiten, die Ihren Vorstellungen am nächsten kommt.

Die Automatik verplant die ungesetzten Unterrichtstermine entsprechend Ihrer Vorgaben. Bereits gesetzte Unterrichtstermine können dabei von der Automatik umgeplant werden, wenn dadurch eine insgesamt bessere Umsetzung der verschiedenen Vorgaben erreicht wird.

!!! info "Hinweis"

    Um zu verhindern, dass bereits gesetzte Stunden von der Setzautomatik noch einmal geändert werden, besteht die Möglichkeit diese Termine im Plan zu fixieren.

Um die Setzautomatik zu starten, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie das `Automatik starten`-Fenster auf und markieren Sie die Option `Setzautomatik`
2. Aktivieren Sie im Bereich `Auswahl` die gewünschte Option für die Auswahl der Termine, die von der Setzautomatik verplant werden sollen.
3. Klicken Sie auf die Schaltfläche `Starten`

Die Automatik verplant daraufhin die Termine entsprechend der von Ihnen vorgenommenen Einstellungen.

Folgende Optionen stehen Ihnen zur Verfügung:

|Auswahl | Bedeutung|
|---|---|
|Alle| Mit dieser Option werden alle Termine von der Setzautomatik verplant.|
|Klassen/Jahrgänge| Bei dieser Einstellung werden nur Termine verplant, denen eine Klasse als Termin-Teilnehmer zugewiesen ist.|
|Lehrer| Mit dieser Variante werden nur die Termine verplant, denen ein Lehrer als Termin-Teilnehmer zugewiesen ist.|
|Räume| Bei dieser Einstellung werden nur Termine verplant, denen ein Raum als Termin-Teilnehmer zugewiesen ist.|
|Fächer| Mit dieser Option werden nur Termine verplant, denen ein Unterrichtsfach zugewiesen ist.|
|Blöcke| Mit dieser Variante werden nur die Termine verplant, bei denen ein Blockkürzel hinterlegt ist.|

Tragen Sie im Feld "Filter" eine Angabe ein, um die Auswahl der zu verplanenden Termine weiter einzuschränken. Für die Eingabe von Filterwerten gelten folgende Konventionen.

|Filter | Bedeutung|
|---|---|
|Filter mit Stammdaten-Kürzel|Sie können die zu verplanenden Termine durch die Eingabe eines bestimmten Stammdaten- bzw. Blockkürzels auf Termine einschränken, denen dieses Kürzel in der Veranstaltungsliste zugewiesen ist. Eine Filterung der zu verplanenden Termine ist mit den Kürzeln der Klassen, Lehrer, Räume, Fächer und Blöcke möglich. Aktivieren Sie dazu wie unter Schritt 2. beschrieben die entsprechende Option im Bereich `Auswahl` und tragen Sie anschließend das gewünschte Stammdaten- bzw. Blockkürzel in das Feld `Filter` ein.|
|Filter mit Platzhaltern| Sie können die zu verplanenden Termine durch die Eingabe nur eines bestimmten Teils eines Stammdaten- bzw. Blockkürzels auf Termine einschränken, denen dieses Teilkürzel in der Veranstaltungsliste zugewiesen ist. Eine Filterung der zu verplanenden Termine ist hier wiederum mit den Kürzeln der Klassen, Lehrer, Räume, Fächer und Blöcke möglich. Aktivieren Sie dazu wie unter Schritt 2. beschrieben die entsprechende Option im Bereich „Auswahl“ und tragen Sie anschließend das gewünschte Teilkürzel Feld „Filter“ ein. Damit das eingetragene Teilkürzel beim Automatikdurchlauf berücksichtigt wird, muss das Teilkürzel um den Platzhalter `*` oder `?` ergänzt werden. Der Platzhalter `*` repräsentiert eine beliebige Zeichenfolge, der Platzhalter `?` hingegen ein beliebiges Einzelzeichen.|

Die Automatik richtet sich dabei neben den Einstellungen, die Sie auf der Registerkarte ``Automatik starten`` vornehmen, nach folgenden Vorgaben:

1. den Einstellungen auf der Registerkarte `Allgemein` des Dialogfensters `Automatikvorgaben`
2. den Angaben für Klassen, Lehrer und Fächer auf den Registerkarten `Klassenvorgaben`, `Lehrervorgaben` und `Fächervorgaben` des Dialogfensters `Automatikvorgaben`
3. den Automatikoptionen für die Verplanung der Termine ohne/ mit Lehrer bzw. ohne/ mit Raum die Sie Sie auf der Registerkarte `Optionen` des Dialogfensters `Automatikvorgaben` einstellen können.
4. den Angaben unter Automatikvorgaben in der Ansicht `Zeitdetails` des Dialogfensters `Veranstaltung`.
5. den angegebenen Doppelstundenpositionen auf der Registerkarte `Positionen` der eingesetzten Zeitrahmen.
6. den eingegebenen Zeitkorridoren für unterschiedliche Termindauern auf der Registerkarte `Positionsschemata` der eingesetzten Zeitrahmen.
7. den eingetragenen Zeitpräferenzen in den Plänen
8. der angegebenen Position für den Vormittag auf der Registerkarte "Allgemein" der eingesetzten Zeitrahmen.

![Zeitrahmen](/assets/images/Zeitrahmen.Positionsschemata01.png)

## Setzautomatik

Die Automatik verplant die ungesetzten Unterrichtstermine entsprechend Ihrer Vorgaben. Bereits gesetzte Unterrichtstermine können dabei von der Automatik umgeplant werden, wenn dadurch eine insgesamt bessere Umsetzung der verschiedenen Vorgaben erreicht wird.

!!! info "Hinweis"

    Um zu verhindern, dass bereits gesetzte Stunden von der Setzautomatik noch einmal geändert werden, besteht die Möglichkeit diese Termine im Plan zu fixieren. Wie Sie einen gesetzten Termin im Plan fixieren können, erfahren Sie hier.

Um die Setzautomatik zu starten, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie das `Automatik starten`-Fenster auf und markieren Sie die Option ``Setzautomatik``
2. Aktivieren Sie im Bereich `Auswahl` die gewünschte Option für die Auswahl der Termine, die von der Setzautomatik verplant werden sollen.
3. Klicken Sie auf die Schaltfläche `Starten`

Die Automatik verplant daraufhin die Termine entsprechend der von Ihnen vorgenommenen Einstellungen.

Folgende Optionen stehen Ihnen zur Verfügung:

|Auswahl | Bedeutung|
|---|----|
|Alle| Mit dieser Option werden alle Termine von der Setzautomatik verplant.|
|Klassen/Jahrgänge| Bei dieser Einstellung werden nur Termine verplant, denen eine Klasse als Termin-Teilnehmer zugewiesen ist.|
|Lehrer| Mit dieser Variante werden nur die Termine verplant, denen ein Lehrer als Termin-Teilnehmer zugewiesen ist.|
|Räume| Bei dieser Einstellung werden nur Termine verplant, denen ein Raum als Termin-Teilnehmer zugewiesen ist.|
|Fächer| Mit dieser Option werden nur Termine verplant, denen ein Unterrichtsfach zugewiesen ist.|
|Blöcke| Mit dieser Variante werden nur die Termine verplant, bei denen ein Blockkürzel hinterlegt ist.

Tragen Sie im Feld `Filter` eine Angabe ein, um die Auswahl der zu verplanenden Termine weiter einzuschränken. Für die Eingabe von Filterwerten gelten folgende Konventionen.

|Filter | Bedeutung|
|---|---|
|Filter mit Stammdaten-Kürzel| Sie können die zu verplanenden Termine durch die Eingabe eines bestimmten Stammdaten- bzw. Blockkürzels auf Termine einschränken, denen dieses Kürzel in der Veranstaltungsliste zugewiesen ist. Eine Filterung der zu verplanenden Termine ist mit den Kürzeln der Klassen, Lehrer, Räume, Fächer und Blöcke möglich. Aktivieren Sie dazu wie unter Schritt 2. beschrieben die entsprechende Option im Bereich `Auswahl` und tragen Sie anschließend das gewünschte Stammdaten- bzw. Blockkürzel in das Feld `Filter` ein.|
|Filter mit Platzhaltern| Sie können die zu verplanenden Termine durch die Eingabe nur eines bestimmten Teils eines Stammdaten- bzw. Blockkürzels auf Termine einschränken, denen dieses Teilkürzel in der Veranstaltungsliste zugewiesen ist. Eine Filterung der zu verplanenden Termine ist hier wiederum mit den Kürzeln der Klassen, Lehrer, Räume, Fächer und Blöcke möglich. Aktivieren Sie dazu wie unter Schritt 2. beschrieben die entsprechende Option im Bereich „Auswahl“ und tragen Sie anschließend das gewünschte Teilkürzel Feld „Filter“ ein. Damit das eingetragene Teilkürzel beim Automatikdurchlauf berücksichtigt wird, muss das Teilkürzel um den Platzhalter `*` oder `?` ergänzt werden. Der Platzhalter `*` repräsentiert eine beliebige Zeichenfolge, der Platzhalter `?` hingegen ein beliebiges Einzelzeichen.|

Die Automatik richtet sich dabei neben den Einstellungen, die Sie auf der Registerkarte ``Automatik starten`` vornehmen, nach folgenden Vorgaben:

1. den Einstellungen auf der Registerkarte `Allgemein` des Dialogfensters `Automatikvorgaben`
2. den Angaben für Klassen, Lehrer und Fächer auf den Registerkarten `Klassenvorgaben`, `Lehrervorgaben` und `Fächervorgaben` des Dialogfensters ``Automatikvorgaben``
3. den Automatikoptionen für die Verplanung der Termine ohne/ mit Lehrer bzw. ohne/ mit Raum die Sie Sie auf der Registerkarte `Optionen` des Dialogfensters `Automatikvorgaben` einstellen können.
4. den Angaben unter Automatikvorgaben in der Ansicht `Zeitdetails` des Dialogfensters `Veranstaltung`.
5. den angegebenen Doppelstundenpositionen auf der Registerkarte `Positionen` der eingesetzten Zeitrahmen.
6. den eingegebenen Zeitkorridoren für unterschiedliche Termindauern auf der Registerkarte `Positionsschemata` der eingesetzten Zeitrahmen.
7. den eingetragenen Zeitpräferenzen in den Plänen
8. der angegebenen Position für den Vormittag auf der Registerkarte `Allgemein` der eingesetzten Zeitrahmen.

## Raumautomatik

Rufen Sie das `Automatik starten`-Fenster auf, markieren Sie die Option `Raumautomatik` und klicken Sie auf `Start`. 

![Raumautomatik starten](/assets/images/RaumautomatikStarten.png)

Die Automatik verplant daraufhin die Räume. Sie können die Raumautomatik auch zusammen mit der Setzautomatik starten, indem Sie die beiden entsprechenden Optionen markieren. Jedoch kann die Raumautomatik nur alleine gestartet werden, wenn vorher die Setzautomatik gelaufen ist oder die Veranstaltungen bereits manuell ohne Räume gesetzt wurden.

Die Raumautomatik versucht, den Raum für einen Termin gemäß folgender Reihenfolge zu bestimmen:

1. Standardvorgaberaum (Spalte „Raum“ der Veranstaltungsliste) versuchen
2. Andere Räume der Raumvorgabeliste (Spalte „Räume“ der Veranstaltungsliste) versuchen
3. Fachräume (Spalte „Räume“ auf der Registerkarte „Fächer“ im Stammdatenfenster) versuchen
4. Klassenraum (Spalte „Raum“ auf der Registerkarte „Klassen“ im Stammdatenfenster) versuchen
5. Anderer freier Raum, der gemäß Kapazität und Teamzugehörigkeit für eine Veranstaltung in Frage kommt.

Darüber hinaus haben Sie die Möglichkeit die Zuordnung von Räumen zu Veranstaltungen auf Räume einer bestimmten Raumart zu beschränken. 

Dabei werden folgende Eingaben vorausgesetzte:

1. Weisen Sie im Stammdatenfenster "Räume" den gewünschten Räumen eine Raumart in Spalte "Raumart" zu.
2. Hinterlegen Sie in der Spalte „Raumart“ der Veranstaltungsliste einen bestimmten Eintrag, um festzulegen, dass bei den entsprechenden Veranstaltungen nur Räume zugewiesen werden dürfen, bei denen in der Stammdaten-Liste der gleiche Eintrag in der Spalte „Raumart“ eingetragen wurde.

!!! info "Hinweis"

    Raumarten definieren Sie über das Schlüsselverzeichnis "Raumarten" unter `Extras > Schlüsselverzeichnisse`.

![Raumarten](/assets/images/Raumarten.png)

## Lehrerautomatik

Die Lehrerzuordnungsautomatik weist verplanten Terminen ohne Lehrerzuordnung einen passenden Lehrer zu. Damit die Automatik einen Lehrer zuweist, müssen folgende Voraussetzungen erfüllt sein:

* Das Unterrichtsfach der Veranstaltung muss bei dem Lehrer in der Spalte „Fächer“ der Stammdaten-Liste „Lehrer“ hinterlegt sein.
* Das Team, dem die unterrichte Klasse zugewiesen ist, muss bei dem Lehrer in der Spalte „Team“ der Stammdaten-Liste eingetragen sein. Ist einer Klasse in den Stammdaten kein Team zugewiesen, spielt die Teamzugehörigkeit eines Lehrers für die Zuordnung keine Rolle.
* Der Lehrer muss auf der Basis der bisherigen Planung noch über ausreichend Differenzstunden zu seiner vorgebenen Sollstundenzahl verfügen.

Es werden von der Automatik also nur Fachlehrer zugewiesen, deren Teamzugehörigkeit mit der unterrichteten Klasse übereinstimmt und die außerdem über ein hinreichendes Reststundenkontingent verfügen.

Um die Lehrerzuordnungsautomatik zu starten, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie das `Automatik starten`-Fenster auf.
2. Markieren Sie im Bereich `Automatik` die Option `Lehrerzuordungsautomatik`.
3. Klicken Sie auf die Schaltfläche `Starten`.

Die Automatik weist daraufhin den verplanten Terminen ohne Lehrerzuordnung passende Lehrer zu.

Sie können die Lehrerzuordnungsautomatik auch zusammen mit der Setz- und der Raumautomatik starten, indem Sie die beiden entsprechenden Optionen markieren. Jedoch kann die Lehrerautomatik nur alleine gestartet werden, wenn vorher die Setzautomatik gelaufen ist oder die Veranstaltungen bereits manuell ohne Lehrer gesetzt wurden.

## Sperrungsautomatik

## Ergebnisse des Automatikdurchlaufs kontrollieren

Die Ergebnisse des Automatikdurchlaufs können Sie im Dialogfenster `Automatik` überprüfen. In diesem Fenster werden alle Veränderungen angezeigt, die von der Automatik geplant werden.

Im Dialogfenster `Automatik` werden verschiedene Arten von Änderungen angezeigt:

|Art | Bedeutung|
|---|---|
|Neu verplant| Ein unverplanter Termin wird an eine bestimmte Position in den Plan gesetzt bzw. ein bereits verplanter Termin an eine andere Position verschoben. Der Zusatz „Geteilt“ in der zweiten Spalte des „Automatik“-Fensters weist darauf hin, dass eine Doppelstunde für die Verplanung durch die Automatik in zwei Einzelstunden zerlegt wurde|
|Raumzuweisung| Ein Termin erhält einen neuen bzw. anderen Raum als den in der Veranstaltungsliste zugewiesenen Erstraum.|
|Raum offen | Ein Termin wurde ohne Raum verplant.|
|Lehrerzuweisung| Ein Termin ohne Lehrerzuordnung erhält einen passenden Lehrer|

Das Dialogfenster `Automatik` können Sie neben das Planungsfenster platzieren und gleichzeitig im Planungsfenster die geplanten Termine ansehen und bearbeiten. Um sich den Klassenplan einer bestimmten Änderung anzusehen, markieren Sie die die zugehörige Änderungszeile im Dialogfenster `Automatik` und klicken Sie anschließend auf die Schaltfläche `Klassenplan` unten links im `Automatik`-Fenster. Den zugehörigen Lehrerplan können Sie über die Schaltfläche Lehrerplan rechts daneben öffnen. Mit den Pfeilschaltflächen rechts neben der Schaltfläche `Lehrerplan` können Sie zum Klassen- bzw. Lehrerplan der nächsten bzw. der vorherigen Änderungszeile blättern.

![Ergebnis](/assets/images/Automatik.Durchlaf.png)

Um die Änderungen des aktuellen Automatikdurchlaufs zu übernehmen, müssen Sie diese mit `OK` bestätigen. Wenn Sie hingegen das Ergebnis des Automatikdurchlaufs insgesamt verwerfen möchten, so klicken Sie bitte auf die Schaltfläche `Zurücksetzen`. Anschließend können Sie die Automatik mit neuen Einstellungen starten.

## Stundenplan prüfen

Im Anschluss an den Automatikdurchlauf bietet es sich an, zu prüfen, wie die vorgenommene Planung sich zu den Vorgaben, die auf der Registerkarte „Allgemein“ des Dialogfensters ``Automatikvorgaben`` getroffen werden können, verhält. Dazu steht Ihnen das Dialogfenster ``Stundenplan prüfen`` zur Verfügung, dass Sie über den Befehl ``Stundenplan prüfen`` im Aufklappmenü der Schaltfläche ``Automatik`` aufrufen können. 

![Aufruf ``Automatik prüfen``](/assets/images/Automatik.Prüfen.png)

In diesem Dialogfenster werden „Verstöße“ gegen die allgemeinen Automatik-vorgaben aufgelistet, sofern diese im Dialogfenster „Automatikvorgeben auf der Registerkarte „Allgemein“ nicht mit dem Wert „0“ bewertet wurden.

!!! info "Hinweis"

    Zur Erinnerung: Die Bewertung „0“ auf der 10-stufigen Skala von „0“ bis „9“ bedeutet, dass ein bestimmtes Ziel für die Planung keine Rolle spielt.

Dabei werden folgende Vorgaben ausgewertet:

**Lehrer** Unter dieser Rubrik werden alle Lehrer aufgelistet, deren Lehrerplan in mindestens einer Unterrichtswoche des Planungszeitraums mehr Springstunden aufweist, als im Dialogfenster „Automa-tikvorgaben“ auf der Registerkarte „Lehrervorgaben“ in der Spalte „Max. Springstunden je Woche“ angegeben sind. Voraussetzung dafür, dass diese Kategorie ausgewertet wird, ist, dass die Vorgabe „Lehrerspringstunden beachten“ in den allgemeinen Automatikvorgaben mindestens mit dem Wert „1“ gewichtet wurde.
**Klassen** Unter dieser Rubrik werden alle Klassen aufgelistet, deren Klassenplan in mindestens einer Unterrichtswoche des Planungszeitraums mehr Springstunden aufweist, als im Dialogfenster „Automa-tikvorgaben“ auf der Registerkarte „Klassenvorgaben“ in der Spalte „Max. Springstunden je Woche“ angegeben sind. Voraussetzung dafür, dass diese Kategorie ausgewertet wird, ist, dass die Vorgabe „Klassenspringstunden beachten“ in den allgemeinen Automatikvorgaben mindestens mit dem Wert „1“ gewichtet wurde.
**Fach in gleicher Stunde** Unter dieser Rubrik werden Termine eines Fachs aufgelistet, die an die gleiche Tagesposition im Wochenplan gesetzt wurden.
Gleiches Fach mehrfach am Tag Unter dieser Rubrik werden Termine eines Fachs aufgelistet die am gleichen Wochentag verplant wurden.
**Mehrstündige Termine am Nachmittag** Unter dieser Rubrik werden mehrstündige Termine aufge-führt, die an eine Nachmittagsposition platziert wurden. Als Nachmittagsunterricht gilt dabei jeder Termin, der nach der im Feld „Vormittag bis“ eingestellten Uhrzeit verplant wurde.
**Mehrstündige Fächer in Tagesfolge** Unter dieser Rubrik werden mehrstündige Termine aufgeführt, die an direkt aufeinander folgenden Tagen verplant wurden
**1-stündiges Fach in 6. Stunde** Unter dieser Rubrik werden Einzelstundentermine aufgelistet, die an die 6. Tagesposition gesetzt wurden.
**1-stündige Termine samstags** Unter dieser Rubrik werden Einzelstundentermine aufgelistet, die an eine Samstagsposition platziert wurden.
**2-stündiger Termin samstags** Unter dieser Rubrik werden Doppelstundentermine aufgelistet, die an eine Samstagsposition platziert wurden.

## Reststunden verplanen

Möglicherweise sind nach einem Automatikdurchlauf unverplante Stunden übrig geblieben, die aufgrund der Vorgaben nicht verplant werden konnten. Reststunden einer Veranstaltung werden in der ersten Spalte „Unverplant“ der Veranstaltungsliste ausgewiesen. Vollständig verplante Veranstaltungen (d.h. keine Reststunden) werden mit der Zahl „0“ angezeigt; überall dort, wo eine Zahl größer als „0“ zu sehen ist, sind noch Reststunden übrig.

Die unverplanten Unterrichtstermine eines Klassen-, Lehrer-, Raum- oder Fachplans können Sie darüber hinaus im Detailfenster ``Unverplant`` des Teilfensters ``Detailbereich`` sehen. Von hier aus können Sie die verbliebenen Reststunden manuell verplanen.
Im Dialogfenster ``Auswahl`` für die Planauswahl können Sie im Feld "Anzeigen" den Filter ``Mit unverplanten Terminen`` wählen. Mit dieser Einstellung werden Ihnen im Auswahlfenster für den Planaufruf nur die Klassen, Lehrer bzw. Räume angezeigt, die noch unverplante Reststunden aufweisen.
