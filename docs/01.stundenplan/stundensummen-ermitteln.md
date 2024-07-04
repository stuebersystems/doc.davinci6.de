# Stundensummen ermitteln

## Berechnungskonzepte

In DaVinci 6 stehen drei verschiedene Berechnungskonzepte zur Verfügung, die Sie für die Ermittlung der Stundensummen benutzen können:

* Faktorbezogene Berechnung
* Wochenbezogene Berechnung
* Tagesbezogene Berechnung

Je nachdem wofür bzw. in welcher Genauigkeit Sie die Daten benötigen, können Sie die Stundensummen unterschiedlich berechnen lassen. Jedes der drei Berechnungskonzepte berücksichtigt unterschiedliche Informationen in der Plandatei und führt zu unterschiedlichen Ergebnissen. Die Unterschiede beziehen sich dabei auf die Summen-Kategorien: „Lehrer-Ist“, „Lehrer-Ist in Klasse“ und „Schüler-Ist“.

Verrechnungsart | Beschreibung
- | -
Tagesbezogen |  Es wird jeden Tag die Anzahl der Stunden gezählt, wobei unterrichtsfreie Tage laut Kalender wie z.B. Ferien und Feiertage nicht mitgezählt werden. Das Resultat ist eine genaue Stundensumme über die Wochen und das Schuljahr, z.B. „2h je Woche in 20 Wochen des Schuljahres = 2h x 20 = 40h [im Schuljahr] => 40h / 40 Wochen = 1h/Woche [als Wochenmittelwert]“.
Wochenbezogen | Es wird jeden Tag die Anzahl der Stunden gezählt, wobei die in „Wochenbezogene Summe“ ausgenommenen Wochen nicht mitgezählt werden. Das Resultat ist eine gemittelte Stundensumme über die Wochen des Schuljahres, z.B. „2h x 20 Wochen / 40 Wochen = 1h [je Woche als Mittelwert]“
Faktorbezogen | Die jeweilige Stundendauer einer Veranstaltung wird mit dem Klassenfaktor (aus Klassensicht) bzw. dem Lehrerfaktor (bei Lehrersicht) multipliziert. Klassenfaktor und Lehrerfaktor können je Veranstaltung über das Dialogfenster „Veranstaltung“ manuell eingegeben werden oder errechnen sich automatisch aus dem Faktor der ggf. zugewiesenen Periode.

### Dauer und Wertung einer Unterrichtstunde festlegen

DaVinci Stundenplan errechnet auf der Basis der erstellten Unterrichtstermine automatisch die anfallenden Unterrichtsstunden. Dabei wird standardmäßig ein Ausgangswert von 45 Minuten pro Unterrichtsstunde vorausgesetzt. Diesen Ausgangswert für die Stundenzählung können Sie bei Bedarf an Ihre spezifischen Gegebenheiten anpassen.

!!! info "Hinweis"

    Der Wert für die statistische Einheit einer Unterrichtsstunde kann von dem Umfang abwei-chen, den Sie im Dialogfenster „Zeitrahmen“ für die Erstellung des Stundenrasters angegeben haben.

Standardmäßig geht DaVinci bei der Stundenzählung davon aus, dass jede geleistete Lehrerstunde unabhängig vom Fach, das gleiche Gewicht erhält. Wenn die Zählung der Lehrerstunden aber auf der Basis fachbezogener Wertfaktoren erfolgen soll, können Sie dies ebenfalls in den allgemeinen Statistikvorgaben des Programms festlegen.
Um die Dauer der Unterrichtsstunden an Ihre besonderen Erfordernisse anzupassen, gehen Sie bitte folgendermaßen vor:

1. Klicken Sie im Menüband auf die Schaltfläche ``Plan``.
2. Wählen Sie im Planmenü den Befehl ``Eigenschaften``.
3. Blättern Sie im Dialogfenster ``Eigenschaften`` zur Registerkarte ``Statistik``.
4. Geben Sie im Bereich ``Zeitdauerangaben`` im Eingabefeld neben ``1 Einheit = …`` den Wert einer Unterrichtsstunde in Minuten an.
5. Legen Sie im Eingabefeld vor ``Nachkommastelle(n)``, die Anzahl der Stellen nach dem Komma fest, die für die Darstellung der ermittelten Stundenwerte genutzt werden sollen.

![Plan-Eigenschaften, Statistik](/assets/images/Plan-EigenschaftenStatistik.png)

6. Bestätigen Sie Ihre Angaben abschließend mit ``OK``.

### Stunden mit Wertfaktoren

In einigen Regionen werden statistisch nicht die realen Zeitstunden sondern die mit Wertfaktoren gewichteten Stunden erfasst, siehe z.B. in Hamburg die Lehrerarbeitszeitkonten. Eine Stunde Mathematik erfordert mehr Vorbereitung als eine Stunde Sport. Daher wird beispielsweise die Mathematik Stunde mit dem Wertfaktor ``1,4`` und die Sport Stunde mit dem Wertfaktor ``1,0`` multipliziert.

