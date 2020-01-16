# DAVINCI ANALYTICS

## Allgemein

Über das Modul DAVINCI ANALYTICS können Sie Ihren Gesamtjahresplan,
bestehend aus aufeinanderfolgenden Planversionen, statistisch auswerten. So können Sie mit diesem Modul z.B. die Summe der Unterrichtsstunden,den Unterrichtsausfall und die Lehrer-Fehlstunden dateiübergreifend aber für einen Planungszeitraum berechnen.
Wenn Sie das Modul DAVINCI ANALYTICS lizenziert haben, finden Sie in DAVINCI im Bereich „Übersichten“ folgende Ansichten:

* Änderungen
* Unterricht
* Unterrichtsstatistik
* Lehrer Arbeitstage
* Lehrer Mehrarbeit
* Ausfallstatistik

![Bereich "Übersichten"](/assets/images/Analytics01.png)

Die Daten für die Analyse der Übersichten "Änderungen", "Unterricht" und "Unterrichtsstatistik werden in einer Datei mit der Endung „.sc“ (für „statistic“) abgespeichert. Die .SC-Datei wird im Ordner DaVinciStatisticFolder (siehe Dialogfenster ``Hilfe > System-Informationen``) gespeichert. Es handelt sich dabei um eine Datei im JSON-Format. In der Regel werden Sie mit jeder Planänderung eine neue Plandatei mit einem neuen Gültigkeitszeitraum erstellen. In der Statistik-Datei können beliebig viele Tage abgespeichert werden, d.h. Sie können dort die Ergebnisse aus allen Plandateien eines Schuljahres aggregieren.

## Arbeit mit mehreren Plandateien

Ergeben sich im Schuljahr weitreichende Änderungen im Stundenplanbereich erstellen Sie in der Regel eine neue DAVINCI Plandatei und pflegen hier Ihre neuen vertretungsregelungen ein. Um die Informationen aus beiden Dateien auszuwerten müssen Sie folgendes beachten:

Bitte beachten Sie folgende Einstellungen in den Dateieigenschaften `Plan > Eigenschaften > Zeitraum`  
