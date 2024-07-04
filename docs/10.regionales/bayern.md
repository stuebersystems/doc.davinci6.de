# Abgleich mit ASV - Amtliche Schulverwaltung Bayern

DaVinci unterstützt den Datenimport aus ASV sowie den Export der Daten aus DaVinci nach ASV- Amtliche Schulverwaltung in Bayern.

DaVinci unterstützt:  

* den **Import** der Lehrer-, Klassen- und Fächerstammdaten sowie der Stundenplandaten aus ASV
* STDFACH.txt (enthält die einzelnen Schulfächer)
* STDLEHR.txt (enthält die Lehrerdaten)
* STDKLAS.txt (enthält Klassenleitung, Ausbildungsrichtung, etc.)
* STDPLAN.txt (enthält Unterrichtsverteilung mit: Klasse, Unterrichtsfach, Lehrkaft etc.)
* den **Export** der Statistikdaten nach ASV ********

## Import der Daten aus ASV

Für den Import der Daten aus ASV erzeugen Sie bitte folgende Daten aus der amtlichen Schulverwaltung:

* STDFACH.txt
* STDKLAS.txt
* STDLEHR.txt
* STDPLAN.txt

Um diese Daten nach DaVinci zu importieren, müssen Sie wie folgt vorgehen:  

1. Öffnen Sie über `Plan > Importieren und Exportieren > Bayern ASV importieren`  
2. Klicken Sie im Import-Assistenten auf ``Weiter``.  
3. Geben Sie unter Importdatei den Pfad der entsprechenden Importdatei an. Beginnen Sie zunächst nacheinander mit dem Import der Stammdaten Lehrer, Klassen und Fächern. (Reihenfolge **zuerst** STDLEHR.TXT, STDFACH.TXT, STDKLASS.TXT)  
4. Klicken Sie auf ``Fertigstellen``. Die Datensätze wurden in das Stammdatenfenster "Fächer", "Lehrer" und "Klassen" importiert.  
5. Wiederholen Sie diesen Schritt nun noch für die Stundenplandaten (STDPLAN.txt).

## Export der Daten nach ASV

Für den Export der Daten nach ASV gehen Sie wie folgt vor.

1. Öffnen Sie über `Plan > Importieren und Exportieren > Statistikdaten exportieren`, klicken Sie auf ``Weiter``.
2. Wählen Sie nun  `Statistik Bayern (ASV) exportieren` 
3. Klicken Sie im Export-Assistenten auf ``Weiter``.
4. Geben Sie nun die Datei an, in die Sie die Daten exportieren wollen und klicken Sie auf ``Weiter``.

## Beispiel für exportierte WinLD-Datei

```
"000001","5a","K","Hk","2","r5","","2","05","0100","GYM","2.0"
"000002","5a","Ev","Lo","2","r5","","2","05","0100","GYM","2.0"
```

## Aufbau der von DaVinci exportierten WinLD Datei

