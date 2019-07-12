# Landestatistik Niedersachsen

DAVINCI exportiert die Daten für die Niedersächsische Landesstatistik. 

**So gehen Sie vor:**

Exportieren Sie mit ``Plan > Importieren und Exportieren > Statistikdaten exportieren`` und dann mit ``Statistik Niedersachsen exportieren`` die entsprechenden Daten.

## Was wird exportiert

Exportiert wird eine Datei mit festen Feldlängen mit folgenden Feldern:

## Aufbau der von DAVINCI exportierten BBS-Planung Datei

Von Stelle | Bis Stelle | Beschreibung
-------|--------|-------------------
1    |   5   |    Schulnummer
6    |   15  |    Name der Klasse / der Gruppe / des Kurses
16   |   18  |    Lfd. Nummer der Klasse/ der Gruppe / des Kurses
19   |   20  |    Organisationsform des Unterrichts
21   |   22  |    Statistische Bezeichnung des Unterrichtsfachs
23   |   28  |    Soll-Unterrichtsstunden der Schülerinnen und Schüler
29   |   34  |    Ist-Unterrichtsstunden der Schülerinnen und Schüler
35   |   40  |    Lehrkräfteunterrichts - Sollstunden
41   |   46  |    Lehrkräfteunterrichts - Iststunden
47   |   51  |    Lehrerkürzel
52   |   53  |    Qualifizierung der Unterrichtsstunde
