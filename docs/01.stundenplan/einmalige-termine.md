# Einmalige Termine

!!! warning "Wichtig"

     Zum Verplanen von einmaligen Termine benötigen Sie eine Lizenz für DaVinci JAHRESTERMINE.

Die meisten Schulen arbeiten In der Regel mit wöchentlichen Termine also z.B. "5 Stunden Deutsch", d.h. fünf Termine verteilt über die Woche mit Wiederholung in jeder Schulwoche. Sollte jede Woche ein anderer Stundenplan erforderlich sein, was bei berufblidenden Schulen der Fall sein kann, ist es möglicherweise sinnvoller mit einmaligen Terminen zu arbeiten. In diesem Fall wären es z.B. "44 Stunden BWL", die über alle Schuljahreswochen auf verschiedene Tage und Uhrzeiten verteilt werden sollen. DaVinci unterscheidet dazu die Art einer Veranstaltung in "wöchentlich" oder "einmalig". Sollten Sie jede Woche oder nach einem Abschnitt aus mehreren Wochen einen anderen Stundenplan planen müssen, bieten einmalige Termine viele Vorteile.

## Einmalige vs. periodische Termine

DaVinci erlaubt es Ihnen mit periodischen Terminen oder mit einmaligen Terminen zu planen.

**Periodische Termine** Die Veranstaltung hat im Veranstaltungsfenster bei ``Zeitvorgaben > Wiederholung`` den Wert "periodisch". Dies ist der Standardfall für Allgemeinbildende und viele Berufsbildende Schulen. Die "Dauer", die Sie für eine Versnstaltung eingeben, ist die Stundendauer je Woche. In der Regel sind das alle Unterrichtswochen des Schuljahres bzw. bestimmte Wochen des Schuljahres (periodischer Unterricht). Zwei Stunden BWL für eine periodische Veranstaltung ergeben z.B. zwei einstündige Termine je Woche, die in jeder Unterichtswoche wiederholt werden..

**Einmalige Termine** Die Veranstaltung hat im Veranstaltungsfenster bei ``Zeitvorgaben > Wiederholung`` den Wert "einmalig". In diesem Fall wird die Angabe in der Spalte "Dauer" der Veranstaltungsliste von DaVinci als absolute Stundenangabe interpretiert, d.h. die Termine dieser Veranstaltung finden nur einmal zu einem bestimmten Termin statt. Zwei Stunden BWL für eine einmalige Veranstaltung ergeben z.b. zwei einstündige Termine irgendwo im Schuljahr.

## Soll ich mit periodischen oder einmaligen Terminen arbeiten

Das hängt davon ab, wie oft Ihr Stundenplan über das Schuljahr sich verändert und in welchem Umfang diese Veränderungen haben. Generell hat sich folgende Regel als nützlich erwiesen:

* Wenn sich Ihr Stundenplan nur in Teilen, also nur für einige bestimmte Klassen verändert, sollten Sie mit periodischen Terminen arbeiten und die Änderungen in diesen Klassen über Zeiträume abbilden.

* Wenn sich Ihr Stundenplan sich häufig verändert, im Extremfall alle paar Wochen, dan sollten Sie mit einmaligen Terminen arbeiten.

Für die Statistik bedeutet das:

Bei periodischen Terminen können Sie die Stundensummen als Wochenmittelwerte oder als Jahressummen in DaVinci ermitteln lassen. Bei einmaligen Terminen machen Wochenmittelwerte keinen Sinn, hier müssen Sie die Summen als Jahressummen in DaVinci ermitteln. Solange Sie mit periodischen und einmaligen Terminen in Ihrem Plan arbeiten, sollten Sie zwecks Vergleichbarkeit der Zahlen mit Jahressummen arbeiten.

## Mit einmalige Termine arbeiten

DaVinci hat spezielle Funktionen für das Planen einmaliger Termine, die wir im folgenden näher betrachten wollen.

### Einmalige Termine in der Stundentafel

