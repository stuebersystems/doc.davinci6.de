# Landestatistik Bremen

DAVINCI exportiert die Daten für die Bremer Lehrer-Ausfallstatistik. Die Übersicht Ausfallstatistik zeigt das Ergebnis der Bremer Ausfallstatistik.

**So gehen Sie vor:**

1. Erstellen Sie den Vertretungplan in DAVINCI.
2. Exportieren Sie mit ``Plan > Importieren und Exportieren > Statistikdaten exportieren`` und dann mit ``Statistik Bremen exportieren`` die entsprechenden Daten.

## Was wird exportiert

Exportiert wird eine CSV-Datei (eine Zeile je Tag) mit folgenden Feldern:

## Aufbau der von DAVINCI exportierten Datei

Feld        | Beschreibung
------------|-------------------
SNR     | Schulnummer
Datum     | Tagesdatum TT.MM.JJJJ
LehrerGesamt|  Anzahl Lehrer
Krank       | Anzahl der Lehrer, die absent sind mit einem Absenzgrund mit Statistikkennzeichen K
AndereGruende | Anzahl der Lehrer, die absent sind mit einem anderen Absenzgrund  Statistikkennzeichen  ungleich K
StdGesamt | gem. Stundenplan zu erteilende Stunden
AusfallBetr | zur Vertretung anfallender Unterricht (ohne Raumvertretungen und Pausenaufsichtsvertretungen)
LVertr |  Anzahl Vertretungen durch Lehrer
BetrErziehVertr |  Anzahl Vertretungen durch Erzieher / Betreuer. Diese werden in den Lehrerstammdaten mit Statistikkennzeichen B gekennzeichnet.
MitBetr |   Anzahl Mitbetreuungen
Auftr_Selbstst| Anzahl Vertretungen mit selbständiger Arbeit (Plus-Vertretungen, Vertreter = „+“)
Ausfall | Ausfall=AusfallBetr-LVertr- BetrErziehVertr- MitBetr- Auftr_Selbstst