Feld | Beschreibung
-----------|-------------------
Kennung | fortlaufende Kennung
Klasse | Bezeichnung der Klasse z. B. 9b <br/> Bei Klassengruppe (Klassenteilen) ist dies am Unterstrich in der Bezeichnung erkennbar z. B. 10a&#95;m und 10a&#95;n
Fach | Fachkürzel
Lehrer | Lehrerkürzel
Stunden | Lehrerstunden für die Unterrichtseinheit
Koppel | eventuell Koppelbezeichnung <br/>(die DaVinci Block Bezeichnung wird in eine WinLD konforme Bezeichnung umgesetzt)
Raum | Raumkürzel
Unterrichtsart | ein Zeichen <br/> 1 Pflicht 1-4; 2 Pflicht 5-6; 3 Pflicht 7-9 bzw. 7-10 4 Pflicht 10; 5 Pflicht 11; 6 Kollegstufe; 7; 8; 9; <br/> s t v Pflicht bei BOS; <br/> w Wahlunterricht;<br/> e Ergänzungsunterr.; <br/> f bzw. g Förderunterr.; <br/> a bzw. n Arbeitsgemeinsch.; <br/> p Pluskurs;<br/> k Hausunterr.; <br/> (siehe `Stundenplan > Veranstaltungen > Fachstatus.Schlüssel`) <br/> WICHTIG: Der DaVinci-Fachstatus ist die WinLD-Unterrichtsart
Jahrgang | zwei Zeichen z. B. 06 oder 11
Schulnr | vier Zeichen (Spalte `"Stammdaten > Klassen > Schule"`)
Schultyp | drei Zeichen (GYM, RS&#95; , FOS, BOS, SBA, VS&#95; , WAL, BS&#95; , WS&#95; , BFS, BAS, FS) <br/>(wird von DaVinci nicht exportiert)
Wochenwert| Wochenwert der Unterrichtseinheit für den Lehrer als Dezimalzahl mit Punkt als Dezimalzeichen. In manchen Schularten (z.B. BS) findet nicht jede Woche derselbe Unterricht statt (z.B. Wiederholung alle 3 Wochen). Der Wochenwert gibt den Mittelwert aller Stunden je Woche über alle Unterrichtswochen wieder. <br/>Zum Beispiel: <br/>3 Stunden jede Woche 3<br/> 3 Stunden in 18 von 37 Wochen 1.45946<br/>3 Stunden in 12 von 37 Wochen 0.97297</div>
Wiederholungsfaktor | Nur für BS, BFS, FS, FAK, BFG<br> Gibt an, wie oft diese Unterrichtseinheit in einem Schuljahr wiederholt wird.
Schülerzahl | Anzahl der Schüler in dieser Unterrichtseinheit <br/>(siehe DaVinci Ansicht `Stundenplan > Stundenplan > Veranstaltungsliste > Spalte Schüler`
ZusatzStd | Abweichung von der Stundentafel, zusätzlich benötigte Lehrerwochenstunden <br/>(wird von DaVinci nicht exportiert)
ZusatzArt | Begründung für die zusätzlich benötigten Lehrerwochenstunden:<br/>T Teilung Übungsgruppen<br/> A Ausgleichsunterricht wegen Kürzung in anderem Fach<br/> B Bilingualer Unterricht (GYM, RS&#95; )<br/> I Intensivierungstunden (GYM)<br/>U Unterrichtsdifferenzierung (RS&#95;)<br/>E erweiterter Musikunterricht (VS_)<br/> F Fördermaßnahmen Deutschförderklasse (VS&#95; )<br/> G Ganztagsangebot (GYM, RS&#95; , VS&#95; , SBA, SVS, WS&#95; , WAL)<br/> P Profilstunden (GYM)<br/>P Talentklasse/Talentgruppe (RS&#95;)<br/> S sonstiger Grund <br/>(wird von DaVinci nicht exportiert)
KuerzStd | Abweichungen von der Stundentafel, gekürzte Lehrerwochenstunden <br/> (wird von DaVinci nicht exportiert)
KuerzArt | Begründung für die gekürzten Stunden:<br/> L Lehrermangel<br/> V Verwaltungsgründe<br/> G Geringe Schülerzahl<br/> K Kooperation mit anderer Schule<br/>N nicht erfolgte Teilung<br/> F Schulversuch Seminarfach (FOS, BOS)<br/> P Kürzung für Talentklasse/Talentgruppe (RS&#95;)<br/>S vorübergehende Kürzung lt. Stundentafel (RS&#95;) <br/>(wird von DaVinci nicht exportiert)

## Aufbau der von DaVinci exportierten ASV Datei:

Feld | Beschreibung
-----------|-------------------
1. | `Kennung`: fortlaufende Kennung die Unterrichtselemente werden durchnummeriert
2. | `Schulnummer`: Nummer der Schule z.B. 0199 `Stammdaten > Klasse > Schule`
3. | `Schulart`Art der Schule z.B. GY wird aktuell nicht aus DaVinci exportiert
4. | `Bezeichnung der Klasse`: z. B. 9a `Stammdaten > Klasse > Kürzel`
5. | `Kennung der Klassengruppe`: z. B. nt
6. | `Fach`: Fachbezeichner, wie er von der Schule in ASV gewählt wurde<br/> z. B. E für Englisch `Stammdaten > Fach > Kürzel`
7. | mehrere Lehrkräfte eingesetzt sind. <br/>z. B. 1 bei besonderem Unterricht bleibt dieses Feld leer
8. | `Kürzel der Lehrkraft`: z. B. Hu `Stammdaten > Lehrer > Kürzel`
9. | `Lehrerwochenstunden`: z. B. 5 `Stundenplan > Veranstaltungen > Ist/W`
10.| `Wiederholungsfaktor`: Gibt an, wie oft dieses Unterrichtselement im ausgewählten Schuljahr wiederholt wird wenn die Schule nach dem Wochenstundenprinzip arbeitet ist dieser Wert immer 0 sonst Anzahl der Wiederholungen
11. | `Unterrichtsart`: Art des Unterrichts z. B. p<br/> (siehe `Stundenplan > Veranstaltungen > Fachstatus.Schlüssel`) <br/> WICHTIG: Der DaVinci-Fachstatus ist die WinLD-Unterrichtsart
12.| `Koppel`:  Bezeichnung der Koppel, wenn ein gekoppeltes Unterrichtselement vorliegt bei ungekoppeltem Unterrichtselement leer `Stundenplan > Veranstaltungen > Block`
13. | `Kursbezeichner`: Bezeichner des Kurses
14. | `wissenschaftlich`: das Unterrichtselement wird für die Lehrkraft wissenschaftlich gewertet
15. | `Kuerzung`: Art und Umfang einer Abweichung von der Stundentafel
16. | `Art und Umfang einer Abweichung von der Stundentafel`: falls keine Abweichung vorliegt, bleibt der Eintrag leer
17. | `Bereich`: das Unterrichtselement gehört zu einem bestimmten Bereich von Unterrichtsstunden (z. B. I)
18. | `Anzahl der Schüler, die diesem Unterrichtselement zugeordnet sind`: Anzahl der zugeordneten Schüler;
19. | `Unterrichtsstunden`: Beim Export bleibt das Feld leer Beim Import: UNTERRICHTSELEMENT.BEMERKUNG = Unterrichtsstunden
