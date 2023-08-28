# Die Veranstaltungsliste

## Allgemeines

Grundlage für die spätere Unterrichtsverteilung bildet die Veranstaltungsliste, die folgendes bestimmt:

* Welche Klassen hat welchen Unterricht?
* Welche Lehrer unterrichten welches Fach in den Klassen?(Lehrereinsatzplanung)
* Welche Räume sind neben dem Klassenraum für bestimmte Veranstaltungen vorgesehen? (Raumeinsatzplanung)

Die sogenannte Veranstaltungsliste in DAVINCI ist eine Liste von Veranstaltungen für jede Klasse. Dabei wird jede Veranstaltung im wesentlichen durch das Fach und die entsprechende Klasse charakterisiert. Jede Veranstaltung hat eine vorgegebene "Dauer" (eine Anzahl von Terminen). So soll z.B. ein Fach "Deutsch" insgesamt mit einer "Dauer" von 5 Stunden unterrichtet werden. Diese Stunden sollen sich auf die drei Termine "2-2-1" aufteilen, also zwei Doppelstunden und eine Einzelstunde. Die Termine übernehmen im Regelfall die Angaben der Veranstaltung, also beispielsweise das Fach, den Fachschwerpunkt, den Lehrer, den Raum, die Block Bezeichnung usw. Ein besonderes Merkmal in DAVINCI ist es allerdings, dass im Spezialfall diese Eigenschaften auch für jeden Termin einzeln eingegeben werden kann. So soll z.B. nur einer der drei Termine mit anderen Terminen geblockt sein.

Die Verplanung des Unterrichts findet hauptsächlich in den Einzelklassenplänen statt. Die anderen Planarten, wie z.B. Lehrer- und Raumpläne, kommen vorwiegend ergänzend oder zur Feinabstimmung bereits fortgeschrittener Stundenpläne zum Einsatz. Deshalb wird in diesem und den nächsten Abschnitten die Planansicht „Klasse“ im Mittelpunkt der Darstellung stehen.

### So beginnen Sie

Wenn Sie zum ersten Mal den Stundenplan einer neuen Klasse aufrufen, dann ist das Programmfenster leer, d.h. es sind noch keine Daten über Unterrichtsveranstaltungen und Termine vorhanden. Zu Beginn müssen Sie daher die Veranstaltungsliste der neuen Klasse mit Daten füllen, bevor Sie im Planungsfenster die Stundenplanung ausarbeiten können.
Grundsätzlich stehen Ihnen zwei Wege zur Verfügung, wie Sie im Bereich Stundenplan neue Veranstaltungen erzeugen können:

1. Sie können neue Veranstaltungen aus den Stundentafeln erzeugen.
2. Sie können Veranstaltungen vollständig neu anlegen.

Beide Möglichkeiten werden wir im Folgenden gesondert darstellen.

!!! info "Hinweis"

    Zum Erzeugen und Bearbeiten von Veranstaltungen empfehlen wir Ihnen den Wechsel in die Ansicht ``Liste``. Klicken Sie dazu in der Menügruppe `Ansicht > Anordnung` auf ``Liste``

![Veranstaltungsliste](/assets/images/Veranstaltungsliste02.png)

In der Ansicht „Liste“ bereiten Sie die Unterrichtsveranstaltungen für das manuelle oder automatische Setzen vor. Folgende Spalten stehen in der Veranstaltungsliste zu Verfügung:

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
Unterrichtsart | siehe  ``Extras > Schlüsselverzeichnisse > Unterrichtsarten``, wichtige Differenzierung z.B. für Leistungs- und Grundkurse sowie Profilfächer für die gymnasiale Oberstufe
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

## Veranstaltungen aus Stundentafel erzeugen

Wenn Sie den Klassen in den Stammdaten eine Stundentafel zugeordnet haben, dann können Sie aus den dort hinterlegten Fächerlisten Veranstaltungen generieren. Die in den Stundentafeln eingetragenen Fachinformationen werden in die entsprechenden Felder der Veranstaltungsliste übertragen. Dabei können Sie zwischen den folgenden beiden Optionen wählen:

1. Sie können für alle Klassen gleichzeitig die auf den Stundentafeln eingetragenen Daten in die zugehörigen Veranstaltungslisten übertragen.
2. Sie können nur für den gerade bearbeiteten Klassenplan die Fachdaten aus einer bestimmten
Stundentafel kopieren. Hierbei können Sie aus allen Stundentafeln wählen, die Sie in den Stammdaten angelegt haben.

!!! info "Hinweis"

    Das Anlegen und Zuweisen einer Stundentafel erweist sich immer dann als sinnvoll, wenn eine Klasse vorwiegend im Klassenverband unterrichtet wird. Erfolgt der Unterricht z.B. in der gymnasialen Oberstufe oder an einer Hochschule hingegen überwiegend im Kurssystem ist die Arbeit mit einer festen Stundentafel in der Regel zu umständlich.

Zu Beginn der Arbeit mit dem Programmbereich `„Stundenplan“` empfiehlt es sich, für die meisten Klassen an allgemein- und berufsbildenden Schulen die erste Option zu wählen. Damit werden alle auf den Stundentafeln hinterlegten Fächer und Soll-Stunden in die zugehörigen Veranstaltungslisten kopiert und können für die weitere Planung genutzt werden. Die Nutzung der zweiten Variante ist hingegen dann sinnvoll, wenn nachträgliche Änderungen an einer Stundentafel in die Veranstaltungsliste der zugehörigen Klasse übernommen werden sollen

Um Veranstaltungen aus den in den Stammdaten erfassten Stundentafeln zu erzeugen, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie den Stundenplan einer bestimmten Klasse auf.
2. Betätigen Sie in der Menügruppe `„Start > Veranstaltungen`“ den unteren Teil der Schaltfläche `Neue Veranstaltung`.

![Aus Stundentafel erzeugen](/assets/images/ausstundentafel.png)

3. Wählen Sie den Eintrag `Aus Stundentafel erzeugen` aus dem Aufklappmenü.
4. Aktivieren Sie die Option `„Für alle Klassen ohne Veranstaltungen“`, wenn Sie Veranstaltungen für alle Klassen mit einer zugewiesenen Stundentafel erzeugen möchten.
Oder
Aktivieren Sie die Option `„Nur für die Klasse“`, wenn Sie nur für die bearbeitete Klasse Veranstaltungen aus einer ausgewählten Stundentafel erzeugen möchten und wählen Sie das Kürzel der gewünschten Stundentafel aus dem zugehörigen Aufklappmenü. Bestätigen Sie Ihre Auswahl abschließend mit OK.

!!! info "Hinweis"

    Für jeden Eintrag in den ausgewählten Stundentafeln wird nun eine Veranstaltungszeile angelegt. Die angelegten Veranstaltungszeilen enthalten die Fachdaten aus den kopierten Stundentafeln sowie verschiedene Informationen, die in den Stammdaten der Klassen und Fächer bereits eingetragen wurden. Dabei werden die entsprechenden Spalten mit Informationen gefüllt. 


!!! info "Hinweis"

    Die Einträge, die beim Kopieren der Stundentafeln in die Veranstaltungsliste kopiert werden, können nachträglich verändert oder ergänzt werden. Die Ausnahme bildet der Soll-Stunden-Wert. Wenn Sie die Soll-Stunden-Anzahl eines Unterrichtsfachs im Nachhinein ändern möchten, so ändern Sie bitte den Stundenwert in der Stundentafel. Im Klassenplan– bzw. –liste geht das am schnellsten indem Sie das Detailfenster „Summen“ links öffnen und auf die Schaltfläche „Stundentafel“ klicken. 

## Veranstaltung anlegen und bearbeiten

Für die Erfassung und Bearbeitung neuer bzw. bereits erzeugter Veranstaltungen steht Ihnen in DAVINCI 6 ein zentrales Dialogfenster zur Verfügung. Wie Sie mit diesem Dialogfenster neue Veranstaltungen von Grund auf anlegen bzw. die aus den Stundentafeln erzeugten Veranstaltungen um weitere Informationen ergänzen können, erfahren Sie im folgenden Abschnitt.

Die Vorgehensweise zum Öffnen des benötigten Dialogfensters `„Veranstaltung“` unterscheidet sich, je nachdem, ob Sie eine bestehende Veranstaltung bearbeiten oder eine neue Veranstaltung anlegen möchten.

