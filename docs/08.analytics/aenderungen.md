# Übersicht „Änderungen“

Diese Übersicht listet pro Tag die zur Vertretung anfallenden
Stunden auf und schlüsselt auf, wie diese vertreten wurden bzw. wie viele Stunden davon ausgefallen sind. Diese Übersicht kann insbesondere für die PES Statistik (Rheinland-Pfalz) und die Lehrerausfallstatistik in Bremen
und Schleswig-Holstein verwendet werden.
Das Ergebnis wird wie folgt angezeigt:

Register | Erläuterungen
--------|-------------------------------------------
Ausfall | Summe der zur Vertretung anstehenden Stunden je Tag und die Summe der Ausfallstunden je Tag
Vertretungen | Summe der zur Vertretung anstehenden Stunden je Lehrer und je Tag
Diagramm | Grafische Darstellung der Liste auf der Registerkarte „Ausfall“
Pivot | Pivot Tabelle der Registerkarte „Vertretungen“

## Filterangaben

So sollten Sie vorgehen:

![Filterangaben](/assets/images/Filter.png)

1. Stellen Sie unter ``Fehlgrund Schlüssel`` den Fehlgrund für ``krank`` ein.
2. Stellen Sie unter ``Lehrerart Schlüssel`` die Lehrerart
``Lehrer`` ein.
3. Stellen Sie unter ``Entfallgrund Schlüssel`` den Entfallgrund
``Selbstorganisierendes Lernen`` ein.
4. Klicken Sie auf ``Aktualisieren`` um die Liste neu anzuzeigen. Indem Sie mehrere oder alle Zeilen der Liste markieren und auf Exportieren klicken, können Sie die Liste nach Excel und in andere Formate exportieren.

![Kopfspalten](/assets/images/aenderungen01.png)

## Register Ausfall

Die Übersicht unterscheidet Vertretungen durch Lehrer von Vertretungen durch Erzieher, Betreuer oder andere. Zudem wird der Entfall einer Vertretung durch selbstorganisiertes Lernen erfasst. Dazu müssen Sie die folgenden Schlüsselverzeichnisse verwenden:

* ``Extras > Schlüsselverzeichnisse > Lehrerarten``
* ``Extras > Schlüsselverzeichnisse > Vertretungsentfallgründe``

Im Bereich „Filter“ können Sie angeben, über welchen Lehrerarten-Schlüssel ein „Lehrer“ ausgezeichnet wurde und welcher Entfallgrund-Schlüssel „Selbstorgansiertes Lernen“ kennzeichnet. Sie müssen dazu jeden Lehrer in
der Ansicht ``Stammdaten > Lehrer`` in der Spalte „Art“ als „Lehrer“, „Betreuer“, „Erzieher“ oder anders kennzeichnen. Den Entfallgrund weisen Sie bei der Erstellung eines Entfalls in der Ansicht ``Vertretungsplan > Vertretungen`` im entsprechenden Dialogfenster zu. Bitte beachten Sie,
dass eine Reihe der Filterangaben nach dem Schlüssel und nicht nach dem Kürzel filtern, d.h. Sie sollten entsprechend die Spalte „Schlüssel“ in den Verzeichnissen ``Lehrerarten`` und ``Vertretungsentfallgründe`` gefüllt haben. Standardmäßig können Sie den Wert aus der Spalte „Kürzel“ in die Spalte „Schlüssel“ übertragen.

### Bereich Zeit

Spalte | Erläuterungen
--------|-------------------------------------------
Status | Ein ausgefüllter schwarzer Stern kennzeichnet Tage des aktuellen Gültigkeitszeitraums der Plandatei siehe ``Plan > Eigenschaften > Zeitraum``, ein nicht ausgefüllter Stern Tage außerhalb des Zeitraums.
Monat | Monat des Datums
Woche | Kalenderwoche des Datums
Datum | Tagesdatum
Tag | Wochentag

### Bereich Info

Spalte | Erläuterungen
--------|-------------------------------------------
Lehreranzahl | Anzahl der Lehrer an diesem Tag
Lehrerausfall | Summe der zur Vertretung anfallenden Unterrichtsstunden (ohne Raumvertretungen und Pausenaufsichtsvertretungen)
Anrechnen | Summe der Anrechenstunden an diesem Tag

### Bereich Lehrerausfall

![Lehrerausfall](/assets/images/aenderungen02.png)

