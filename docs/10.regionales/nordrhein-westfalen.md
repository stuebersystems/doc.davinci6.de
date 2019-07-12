# Landestatistik Nordrhein-Westfalen

DAVINCI exportiert die Daten für die Nordrhein-Westfälische Landesstatistik.

**So gehen Sie vor:**

Exportieren Sie mit ``Plan > Importieren und Exportieren > Statistikdaten exportieren`` und dann mit ``Statistik Nordrhein-Westfalen ABS (Extern.dat)  exportieren`` oder ``Statistik Nordrhein-Westfalen BBS (Extern.dat)  exportieren`` die entsprechenden Daten.

## Was wird exportiert

Exportiert werden CSV-Dateien mit folgenden Feldern:

### Exportformat für die Statistik NRW ABS EXTERN.DAT

## Notwendige Angaben für die ABS-Statistik

Die folgenden Angaben müssen in DAVINCI bei allgemeinbildenden Schulen gemäß der offiziellen Statistikvorgaben gemacht werden. Bitte beachten Sie unbedingt die maximal zulässige Länge für Klassen-, Lehrer- und Fachkürzel.

Angabe gemäß Statistik | Angabe in DAVINCI
------------|-------------------
Klassenkürzel|Klassenkürzel im Stammdatenfenster auf Registerkarte „Klassen“, maximal 4stellig
Gruppe | wird in DAVINCI nicht erfasst
Fachkürzel|Spalte "Kürzel" im Stammdatenfenster auf Registerkarte „Fächer“, maximal 4stellig
Wochenstunden|Spalte „Dauer/W“ in der Unterrichtsliste des Planungsfenster
Lehrerkürzel|Lehrerkürzel im Stammdatenfenster auf Registerkarte „Lehrer“
Schülerzahl insgesamt|Spalte „Schüler“ in der Unterrichtsliste des Planungsfensters
Schülerzahl weiblich|wird derzeit nicht unterstützt
Schülerzahl Fremde|wird derzeit nicht unterstützt

Die folgenden Angaben müssen in DAVINCI bei allgemeinbildenden Schulen gemäß der offiziellen Statistikvorgaben gemacht werden. Bitte beachten Sie unbedingt die maximal zulässige Länge für Klassen-, Lehrer- und Fachkürzel.

Feld        | Stellen | Positionen | Beschreibung
------------|-------------------
Klasse|        4-stellig |Pos. 1- 4 |Klassenkürzel
Gruppe|        2-stellig |Pos. 5- 6 |Art der Gruppe
Wstd|       2-stellig |Pos. 7- 8 |Erteilte Wochenstunden
Fach |4-stellig |Pos. 9-12 |Fach
Lehrer|        4-stellig |Pos. 13-16 |Lehrerkürzel
Schueler |        2-stellig |Pos. 17-18 |Schüler insgesamt
darunter weiblich|2-stellig |Pos. 19-20 |Schülerinnen im Unterricht
Fremde|        1-stellig |Pos. 21 | Merkmal für Schüler anderer Schulen
Bildungsgang |       3-stellig | Pos. 22-24 |
Produktname |    20-stellig | Pos. 25-44  | Produktname
Produktversion |   20-stellig | Pos. 45-64  | DAVINCI Produktversion

### Exportformat für die Statistik NRW BBS EXTERN.DAT

## Notwendige Angaben für die BBS-Statistik

Die folgenden Angaben müssen in DAVINCI bei Berufskollegs gemäß der offiziellen Statistikvorgaben gemacht werden. Bitte beachten Sie unbedingt die maximal zulässige Länge für Klassen-, Lehrer- und Fachkürzel.

Angabe gemäß Statistik|Angabe in DAVINCI
------------|-------------------
Klassenkürzel|Klassenkürzel im Stammdatenfenster auf Registerkarte „Klassen“, maximal 6stellig
Teilklassenmerkmal|wird in DAVINCI nicht erfasst
Gruppe|wird in DAVINCI nicht erfasst
Fachkürzel|Spalte „Kürzel“ im Stammdatenfenster auf Registerkarte „Fächer“, maximal 4stellig
Wochenstunden|Spalte „Dauer/W“ in der Unterrichtsliste des Planungsfenster
Lehrerkürzel|Lehrerkürzel im Stammdatenfenster auf Registerkarte „Lehrer“
Schülerzahl insgesamt|Spalte „Schüler“ in der Unterrichtsliste des Planungsfensters

Feld        | Stellen | Positionen | Beschreibung
------------|-------------------
Klasse      | 6-stellig |Pos. 1 - 6 |Klassenkürzel
TKM    | 1-stellig |Pos. 7 |  Teilklassenmerkmal
Gruppe      | 2-stellig |Pos. 8 - 9 |Art der Gruppe
Wstd   |  2-stellig | Pos. 10-11 |  Erteilte Wochenstunden
Fach    | 4-stellig |Pos. 12-15 |  Fach
Lehrer      | 4-stellig |Pos. 16-19 |  Lehrerkürzel
Schueler    |  2-stellig |Pos. 20-21 |  Schüler insgesamt
Dummy     | 6-stellig |Pos. 22-27 |  z.Z. leer
Produktname   |  20-stellig |  Pos. 28-47  |      DAVINCI 
Produktversion | 20-stellig |  Pos. 48-67  |     DAVINCI Produktversion

### Exportformate für die Statistik NRW GPC (Gesundheitsstatistik per PC)

## Lehrerdaten