Wenn Sie eine Veranstaltung bearbeiten möchten, die Sie z.B. vorher aus einer Stundentafel erzeugt haben, so führen Sie bitte folgende Schritte aus:

1. Markieren Sie in der Veranstaltungsliste die Zeile der gewünschten Veranstaltung
2. Klicken Sie in der Menüleiste `„Start > Veranstaltungen“` auf den oberen Teil der Schaltfläche `Veranstaltung bearbeiten`.
3. Es öffnet sich das Dialogfenster „[Fachkürzel]Veranstaltung“, in dem Sie Angaben zur gewählten Veranstaltung ergänzen oder ändern können.

![](/assets/images/veransatltung bearbeiten.png)

Auf der Seite „Veranstaltung“ des Dialogfensters `Veranstaltung` können Sie Veranstaltungsdaten bearbeiten und neue Veranstaltungen anlegen.

Wenn Sie hingegen eine neue Veranstaltung erzeugen möchten, gehen Sie bitte folgendermaßen vor:

1. Rufen Sie den Stundenplan der gewünschten Klasse auf.
2. Klicken Sie in der Menüleiste `Start > Veranstaltungen` auf den oberen Teil der Schaltfläche `Neue Veranstaltung`.
3. Es öffnet sich das Dialogfenster ``[Neue] Veranstaltung``, in dem Sie die Daten der neuen Unterrichtsveranstaltung eingeben können.
4. Das Dialogfenster ``Veranstaltung`` öffnet sich auf beiden Wegen jeweils mit der Seite ``Veranstaltung``.
5. Die Dialogseite „Veranstaltung“ zeigt eine Erfassungsmaske für Veranstaltungsdaten, mit diversen Eingabe- und Auswahlfeldern. In dieser Eingabemaske befinden sich u.a. die meisten Datenfelder zur Eingabe und Bearbeitung der Spaltenwerte der zugehörigen Veranstaltungszeile. Sie tragen  den gleichen Namen wie die entsprechenden Spalten der Veranstaltungsliste. So heißt z.B. das Eingabefeld für das Unterrichtsfach einer Veranstaltung „Fach“ genauso wie die zugehörige Spalte in der Veranstaltungsliste.

Um die zugehörigen Spaltenwerte der Veranstaltungsliste einzutragen oder zu ändern, müssen Sie eine entsprechende Eingabe in den gleichnamigen Feldern der Erfassungsmaske vornehmen. Führen Sie dazu in diesen Eingabefeldern die folgenden Schritte aus:

**Nr: **Geben Sie hier die zutreffende Veranstaltungsnummer einfach über die Tastatur ein.

**Fach**: Das Feld „Fach“ verweist auf die Liste der Fächer in den Stammdaten. Um einer Veranstaltung ein bestimmtes Unterrichtsfach zuzuweisen, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Kursnr.:** Im ergänzenden Eingabefeld „Kursnummer“ können Sie dem Unterrichtsfach eine Kursnummer hinzufügen. Die Kursnummer wird im Spaltenfeld „Fach“ der zugehörigen Veranstaltungszeile ohne Leerzeichen an das Fachkürzel angehängt. Geben Sie die zutreffende Kursnummer einfach über die Tastatur ein.

**Bemerkung** Geben Sie hier den gewünschten Bemerkungstext einfach über die Tastatur ein

**Block:** Das Feld „Block“ stellt ein kombiniertes Datenfeld für die Eingabe und Auswahl des geeigneten Blockkürzels dar. Sie können hier sowohl über die Tastatur ein neues Blockkürzel frei eingeben als auch in einem hinterlegten Übersichtsfenster aus einer Liste der in der Plandatei bereits vorhandenen Blockkürzel auswählen. Sie können also in diesem Feld für die bearbeitete Veranstaltung einen neuen Block erstellen, ebenso aber diese Veranstaltung einem bereits existierenden Block zuordnen.

**Dauer/ Rest:** Im Feld „Dauer/ Rest“ wird die Dauer der Veranstaltung in Schulstunden dem unverplanten Rest dieses Stundenwerts gegenübergestellt. Der Wert der Veranstaltungsdauer ergibt sich aus der Summe der einzelnen Veranstaltungstermine. Eine Veranstaltung mit einem Einzel und einem Doppelstundentermine erhält demzufolge die Dauer „3“ unabhängig davon, ob die Termine in allen Wochen gleich stattfinden.

