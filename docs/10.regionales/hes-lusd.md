# Landestatistik LUSD Hessen

DaVinci ist für den Datensynchronisation mit dem vom hessischen Kultusministerium herausgegebenen Schulverwaltungsprogramm LUSD zertifiziert.

Die Daten werden dabei in verschlüsselten XML-Dateien übertragen. Die Verschlüsselung erfolgt mit der frei im Internet verfügbaren Software „GnuPG“, die Sie installieren müssen, bevor Sie in DaVinci Daten aus LUSD importieren bzw. Daten nach LUSD exportieren können.

## Vorgehensweise

1. Installieren Sie zunächst die Verschlüsselungssoftware GnuPG. Vor einem Import bzw. Export von Daten aus LUSD bzw. nach LUSD müssen Sie die Verschlüsselungssoftware GnuPG installieren. [Hier](https://www.gnupg.org/%28de%29/download/index.html) finden Sie die Downloadseite. Die aktuellste Version zum Zeitpunkt der Erstellung dieses Dokuments ist die Version GnuPG 1.4.7, hier der direkte Link:
[ftp://ftp.gnupg.org/gcrypt/binary/gnupg-w32cli-1.4.7.exe](ftp://ftp.gnupg.org/gcrypt/binary/gnupg-w32cli-1.4.7.exe)
Führen Sie das Installationsprogramm von GnuPG mit den Standardvorgaben aus.

!!! info "Hinweis"

    Sie können nach LUSD keine in DaVinci neu angelegten Stammdaten übertragen. Neue Stammdaten müssen immer zuerst in der LUSD erfasst werden und dann über einen Datenimport in DaVinci übergeben werden.

2. Laden Sie mit `Plan > Importieren und Exportieren > Hessen LUSD importieren` die Stammdaten und die Unterrichtsverteilung aus der LUSD. Sie kann aus der LUSD in Form einer verschlüsselten XML-Datei exportiert werden.

![Import/Export-Assistent, Hessen LUSD importieren](/assets/images/regionales/reg1.png)

3. Erstellen Sie den Stundenplan in DaVinci.
4. Exportieren Sie mit `Plan > Importieren und Exportieren > Statistikdaten exportieren > Statistik Hessen (LUSD) exportieren`  die verplanten Termine wieder nach LUSD.

![Import/Export-Assistent, Statistikdaten exportieren > Statistik Hessen (LUSD) exportieren](/assets/images/regionales/reg2.png)

!!! info "Hinweis"

    Sie können in DaVinci neu eingegebene Kurse nicht nach LUSD übernehmen, weil die LUSD Synchronisation dies leider nicht vorsieht.

## Was wird synchronisiert

Es werden folgende Daten zwischen DaVinci und LUSD synchronisiert. Es handelt sich um eine echte Untermenge der Daten die in DaVinci vorhanden sind: So können in DaVinci z.B. je Termin mehrere Räume zugeordnet sein, in LUSD nur jeweils ein Raum, d.h. alle zweiten und dritten Räume werde nicht synchronisiert.

**Folgende Daten werden synchronisiert:**

## Termine

| Feld      | Beschreibung                 |
| --------- | ---------------------------- |
| Lehrer    | Lehrer                       |
| Raum      | Raum                         |
| Dauer     | Dauer des Termins in Minuten |
| Wochentag | Wochentag des Termins        |

## Veranstaltungen/Kurse

| Feld                    | Beschreibung                                                                      |
| ----------------------- | --------------------------------------------------------------------------------- |
| VeranstaltungsNr        | Veranstaltungs/Kurs Nummer, wird von LUSD zur Identifikation des Kurses verwendet |
| Fach                    | Fach des Kurses                                                                   |
| Stufe/Semester          | Stufen/Semsterbezeichnung aus LUSD                                                |
| Schulform               | siehe `Extras > Schlüsselverzeichnisse > Schulformen`                             |
| Klasse                  | Klassen des Kurses                                                                |
| Termine                 | Terminliste des Kurses                                                            |
| Unterrichtsart          | siehe `Extras > Schlüsselverzeichnisse > Unterrichtsarten`                        |
| Differenzierung         | Differenzierungsmerkmal aus LUSD                                                  |
| Unterrichtsform         | siehe `Extras > Schlüsselverzeichnisse > Unterrichtsformen`                       |
| Veranstaltungskategorie | siehe `Extras > Schlüsselverzeichnisse > Veranstaltungskategorien`                |
| Schüleranzahl           | Anzahl der Schüler                                                                |

## Schüler

| Feld     | Beschreibung          |
| -------- | --------------------- |
| Nachname | Nachname des Schülers |
| Vorname  | Vorname des Schülers  |
| Klasse   | Klasse des Schülers   |

## Schüler-Kurswahlen

| Feld             | Beschreibung                    |
| ---------------- | ------------------------------- |
| Schüler-ID       | ID des Schülers                 |
| VeranstaltungsNr | identifiziert die Veranstaltung |
| Fach             | das Fach                        |
| Unterrichtsart   | die Unterrichtsart              |
| Kursnummer       | Kurs Nummer                     |

## Klasse

| Feld          | Beschreibung   |
| ------------- | -------------- |
| Kürzel        | Klassen Kürzel |
| Bezeichnung   | Bezeichnung    |
| Schüleranzahl | Schüleranzahl  |
| Lehrer        | Lehrer         |
| Schulform     | Schulform      |
| Stufe         | Stufe          |
| Kursmodus     | Kursmodus      |

## Fächer

| Feld        | Beschreibung           |
| ----------- | ---------------------- |
| Externe ID  | ID des Faches aus LUSD |
| Kürzel      | Fachkürzel aus DaVinci |
| Schlüssel   | Schlüssel des HKM      |
| Bezeichnung | Bezeichnung            |

## Räume

| Feld        | Beschreibung           |
| ----------- | ---------------------- |
| Kürzel      | Raumkürzel aus DaVinci |
| Bezeichnung | Bezeichnung            |

## Lehrer

| Feld         | Beschreibung             |
| ------------ | ------------------------ |
| Vorname      | Lehrerkürzel aus DaVinci |
| Nachname     | Bezeichnung              |
| Anrechnungen | Summe, siehe Zeitkonto   |
| Abordnungen  | Summe, siehe Zeitkonto   |
| Sollstunden  | Summe, siehe Zeitkonto   |

## Perioden (DaVinci) /Frequenz (LUSD)

| Feld        | Beschreibung                   |
| ----------- | ------------------------------ |
| Kürzel      | Kürzel der Periode aus DaVinci |
| Bezeichnung | Bezeichnung                    |