Markieren Sie im Dialogfenster ``Plan-Eigenschaften`` im Bereich ``Verreichnungsart`` die Option ``Mit Wertfaktoren (aus Stundentafel, Fach, Klasse, Veranstaltung)``, wenn sie mit Wertfaktoren arbeiten möchten.

![Mit Wertfaktoren arbeiten](/assets/images/Plan-EigenschaftenStatistik01.png)

!!! info "Hinweis"

    Wie Sie im Programmbereich ``Stammdaten`` auf der Registerkarte ``Stundentafeln`` die Lehrer-Wertfaktoren der Unterrichtsfächer eingeben können, entnehmen Sie bitte dem Abschnitt [Stundentafeln](/davinci-stundenplan/stammdaten/stundentafeln.md).

### Faktorbezogene Berechnung aktivieren

![Summierung](/assets/images/Summierung.Faktorbezogen.png)

Bei diesem Berechnungskonzept werden die Wochendurchschnitts- und Jahresstundenwerte der genannten Summenkategorien auf der Basis wochenbezogener Berechnungsfaktoren gebildet. Alle Werte werden nur aufgrund der im Teilfenster ``Veranstaltungsliste`` vorhandenen Terminformationen ermittelt. Informationen über Ferien und Feiertage und andere schulfreie Ereignisse, die nur im Teilfenster ``Planungsfenster`` vorhanden sind, werden nicht berücksichtigt.

Um in den Dateieigenschaften die faktorbezogene Berechnungsart der Stundensummen zu aktivieren, gehen Sie bitte folgendermaßen vor:

1. Klicken Sie im Menüband auf die Schaltfläche ``Plan``.
2. Wählen Sie im Planmenü den Befehl ``Eigenschaften``.
3. Blättern Sie im Dialogfenster ``Eigenschaften`` zur Registerkarte ``Statistik``.
4. Wählen Sie im Bereich ``Verrechnungsart`` den Eintrag ``faktorbezogen`` aus dem Aufklappmenü des Feldes ``Summierung``.
5. Bestätigen Sie Ihre Angaben mit ``OK``. Die faktorbezogene Berechnung wird nun für die Ermittlung der Lehrer- und Klassenstunden aktiviert.

Bei der faktorbezogenen Berechnung fließen folgende Informationen in die Berechnung der Stundensummen ein:

* Die Angaben in der Spalte „Dauer/W“ der Veranstaltungsliste
* Der individuelle Klassenfaktor der Veranstaltungen.
* Der individuelle Lehrerfaktor der Veranstaltungen.
* Der allgemeine Wochenfaktor in den Statistikeigenschaften der Datei.
* Die Informationen über die ausgenommenen Wochen in den Statistikeigenschaften der Datei.
* Die Angaben in der Spalte „Block“ der Veranstaltungsliste
* Die Angaben in der Spalte „Wochen“ der Veranstaltungsliste

Der Klassen- und der Lehrerfaktor einer Veranstaltung werden von DaVinci automatisch ermittelt. Beide Faktoren können jeweils einen Wert zwischen „1“ und „0“ annehmen. Der Wert „1“ bedeutet, dass eine Veranstaltung in allen Unterrichtswochen des Planungszeitraums stattfindet.
Ein Wert kleiner als „1“ bedeutet, dass eine Veranstaltung nicht in allen Unterrichtswochen des Planungszeitraums stattfindet. Die Anzahl der Unterrichtswochen einer bestimmten Veranstaltung wird dabei durch den allgemeinen Wochenfaktor geteilt. Der allgemeine Wochenfaktor steht als statistischer Kennwert für die Anzahl aller Unterrichtswochen des Planungszeitraums und wird vom Planer im Vorfeld definiert.

### Wochenbezogene Berechnung

Bei der wochenbezogenen Berechnungsweise werden die Stundenwerte der Lehrer und Klassen in den vom Planer definierten Unterrichtswochen zu Jahresstundenwerten addiert. Die zugehörigen Durchschnittswerte ergeben sich, indem die Jahresstundenwerte durch den allgemeinen Wochenfaktor in den Statistikeigenschaften der Datei dividiert werden. Zur Ermittlung der Ist-Stundenwerte werden nur die im Teilfenster „Veranstaltungsliste“ verfügbaren Termininformationen herangezogen. Informationen über Ferien- und Feiertage und andere schulfreie Ereignisse, die nur im Teilfenster „Planungsfenster“ hinterlegt sind, werden nicht berücksichtigt. Allerdings wird berücksichtigt, wenn gesetzte Termine sich im Plan überschneiden z.B. aufgrund von Schienen.

Um in den Dateieigenschaften die wochenbezogene Berechnungsart der Stundensummen zu aktivieren, gehen Sie bitte folgendermaßen vor:

1. Klicken Sie im Menüband auf die Schaltfläche ``Plan``.
2. Wählen Sie im Planmenü den Befehl ``Eigenschaften``.
3. Blättern Sie im Dialogfenster ``Eigenschaften`` zur Registerkarte ``Statistik``. 
4. Wählen Sie im Bereich ``Verrechnungsart`` den Eintrag ``wochenbezogen`` aus dem Aufklappmenü des Feldes ``Summierung``.
5. Bestätigen Sie Ihre Angaben mit ``OK``. Die wochenbezogene Berechnung wird nun für die Ermittlung der Lehrer- und Klassenstunden aktiviert.