**Termine:** Im Feld „Termine“ geben Sie die Terminserie einer Veranstaltung ein. Über diese Eingabe bestimmen Sie automatisch die Dauer einer Veranstaltung. Tragen Sie im Eingabefeld „Termine“ eine selbstdefinierte Terminserie ein oder wählen Sie eine der vordefinierten Terminserien aus dem Aufklappmenü. Dabei gelten folgende Eingabekonventionen.

**Termindauer: **Der Wert einer ganzen Zahl definiert die Dauer eines Einzeltermins der bearbeiteten Veranstaltung in Unterrichtsstunden. Die Zahl „1“ steht für eine Einzelstunde, die Zahl „2“ für eine Doppelstunde die Zahl „3“ für einen Termin mit 3 Stunden usw.

**Terminanzahl: **Die Menge der ganzen Zahlen getrennt durch einen Bindestrich ohne Leerzeichen
definiert die Anzahl der Unterrichtstermine. Die Notation „1-1“ steht für zwei Einzelstunden, die Notation „1-2“ für eine Einzelstunde und eine Doppelstunde“ usw. Die aus der eingetragenen Terminserie resultierende Veranstaltungsdauer wird im Feld „Dauer/ Rest“ entsprechend angepasst.

**Unabhängig vom Block:** Mit dem Haken im Kontrollkästchen an dieser Stelle legen Sie fest, dass verschiedene Einstellungen bezüglich der Veranstaltungen unabhängig von den entsprechenden 
Einstellungen anderer Veranstaltungen im gleichen Block beibehalten werden. Dies betrifft z.B. die Dauer, aber auch verschiedene Automatikvorgaben der Veranstaltung.

**Schüleranzahl:** Geben Sie die zutreffende Schülerzahl einfach über die Tastatur ein oder benutzen Sie die beiden integrierten Pfeilschaltflächen um den angegebenen Zahlenwert hoch- oder runterzusetzen. Standardmäßig ist hier der Wert eingetragen, den Sie in den Stammdaten der Klasse im Feld „Schüler“ eingetragen haben.

**Periode:** Das Feld „Periode“ verweist auf die Liste der Perioden in den Stammdaten. Um einer Veranstaltung eine bestimmte Periode zuzuweisen, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Gültig von/ bis:** Mit diesen beiden Feldern können Sie den Geltungszeitraum der zugewiesenen
Periode auf ein genaues Anfangs- und Enddatum einschränken. Wenn z.B. der Unterricht in der ersten Periodenwoche nicht direkt am Montag, sondern erst am Mittwoch beginnt, dann können Sie im Feld neben „Gültig von“ das genaue Datum des ersten Unterrichtstages eintragen. Diese Einschränkung wird später von DAVINCI beim manuellen und automatischen Setzen berücksichtigt. Bei periodischem Montagsunterricht taucht die zugehörige Veranstaltung in der ersten Periodenwoche nicht im Plan auf. Wenn z.B. der Unterricht in der letzten Periodenwoche nicht erst am Freitag, sondern schon am Mittwoch endet, dann können Sie im Feld neben „bis“ das genaue Datum des letzten Unterrichtstages eintragen. Auch diese Information wird von daVinci beim Setzen des Unterrichts berücksichtigt. Bei periodischem Freitagsunterricht taucht die zugehörige Veranstaltung in der letzten Periodenwoche nicht im Plan auf.

**Wochen:** Das Feld „Wochen“ zeigt an, ob eine Veranstaltung in allen oder nur in bestimmten Unterrichtswochen stattfindet. Der Eintrag „Jede Woche“ weist darauf hin, dass eine Veranstaltung uneingeschränkt in allen Unterrichtswochen stattfindet. Findet Unterricht (in der Regel aufgrund einer Periode) nur in ausgewählten Unterrichtswochen statt, werden die Nummern der zugehörigen Kalenderwochen im Feld „Wochen“ eingeblendet.

## Sollstunden und Terminserie

