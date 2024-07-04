# Übersicht "Ausfallstatistik"

[1]:/assets/images/analytics/ausfallstatistik01.png
[2]:/assets/images/analytics/schulformen.png
[3]:/assets/images/analytics/analytics.lehrerfehlgruende.png
[4]:/assets/images/analytics/klassenfehlgruende.png
[5]:/assets/images/analytics/ausfallstatistik02.png
[6]:/assets/images/analytics/ausfallstatistik03.png
[7]:/assets/images/analytics/ausfallstatistik04.png

Die Ausfallstatistik liefert den Unterrichtsausfall nach Fächern oder nach Schulformen entweder aus Schüler- oder aus Lehrersicht. Dazu werden die Vertretungsstunden gemäß ihrer Qualifizierung durch Lehrer/Klassen-Fehlgründe und durch Vertretungsentfallgründe aufsummiert.

!!! info "Hinweis"

    Bei dieser Statistik werden nur Stunden erfasst, die Statistik relevant sind. Sie können Klassen (siehe `Stammdaten > Klassen > Details`), Lehrer (siehe `Stammdaten > Lehrer > Details`), Fächer (siehe `Stammdaten > Fächer > Details`) und Zusatzunterricht (im Eingabe Dialog) als `Nicht Statistik relevant` vermerken.

[![Ausfallstatistik][1]][1]

## Die Sichtweisen

| Sichtweise | Beschreibung |
| --- | --- |
| Nach Schülern | Schüler orientiert: Erfasst nur außerplanmäßigen Unterrichtsausfall, d.h. Ausfälle die nicht mit gleichem Fach vertreten wurden oder die entfallen sind |
| Nach Lehrern | Lehrer orientiert: Erfasst jeden Unterrichtsausfall unabhängig davon ob er vertreten wurde oder entfällt |

!!! info "Hinweis"

    Bitte beachten Sie folgenden Spezialfall: Bei der Sichtweise `Nach Schülern` wird der Unterricht in geblockten Veranstaltungen aufgrund der Schüleranzahl in der betreffenden Gruppe (siehe Dialog `Veranstaltungsdetails > Schüleranzahl` oder `Veranstaltungsliste > Schüler`) anteilig an der Gesamtschülerzahl in der Klasse (siehe `Stammdaten > Klassen > Schüler`) errechnet (fehlt diese Schülerzahl, ist also der Wert Null, dann wird keine anteilige Berechnung durchgeführt), z.B:

```txt

Beispiel für geblockten Unterricht aus Schüler Sicht:

Block (gleichzeitig stattfindender Unterricht) bestehend aus:
1 Stunde BWL Kurs/Gruppe "1" in Klasse "A"
1 Stunde BWL Kurs/Gruppe "2" in Klasse "A"

24 Schüler in Klasse "A"
12 Schüler in BWL Kurs/Gruppe "1"  
12 Schüler in BWL Kurs/Gruppe "2"  

Von der Vertretung betroffen sei nur BWL Kurs/Gruppe "1".
Der statistische Stundenwert aus Schüler-Sicht ergibt sich damit:
Stundenwert = 1 Stunde * 12/24 = 0,5

```

## Die Gruppierung

| Gruppiert | Beschreibung |
| --- | --- |
| Nach Fächern | Diese Ansicht gruppiert die Summen nach Fächern. Dazu müssen Sie unter `Stammdaten > Fächer` die entsprechenden Fächer eingeben. Es erscheinen alle dort angegebenen Fächer mit einer Angabe in der Spalte "Schlüssel". |
| Nach Schulform | Diese Ansicht gruppiert die Summen nach Schulformen. Sie müssen dazu jeder Klasse unter `Stammdaten > Klassen > Schulform` eine Schulform zugeordnet haben. Dazu müssen Sie unter `Extras > Schlüsselverzeichnisse > Schulformen im Schlüsselverzeichnis `Schulformen` die entsprechenden Schulformen eingeben. Es erscheinen alle dort angegebenen Schulformen mit einer Angabe unter "Schlüssel" als Zeilen. |
| Nach Schulform | Diese Ansicht gruppiert die Summen nach Schulformen. Sie müssen dazu jeder Klasse unter `Stammdaten > Klassen > Schulform` eine Schulform zugeordnet haben. Dazu müssen Sie unter `Extras > Schlüsselverzeichnisse > Schulformen` die entsprechenden Schulformen eingeben. Es erscheinen alle dort angegebenen Schulformen mit einer Angabe unter "Schlüssel" als Zeilen.|

[![Schlüsselverzeichnis Schulformen][2]][2]

## Die Spalten

Die Übersicht errechnet sich dynamisch aufgrund der von Ihnen dafür gekennzeichneten Lehrerfehlgründe, Klassenfehlgründe und Vertretungsentfallgründe. Dabei geht DaVinci nach folgender Regel vor: Es erscheinen diejenigen Kürzel als Spalten in der Tabelle, die einen Schlüsselwert in der Spalte "Schlüssel" des jeweiligen Schlüsselverzeichnisses haben. Zusätzlich wird das erste Kürzel als Spalte aufgeführt, dass keinen Eintrag in der Spalte "Schlüssel" hat. Es dient dazu, alle weiteren Gründe zu sammeln, solange diese ebenfalls keine Angabe im Feld "Schlüssel" haben.

[![Schlüsselverzeichnis > Lehrerfehlgründe][3]][3]

[![Schlüsselverzeichnis > Klassenfehlgründe][4]][4]

[![Übersichten > Ausfallstatistik][5]][5]

| Spalte | Beschreibung |
| --- | --- |
| Verplant | Stundensumme gemäß Plan als Sollvorgabe |
| Ausfall | Summe der ausgefallene Stunden, bei denen ein Vertretungsentfallgrund angegeben wurde |
| Planm. Ausfall | Planmäßiger Ausfall, d.h. die Stunden die von Vertretungen laut Plan betroffen sind, unabhängig davon ob sie vertreten wurden oder entfallen sind |

[![Übersichten > Ausfallstatistik][6]][6]

| Spalte | Beschreibung |
| --- | --- |
| Außerplanmäßiger Unterrichtsausfall wegen | Unterrichtsausfall, weil ein anderes Fach vertreten wurde oder die Stunde entfallen ist |
| Unterrichtsausfall wegen | Geplanter Unterricht fällt aus, aufgeschlüsselt nach Fehlgründen (Lehrer- und Klassenfehlgründen) |

[![Übersichten > Ausfallstatistik][7]][7]

| Spalte | Beschreibung |
| --- | --- |
| Vertretungen im gleichen Fach | Summe der Vertretungen im gleichen Fach |
| Vertretungen in anderem Fach | Summe der Vertretungen in anderem Fach als Gesamtsumme (Spalte "Gesamt") und aufgeschlüsselt nach Entfallgründen |

## Ergebnis exportieren

Über `Start > Exportieren` können Sie die Daten als für die Ausfallstatistik Sachsen exportieren. Diese können Sie als XML-Datei, Excel-, HTML- oder Textdatei speichern.

!!! info "Hinweis"

     Wie Sie mit der Ausfallstatistik die sächsische Landesstatistik erstellen können, erfahren Sie im DaVinci Benutzerhandbuch unter Regionales im Abschnitt [Sachsen](https://doc.davinci6.stueber.de/10.regionales/sac-ausfallstatistik).