![Verrechnungsart wochenbezogen](/assets/images/Summierung.Wochenbezogen.png)

Bei der wochenbezogenen Berechnung fließen folgende Informationen in die Berechnung der Stundensummen ein:

* Die Angaben in der Spalte „Dauer/W“ der Veranstaltungsliste
* Der allgemeine Wochenfaktor in den Statistikeigenschaften der Datei.
* Die Informationen über die ausgenommenen Wochen in den Statistikeigenschaften der Datei.
* Die Angaben in der Spalte „Block“ der Veranstaltungsliste
* Die Angaben in der Spalte „Wochen“ der Veranstaltungsliste
* Die Angaben in der Spalte „Zeit“ der Terminzeilen in der Veranstaltungsliste

### Tagesbezogene Berechnung

Bei der tagesbezogenen Berechnung werden die Lehrer-Ist-Werte für die einzelne Unterrichtswoche ermittelt, indem die Dauer der im Teilfenster ``Planungsfenster`` definierten Unterrichtstermine miteinander addiert werden. Informationen über unterrichtsfreie Ereignisse, wie z.B. Ferien oder Feiertage werden dabei berücksichtigt. Der Jahresstundenwert des Lehrer-Ist wird errechnet, indem die Stundenwerte der einzelnen Wochen miteinander addiert werden. Der Wochendurchschnittswert des Lehrer-Ist wird gebildet, indem der Jahresstundenwert durch einen automatisch generierten Wochenfaktor dividiert wird.

Um in den Dateieigenschaften die tagesbezogene Berechnungsart der Stundensummen zu aktivieren, gehen Sie bitte folgendermaßen vor:

1. Klicken Sie im Menüband auf die Schaltfläche ``Plan``.
2. Wählen Sie im Planmenü den Befehl ``Eigenschaften``.
3. Blättern Sie im Dialogfenster ``Eigenschaften`` zur Registerkarte ``Statistik``.
4. Wählen Sie im Bereich ``Verrechnungsart`` den Eintrag ``Tagesbezogen`` aus dem Aufklappmenü des Feldes ``Summierung``.
5. Bestätigen Sie Ihre Angaben mit ``OK``. Die tagesbezogene Berechnung wird nun für die Ermittlung der Lehrer- und Klassenstunden aktiviert.

![Verrechnungsart tagesbezogen](/assets/images/Summierung.Tagesbezogen.png)

Bei der tagesbezogenen Berechnung fließen folgende Informationen in die Berechnung der Stundensummen ein:

* Anfangs- und Enddatum des Planungszeitraums
* Unterrichtsfreie Termine
* Dauer der Unterrichtstermine
* Überschneidungsinformationen im Planungsfenster
* Automatisch generierter Wochenfaktor

## Auswertungen

### Jahresverteilung

In der Jahresverteilung bietet eine Übersicht der Stundensummen der einzelnen Kalenderwochen aus Sicht der Lehrkräfte oder Klassen.

In der Jahresverteilung können Sie im Menü `Start > Jahresverteilung > Farben anzeigen` können Sie die einzelnen Wochenwerte farbig nach betsimmten Kriterien ausgeben. Die Einstellzung hierfür machen Sie in den `DaVinci Optionen > Farben > Jahresverteilung`. Hier können Sie Farben für die Werte 

* Planvorgabe Null
* Planvorgabe überschritten
* Planvorgabe unterschritten
* sonstige Wochen

vornehmen

In der Jahresverteilung können Sie im Menü `Start > Jahresverteilung > Listenansicht` die Ausgabe der Werte in der einzelnen Kalenderwochen auswählen:
* Soll - Sollstunden laut Stundentafel für die Klassen oder Lehrerzeitkonto für die Lehrkräfte
* Geplant
* Verplant
* Unverplant - Differenz aus Sollstunden und verplanten Stunden

#### Klassen

Spalte | Bedeutung
-|-
Kürzel| `Stammdaten > Klasse > Kürzel`
Name|`Stammdaten > Klasse > Bezeichnung`
Soll/J|Stundentafelsoll 
Geplant/J|Schülerist/J
Summe|Summe der Stunden je nach Auswahl der einzelnen Kalenderwochen
Kalenderwochen|Stundenanzahl in der Kalenderwoche je nach Auswahl

#### Lehrkräfte


Spalte | Bedeutung
-|-
Kürzel|`Stammdaten > Lehrer > Kürzel`
Name|`Stammdaten > Lehrer > Bezeichnung`
Soll/J|Sollstunden x Wochenfaktor
Geplant/J|geplante Stunden im Wochenschnitt x Wochenfaktor
Summe|Summe der Stunden je nach Auswahl der einzelnen Kalenderwochen
Kalenderwochen|Stundenanzahl in der Kalenderwoche je nach Auswahl