Bei Stundentafel können Sie in der Spalte **Wiederholung** den Wert "einmalig" einstellen. Die Stundenangaben werden dann als Jahressummen interpretiert. Sie müssen dann also 80 Stunden BWL angeben, wenn 2 Stunden je Woche in 40 Unterrichtswochen unterrichtet werden sollen.
![Einmalige Termine in der Stundentafel](/assets/images/stundenplan/sp01.png)

### Einmalige Termine in der Veranstaltungsliste

Einmalige Veranstaltungen werden wie periodische Veranstaltungen in der Veranstaltungsliste geführt. Wichtige Splaten zur Planung sind hier die Spalten Soll/J und Ist/J

![Einmalige Termine in der Veranstaltungsliste](/assets/images/stundenplan/sp02.png)

Spalte | Bedeutung
-|-
Soll/J|Eintrag aus der Spalte **Soll** in der Stundentafel (wenn das Fach neu angelegt wird und nicht in der Stundentafel ist, ist der Wert hier 0)
Ist/J|bereits gesetzte Veransatltungen
Dauer| wird mit dem Soll/J aus der Stundentafel vorbelegt
Unverplant| noch zu setzende Stunden

Unter ``DaVinci Optionen > Einstellungen > Veranstaltungsliste`` bei **Wiederholung** einmalig voreinstellen. Wenn Sie nun in der Veranstltungliste eine neue Veranstaltung anlegen, wird diese als einmalig angelegt.

![Einmalige Termine in der Veranstaltungsliste](/assets/images/stundenplan/sp03.png)

### Einmalige Termine im Stundenplan

Einmalige Termine werden im Stundenplan analog mit einem Punkt rechts oben in der Terminzelle gekennzeichnet.

![Einmalige Termine im Stundenplan](/assets/images/stundenplan/sp04.png)

Bitte achten Sie darauf, dass einmalige Termine nur in einer bestimmten Woche, also niemals in der Ansicht "Alle Wochen", verplant werden können, da diese Termine zwingend ein bestimmtes Datum haben müssen. Bei einmaligen Termine sollten Sie im Planfenster mit der ``Start > Einstellung > Kollisionen`` und dem Wert **zulassen, nichts anzeigen** arbeiten, dann haben nämlich die folgenden Befehle den Effekt, dass sie sich auch auf die nachfolgenden Termine in den Folgewochen beziehen, wenn Sie dies in den entsprechenden Dialogfenstern so bestätigen:
![Einstellungen](/assets/images/stundenplan/sp05.png)

* Beim Verschieben eines Termins mit Drag & Drop
* Beim Entfernen eines Termins aus dem Plan mit ``Termine(e) aus Plan entfernen``
* Beim Löschen eines Termins mit ``Löschen``

Sie können einmalige Termine aus dem Veranstaltungsfenster in der Ansicht "Veranstaltungen" aus der `Veranstltungsliste` oder aus dem `Zusatzfenster > Unverplant` per Drag & Drop in den Plan ziehen.

Wenn Sie sehen möchten wie Ihre einmaligen Termine über das Schuljahr verplant sind, wechseln Sie im Stundenplanfenster einfach in die Ansicht "Jahresplan" (z.B. über rechte Maustaste). In dieser Ansicht können Sie ebenfalls die Termine per SDrag & Drop aus der Veranstlatunsliste verplanen.

### Mit Null Terminen beginnend hochzählen

Beim Kopieren der Stundentafel in die Veranstaltungsliste können Sie optional die Dauer als Nullwert übernehmen, d.h. die Veranstaltungen werden eingerichtet, haben aber keine Termine.

Im Stundenplanfenster sind somit vorerst nur Veranstaltungen aber keine Termine vorhanden. Wenn sie nun eine Veranstaltung per Drag & Drop in den Plan ziehen, wird automatisch ein neuer Termin angelegt. Auf diese Weise können Sie jeweils einen neuen Termin verplanen, bis die gewünschte Sollstundenanzahl erreicht ist.

### Termine gemäß Stundentafel hinzufügen

Wenn Sie beim Kopieren der Stundentafel in die Veranstaltungsliste  die Dauer übernehmen, werden die Veranstaltungen mit der entsprechenden Terminanzahl eingerichtet. Diese können sie dann manuell oder per Automatik auf die Wochen verplanen.