Nr |Feld        | Stellen | Leer | Beschreibung
------------|-------------------
 1 | Lehrerkürzel |      Text(255) | nein  |  Eindeutiges Kürzel der Lehrkraft
 2 | Nachname |              Text(255)  |     nein  |  Nachname der Lehrkraft
 3 | Vorname  |             Text(255)  |     nein  |  Vorname der Lehrkraft
 4 | Geburtsdatum | Datum  |    nein  |  Geburtsdatum der Lehrkraft (Format:TT.MM.JJJJ)
5 | Geschlecht   |         Integer  |       ja   |   3 = männlich / 4 = weiblich
6 | Rechtsverhältnis |  Text(1)    |     ja   |   Abkürzungsmerkmal für das Rechtsverhältnis (siehe nachfolgende Aufstellung)
7 | Personalaktennummer |  Text(255) |       ja  |     Personalaktennummer der Lehrkraft bei der personalaktenführenden Stelle

## Unterricht

Nr |Feld        | Stellen | Leer | Beschreibung
------------|-------------------
  1 | Lehrkraftkürzel |    Textt(255) |     nein |   Eindeutiges Kürzel der Lehrkraft
  2 | Beginndatum    |     Datum     |      nein  |  Datum des Beginns des Unterrichtszeitraums (Format: TT.MM.JJJJ)
  3 | Endedatum      |     Datum      |     nein  |  Datum des Endes des Unterrichtszeitraums (Format: TT.MM.JJJJ)
  4 | Mo            |      Text(1)    |    ja  |    Hat am Montag Unterricht. Jedes Zeichen außer einer Leereingabe wird als Unterricht an dem Tag gewertet.
  5 | Di            |      Text(1)     |   ja   |   Hat am Dienstag Unterricht. Jedes Zeichen außer einer Leereingabe wird als Unterricht an dem Tag gewertet.
  6 | Mi            |       Text(1)   |     ja   |   Hat am Mittwoch Unterricht. Jedes Zeichen außer einer Leereingabe wird als Unterricht an dem Tag gewertet.
  7 | Do           |       Text(1)   |     ja    |  Hat am Donnerstag Unterricht. Jedes Zeichen außer einer Leereingabe wird als Unterricht an dem Tag gewertet.
  8 | Fr            |      Text(1)  |     ja    |  Hat am Freitag Unterricht. Jedes Zeichen außer einer Leereingabe wird als Unterricht an dem Tag gewertet.
  9 | Sa             |     Text(1)  |      ja   |   Hat am Samstag Unterricht. Jedes Zeichen außer einer Leereingabe wird als Unterricht an dem Tag gewertet.

## Krankheit

Nr |Feld        | Stellen | Leer | Beschreibung
------------|-------------------
  1 | Lehrkraftkürzel  |   Text(255) |     nein  |  Eindeutiges Kürzel der Lehrkraft
  2 | Beginndatum  |       Datum      |     nein |   Datum des Beginns der Krankheit (Format:TT.MM.JJJJ)
  3 | Endedatum      |     Datum      |     nein |   Datum des Endes der Krankheit (Format: TT.MM.JJJJ)
  4 | Krankheitskürzel  |   Text(255)  |    ja  |    Abkürzungsmerkmal für die Art der Krankheit

## Ferien

Nr |Feld        | Stellen | Leer | Beschreibung
------------|-------------------
  1| Beginndatum |  Datum    | nein |   Datum des Beginns des Ferienzeitraums (TT.MM.JJJJ)
  2 | Endedatum |    Datum |  nein  | Datum des Endes des Ferienzeitraums (TT.MM.JJJJ)
  3 | Ferienkürzel   |     Integer   | nein  |  Schlüsselwerte: 1 = Ferien; 2 = Feiertag; 3 = Bewegliche Ferientage
  4 | Bemerkung     |      Text(255)  |  ja  |    Erläuterungen zur Ferienzeit. z.B.: Osterferien

## Krankentage

Beispiel:

```
Merkmal; Lehrkräftezusammen; Nettotage; Krankentage_Tage; Krankentage_Quote;Krankentage_Lehrkräfte; Krankentage_1bis3_Tage;
Krankentage_1bis3_Quote; Krankentage_1bis3_Lehrkräfte; Krankentage_4-bis30_Tage; Krankentage_4bis30_Quote; Krankentage_4bis30_Lehrkräfte;
 Krankentage_über30_Tage; Krankentage_über30_Quote; Krankentage_über30_Lehrkräfte;

```

```
 Lehrkräfte insg.;8;767;73;9,5;8;1;0,1;1;36;4,7;4;36;4,7;1
 Nur Lehrerinnen;2;130;0;0,0;2;0;0,0;0;0;0,0;0;0;0,0;0
 Nur Lehrer;6;637;73;11,5;6;1;0,2;1;36;5,7;4;36;5,7;1
 Nur verbeamtete Lehrkräfte;5;505;66;13,1;5;0;0,0;0;30;5,9;3;36;7,1;1
 Nur tarifbeschäftigte Lehrkräfte;3;262;7;2,7;3;1;0,4;1;6;2,3;1;0;0,0;0
 Lehrkräfte unter 36 Jahre;2;175;6;3,4;2;0;0,0;0;6;3,4;1;0;0,0;0
 Lehrkräfte zwischen 36 und 45;1;65;0;0,0;1;0;0,0;0;0;0,0;0;0;0,0;0
 Lehrkräfte zwischen 46 und 55;2;220;25;11,4;2;0;0,0;0;25;11,4;2;0;0,0;0
 Lehrkräfte über 55 Jahre;3;307;42;13,7;3;1;0,3;1;5;1,6;1;36;11,7;1

}

```