Wenn Sie eine Veranstaltung aus der Stundentafel erzeugen, dann wird der bei dem Fach auf der
Stundentafel hinterlegte Wert in der Spalte „Soll“ als Veranstaltungsdauer vorbesetzt. Ebenso wird standardmäßig eine Terminserie eingerichtet. Die Aufteilung der Veranstaltungsdauer auf einzelne Termine, orientiert sich dabei an den Vorgaben, die Sie in den Programmoptionen zur Standardtermindauer, gemacht haben. Falls dort eine Standardtermindauer von „1“ hinterlegt wurde teilt DAVINCI beim Kopieren der Stundentafel die Gesamtdauer automatisch in Einzelstundentermine. Bei einem höheren Wert werden – so weit möglich – entsprechende Mehrstundentermine angelegt. Der nicht mehr durch den vorgegebenen Standardwert teilbare Rest wird in Einzelstundentermine zerlegt.

Um die Standardtermindauer in den Programmoptionen festzulegen, gehen Sie bitte folgendermaßen
vor:

1. Blättern Sie im Menüband zur Registerkarte `Extras`.
2. Klicken Sie in der Menügruppe `Verwalten > Optionen`.
3. Folgen Sie in der Navigationsleiste des Dialogfensters `Optionen` dem Link Einstellungen. 
4. Setzen Sie im Bereich ``Veranstaltungsliste`` der Dialogseite ``Einstellungen`` den Haken im Kontrollkästchen vor ``Einzeltermine der Dauer``
5. Tragen Sie im Eingabefeld neben ``Einzeltermine der Dauer`` den gewünschten Standardwert für die Termindauer ein.
6. Bestätigen Sie Ihre Angaben mit `OK`.

![Termindauer](/assets/images/Termindauer.png)

Der bearbeitete Stundenwert wird nun als Standardtermindauer für die Einrichtung von Terminserien zugrunde gelegt.

## Einer Veranstaltung eine Periode zuweisen

Wenn Sie der Veranstaltung keine Periode zugewiesen haben, können Sie die Unterrichtswochen der
Veranstaltung im Dialogfenster „Veranstaltung“ individuell auswählen. Gehen Sie dazu folgendermaßen vor:

1. Betätigen Sie die Schaltfläche `Bearbeiten` rechts neben dem Feld „Wochen“.
2. Entfernen Sie im erscheinenden Dialogfenster „Wochen bearbeiten“ den Haken vor den Kalenderwochen, in denen die Veranstaltung nicht unterrichtet werden soll.
3. Bestätigen Sie Ihre Einstellungen im Dialogfenster „Wochen bearbeiten“ mit `OK`. Die Kalenderwochen der verbliebenen Unterrichtswochen werden nun im Feld „Wochen“ angezeigt.

![Wochen bearbeiten](/assets/images/wochenbearbeiten1.png)

### Weitere Zuweisungen

**Zeitschiene:** In diesem Feld können Sie die Zeitschiene auswählen, auf der eine Veranstaltung angesiedelt ist. Standardmäßig ist hier die Zeitschiene „A“ hinterlegt. Darüber hinaus stehen die Zeitschienen „B“, „C“, „D“, „E“ sowie „X“ und „Y“ zur Verfügung. Durch die Zuweisung von Zeitschienen, können Sie der Setzautomatik detaillierte Vorgaben machen, welche Veranstaltungen sich im Plan überschneiden dürfen und welche nicht. Dabei gelten folgende Regeln:

* Veranstaltungen, die sich auf der gleichen Zeitschiene befinden, dürfen von der Automatik nicht zum gleichen Zeitpunkt verplant werden, es sein denn diese Veranstaltungen befinden sich in einem gemeinsamen Block.
* Veranstaltungen, die sich auf einer der Zeitschienen „A“ bis „E“ befinden, dürfen mit anderen
Veranstaltungen, die sich auf einer anderen der Zeitschienen „A“ bis „E“ befinden zum gleichen
Zeitpunkt verplant werden.
* Veranstaltungen, sich auf der Zeitschiene „X“ befinden dürfen sich im Plan mit keiner anderen Veranstaltung der gleichen oder einer anderen Zeitschiene überschneiden, es sei denn die Veranstaltungen befinden sich in einem gemeinsamen Block.
* Veranstaltungen, sich auf der Zeitschiene „Y“ befinden dürfen sich im Plan mit allen anderen
Veranstaltungen der gleichen oder einer anderen Zeitschiene überschneiden, es sei denn diese Veranstaltungen befindet sich auf der Schiene „X“.