Spalte | Erläuterungen
--------|-------------------------------------------
Geplant | Summe der geplanten Unterrichtsstunden des Tages
Ist | Summe tatsächlich Unterrichtsstunden des Tages
Ausfall | Summe der ausgefallenen Lehrerstunden des Tages
Zusätzlich | Summe der zustätzlichen Lehrerstunden des Tages
Fehlgrund | Summe der Stunden des Fehlgrunds für den Tag (Vertretungsstunden am Tag laut Filter „Fehlgrund Schlüssel“ (z.B. „krank“))
Andere Fehlgründe | Summe der Stunden, die nicht zu dem Fehlgrund gehören für den Tag (Summe der anderen Vertretungsstunden am Tag (Komplement zur Spalte „Fehlgrund“))
Krank | Anzahl der Fehlgrund.Schlüssel=`K` Entfälle für den Tag
Andere | Anzahl der Entfälle aus anderen Fehlgründen für den Tag

### Bereich Vertretung

![Vertretungen](/assets/images/Änderungen03.png)

Spalte | Erläuterungen
--------|-------------------------------------------
Lehrer Vertretungen Anzahl | Summe der Vertretungsereignisse durch Lehrer der Lehrerart für den Tag = Anzahl Vertretungen am Tag durch Lehrer der Lehrerart (siehe ``Extras > Schlüsselverzeichnisse > Lehrerarten``) laut Filter „Lehrerart Schlüssel“ (z.B. Lehrerart „Lehrer“) <img src=/assets/images/Lehrerart.png>
Lehrer Vertretungen Stunden | Anzahl Vertretungen am Tag durch andere z.B. Erzieher/Betreuer (Komplement zur Spalte „Lehrer Vertretungen“)
Andere Vertretungen Stunden | Summe der Vertretungen durch Personen, die nicht mit Lehrerart gekennzeichnet sind für den Tag
Andere Vertretungen Anzahl | Anzahl der Vertretungen durch Personen, die nicht mit Lehrerart gekennzeichnet sind für den Tag
Mitbetreuung Stunden | Summe der Mitbetreuungen an diesem Tag, d.h. der Stunden, die durch indirekte Vertreter unterrichtet werden (= Summe der indirekten Vertretungen für den Tag)
Mitbetreuung Anzahl | Anzahl der indirekten Vertretungen für den Tag
SOL Stunden | Summe der Selbst. organisiertes Lernen (SOL) Entfälle, die mit dem "Entfallgrund" als "SOL" gekennzeichnet wurden für den Tag (siehe ``Extras > Schlüsselverzeichnisse > Vertretungsentfallgründe`` laut Filter „Entfallgrund Schlüssel“ gekennzeichnet wurden)
<img src=/assets/images/SOL.png>
SOL Anzahl | Anzahl der Selbst. organisiertes Lernen (SOL) Entfälle, die mit dem "Entfallgrund" als "SOL" gekennzeichnet wurden für den Tag
Unterrichtsausfall Stunden | Unterrichtsausfall Stunden = LehrerAusfall - LehrerVertretungen - AndereVertretungen - Mitbetreuung - SOL

## Register Vertretungen

Spalte | Erläuterungen
--------|-------------------------------------------
Status | Ein ausgefüllter schwarzer Stern kennzeichnet Tage des aktuellen Gültigkeitszeitraums der Plandatei siehe ``Plan > Eigenschaften > Zeitraum``, ein nicht ausgefüllter Stern Tage außerhalb des Zeitraums.
Monat | Monat des Datums
Woche | Kalenderwoche des Datums
Datum | Tagesdatum
Tag | Wochentag
Fehlt| fehlender Lehrer
Vertreter| Vertretungslehrer
Fehlgrund| bei der Fehlzeit des Lehrers eingetragener Fehlergrund siehe Schlüsselverzeichniss `Extras > Schlüsselverzeichnisse > Lehrerfehlgründe`
Fach| Original- und Vertretungsfach
Vertretungsentfall| bei Vertretungsentfall eingetragener "Entfallgrund" siehe Schlüsselverzeichniss `Extras > Schlüsselverzeichnisse > Vertretungsentfallgründe`
Vertretungslehrermerkmal| Art des Vertretungseinsatzes <br> Zusätzlich: Zusatzunterricht<br>Verschoben: vorgezogener Unterricht<br> Mehrfach: Unterricht wird zusätzlich zum eigentlichen Unterricht  übernommen<br> Freigestellt: Lehrer wird aus dem eigentlichen Unterricht freigestellt und übernimmt die Vertretung
Vertretungslehrertyp| bei der Vertretung eingetragener Vertretungslehrertyp siehe Schlüsselverzeichniss `Extras > Schlüsselverzeichnisse > Vertretungslehrertyp`
Ausfall| durch eine Lehrerfehlzeit anfallende "Ausfallstunden"
Anrechenstunden| durch eine Vertretung entstandenen positive Anrechenstunden
Zusätzlich| durch Zusatzunterricht entstandene "zusätzliche Stunden"

## Register Diagramm

## Register Pivot