Um einer Veranstaltung die gewünschte Zeitschiene zuzuweisen, wählen Sie bitte den zutreffenden
Eintrag aus dem Aufklappmenü des Feldes „Zeitschiene“.

**Raum:** Das Feld „Raum“ verweist auf die Liste „Räume“ in den Stammdaten.

**Raumart:** In diesem Feld können Sie die Raumart hinterlegen, die von der Automatik bei der Zuweisung eines Unterrichtsraums für die Veranstaltung berücksichtigt werden soll. Das Feld "Raumart“ verweist auf das Schlüsselverzeichnis „Raumarten“. Um einer Veranstaltung eine bestimmte Raumart zuzuweisen, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Vorgaben:** Nicht alle Spaltenwerte der Veranstaltungsliste können Sie allerdings über die Felder der Seite „Veranstaltung“ des aufgerufenen Dialogfensters eintragen oder verändern. Dies betrifft insbesondere die Spalten „Räume“, „Lehrer“ und „Klassen“ der Veranstaltungsliste. Die Einträge dieser Felder zählen zur Kategorie der Veranstaltungsteilnehmer für deren Bearbeitung das Dialogfenster die Ansicht „Teilnehmerplanung“ zur Verfügung stellt.

Die zugewiesenen Teilnehmer einer Unterrichtsveranstaltung, also u.a. Klassen, Räume, Lehrer, sehen Sie auf der Dialogseite „Veranstaltung“ im Anzeigefeld neben der Schaltfläche Vorgaben. Wenn Sie auf der Dialogseite gerade eine neue Veranstaltung erfassen, dann enthält dieser Bereich bereits den Vertreter der Planart, dessen Stundenplan Sie aktuell bearbeiten.

!!! info "Hinweis"

    Wie Sie einer Unterrichtsveranstaltung im Dialogfenster „Veranstaltung“ Lehrer und Räume zuweisen können, erfahren Sie im Abschnitt [Teilnehmer zu einer Veranstaltung hinzufügen](/01.stundenplan/teilnehmer-zuweisen/).

Neben den Spalten „Räume“, „Lehrer“ und Klassen“ kann außerdem die Spalte „Fachfolge“ nicht über die Dialogseite Veranstaltung bearbeitet werden. Für die Eingabe des Fachfolgekürzels steht im Dialogfenster „Veranstaltung“ die Teilansicht „Zeitdetails“ zur Verfügung, mit der Sie die Automatikvorgaben einer Veranstaltung bearbeiten können.

Darüber hinaus hat die Dialogseite „Veranstaltung“ einige zusätzliche Felder für die Eingabe von Daten, die nicht in der Veranstaltungsliste angezeigt werden. Diese Felder sollen im Folgenden gesondert vorgestellt werden:

**Titel:** In diesem Feld können Sie einen Titel für die Veranstaltung erfassen. Dieser Titel wird in der Kalenderansicht der Veranstaltungstermine, die Ihnen im Programmbereich „Kalender“ zur Verfügung steht, angezeigt.

**Wiederholung:** Mit dem Eintrag in diesem Feld geben Sie an, ob eine Veranstaltung wiederkehrend in allen Unterrichtwochen bzw. den Wochen der zugewiesenen Periode oder nur einmalig in einer bestimmten Unterrichtswoche stattfinden soll. Standardmäßig ist hier der Eintrag „Periodisch“ für wiederkehrenden Unterricht voreingestellt. Um anzugeben, dass eine Veranstaltung nur in einer bestimmten Woche stattfinden soll, wählen Sie bitte den Eintrag „Einmalig“ aus dem Kontextmenu.

!!! info "Hinweis"

    Die Einstellung im Feld „Wiederholung“ kann nur beim Anlegen einer Veranstaltung angepasst werden.
Bitte beachten Sie, dass Veranstaltungen, die Sie aus einer Stundentafel erzeugen, automatisch zunächst als wiederkehrende Veranstaltungen angelegt werden. Um eine wiederkehrende Veranstaltung im Nachhinein in eine einmalige zu verwandeln, gehen Sie bitte folgendermaßen vor:

1. Markieren Sie die Veranstaltung in der Veranstaltungsliste.
2. Klicken Sie in der Menügruppe `Start > Veranstaltungen` auf die untere Hälfte der Schaltfläche `Veranstaltung bearbeiten`.
3. Wählen Sie den Befehl `In Einzeltermine umwandeln` aus dem Aufklappmenü
Die Wiederholungsart der Veranstaltung wird nun von **Periodisch** in **Einmalig** geändert.

**Art:** In diesem Feld können Sie die „Unterrichtsart“ der Veranstaltung zuordnen. Das Feld „Art“ greift auf das Schlüsselverzeichnis „Unterrichtsarten“ zu. Um eine Veranstaltung nach Ihrer Unterrichtsart zu kategorisieren, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Fachstatus: **In diesem Feld können Sie den „Fachstatus“ der Veranstaltung zuordnen. Die Eingabe des Fachstatus hat keine direkte Funktion für die Stundenplanung. Sie hat ausschließlich informativen Charakter, kann aber neben statistischen Zwecken z.B. auch für den Datenabgleich mit dem Schulverwaltungsprogramm Magellan wichtig sein. Das Feld „Fachstatus“ greift auf das Schlüsselverzeichnis „Fachstatus“ zu. Um eine Veranstaltung nach Ihrem Fachstatus zu kategorisieren, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Schulform:** In diesem Feld können Sie eingeben welcher Schulform die Veranstaltung zugeordnet ist. Die Eingabe der Schulform hat keine direkte Funktion für die Stundenplanung. Sie hat ausschließlich informativen Charakter und kann z.B. für statistische Zwecke genutzt werden. Das Feld „Schulform“ greift auf das Schlüsselverzeichnis „Schulformen“ zu. Um eine Veranstaltung nach Ihrer Schulform zu kategorisieren, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Unterrichtsform: **In diesem Feld können Sie die Unterrichtsform der Veranstaltung spezifizieren. Die Eingabe der Unterrichtsform hat keine direkte Funktion für die Stundenplanung. Sie hat ausschließlich informativen Charakter und kann z.B. für statistische Zwecke genutzt werden. Das Feld „Unterrichtsform“ greift auf das Schlüsselverzeichnis „Unterrichtsformen“ zu. Um eine Veranstaltung nach Ihrer Unterrichtsform zu kategorisieren, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Merkmal:** In diesem Feld können Sie der Unterrichtsveranstaltung ein zusätzliches Merkmal zuordnen. Die Eingabe eines zusätzlichen Merkmals hat keine direkte Funktion für die Stundenplanung. Sie hat ausschließlich informativen Charakter und kann z.B. für statistische Zwecke genutzt werden.  Das Feld „Merkmal“ greift auf das Schlüsselverzeichnis „Merkmale“ zu. Um eine Veranstaltung nach einem zusätzlichen Merkmal zu kategorisieren, wählen Sie bitte den gewünschten Eintrag aus dem Aufklappmenü.

**Intern:** In diesem Feld können Sie ergänzende Informationen zu einer Veranstaltung eintragen. Der Eintrag, den Sie hier vornehmen besitzt keine direkte Relevanz für die Stundenplanung. Er hat rein informativen Charakter und kann z.B. für die interne Abstimmung mit anderen Planern genutzt werden.

Um die eingegebenen oder bearbeiteten Daten zu speichern, bestätigen Sie Ihre Angaben abschließend mit `Schließen`. Falls Sie eine Veranstaltung neu angelegt haben, so wird eine neue Zeile mit den zugehörigen Daten in der Veranstaltungsliste hinzugefügt. Damit eine neue Veranstaltung angelegt werden kann, müssen Sie mindestens eine Eingabe in den Feldern „Fach“ oder „Titel“ vornehmen.

!!! info "Hinweis"

    Wenn Sie mehrere Veranstaltungen einer Klasse nacheinander bearbeiten möchten, so müssen Sie das Dialogfenster nicht für jede Veranstaltung schließen und neu aufrufen. Klicken Sie bei geöffnetem Dialogfenster einfach auf die Zeile der nächsten zu bearbeitenden Veranstaltung in der Veranstaltungsliste der Klasse.
Darüber hinaus besteht die Möglichkeit mehrere Instanzen des Dialogfensters „Veranstaltung“ parallel zu öffnen. Auf diese Weise können Sie mehrere Veranstaltungen in der synchronen Zusammenschau anlegen bzw. bearbeiten.
