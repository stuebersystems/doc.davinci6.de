# Datenaustausch mit Magellan

Wenn Sie Magellan  und DaVinci gemeinsam einsetzen, so haben Sie den Vorteil, dass viele Daten nur einmal eingegeben werden müssen. Dadurch können Doppelerfassungen von Daten minimiert bzw. vermieden werden. Bittte beachten Sie auch folgendes:

* Von Magellan können die Abteilungen, die Lehrer, die Fächer, die Fachtafeln, die Klassen und die Schüler der Oberstufe an daVinci übergeben werden.
* Von DaVinci können die Abteilungen, die Lehrer, die Fächer, die Stundentafeln, die Kurswahlen der Schüler der Oberstufe und der Fach- bzw. Kurslehrer an Magellan übergeben werden.
* Der Datenaustausch wird grundsätzlich (egal in welche Richtung) von DaVinci aus gestartet.
* Sie benötigen die Magellan-Administrator-Kennung, da der Austausch nur mit Administrator-Rechten erfolgen kann.

**Wenn Sie Magellan und DaVinci einsetzen, sollten Sie wie folgt vorgehen:**

1. Geben Sie die Klassen, Lehrer, Fächer und Schüler in Magellan ein und übertragen Sie diese Daten anschließend nach DaVinci.
2. Geben Sie die Unterrichtsverteilung in DaVinci ein und erstellen Sie mit DaVinci den Stundenplan.
3. Geben Sie ggf. die Schülerfachwahlen in DaVinci ein und übertragen Sie die Kurswahlen nach Magellan. Wenn Sie Schüler-Fachwahlen nach Magellan übertragen wollen und Sie neue Fächer in DaVinci eingegeben haben, die noch nicht in Magellan vorhanden sind, dann müssen Sie beim Datenabgleich neben den Schülerfachwahlen auch markieren, dass die Fächer übernommen werden sollen.

**Für den Datenabgleich mit Magellan gelten folgende Regeln:**

* Stammdaten (Klassen, Lehrer, Fächer usw.) werden anhand der ID (Spalte „ID“) bzw. des Kürzels (falls die ID nicht vorhanden ist) synchronisiert. Beim Austausch über das Kürzel wird die Groß- und Kleinschreibung beachtet. Neue Stammdaten werden hinzugefügt. In Magellan gelöschte Stammdaten werden in DaVinci nicht gelöscht, müssen also ggf. nachträglich in DaVinci von Ihnen gelöscht werden.
* `Unterrichtsart` und `Fachstatus` in DaVinci müssen die gleichen Kürzel besitzen wie in Magellan.
* Schüler in DaVinci müssen Fächer mit den gleichen zugeordneten Eigenschaften `Unterrichtsart`, `Fachstatus` und `Kursnummer` besitzen wie in Magellan.
* Die Feldlängen in DaVinci sind praktisch unbegrenzt, die in Magellan sind begrenzt, Z.B ist kann das Kürzel einer Fachtafel (Stundentafel) in Magellan nur 20 Zeichen lang sein kann. Sind die Stundentafel-Kürzel in DaVinci länger als 20 Zeichen, kommt es zu einer Fehlermeldung beim Datenabgleich. Daher sollten Sie darauf achten, wenn Sie die Stunden- bzw. Fachtafeln abgleichen wollen, dass die Kürzel jeweils maximal 20 Zeichen lang sind.

!!! info "Hinweis"

    Vor jedem Datenaustausch sollten Sie eine [Datensicherung](https://doc.magellan7.stueber.de/schulverwaltung/admin/admin.datenbankverbindungen/#unterpunkt-datensicherung) der Magellan-Datenbank (MAGELLAN7.fdb) und der DaVinci-Plandatei (*.daVinci) durchführen.

Nicht alle Stammdatenfelder aus DaVinci sind auch in Magellan vorhanden und umgekehrt. Werden die vorhandenen Daten beim Austausch aktualisiert (überschrieben), können vorhandene Einträge verloren gehen, z.B. bei den Klassen der Klassenraum oder bei den Stundentafeln die Soll-Stunden. Bitte entscheiden Sie mit Bedacht, welche Daten Sie austauschen.

## Daten von Magellan übernehmen

Sie können die Magellan-Daten in eine leere oder eine DaVinci-Datei, die bereits Daten enthält, übernehmen. Wenn Sie einen neuen, bisher leeren Plan, mit Daten aus Magellan füllen möchten, müssen Sie in DaVinci eine neue Plandatei anlegen. Wenn in der DaVinci-Datei bereits Daten enthalten sind, werden die vorhandenen Stammdaten ergänzt bzw. aktualisiert (mit den Daten aus Magellan überschrieben).

### So übertragen Sie Daten von Magellan nach DaVinci

1. Öffnen Sie DaVinci und klicken Sie im Menüband des Programmfensters auf die Schaltfläche `Plan` und wählen Sie im Planmenü den Befehl `Importieren und Exportieren`: der Assistent `Import/Export-Assistent` wird geöffnet.
2. Markieren Sie auf der ersten Assistentenseite im Bereich `Importieren` den Eintrag `Von Magellan importieren`. Bestätigen Sie Ihre Auswahl mit `Weiter`.
3. Geben Sie im erscheinenden Dialogfenster `Magellan-Anmeldung` Benutzername und Kennwort des Administratorkontos ein und bestätigen Sie Ihre Zugangsdaten mit `OK`: der Assistent `Magellan-Datenaustausch` wird geöffnet.

![Hier sehen Sie die erste Seite des Assistenten "Magellan-Datenaustausch"](/assets/images/Datenaustausch/datenaustausch2.png)

4. Bestätigen Sie auf der ersten Seite des Assistenten die Option `Daten aus Magellan in eine SDTF-6.Datei schreiben` mit `Weiter`.
5. Wählen Sie auf der folgenden Assistentenseite in den Feldern `Übertrage Daten aus folgendem Mandanten` und `Übertrage Daten aus folgendem Zeitraum` den gewünschten Mandanten und Zeitraum aus dem Aufklappmenü. Bestätigen Sie Ihre Auswahl mit `Weiter`.
6. Setzen Sie auf der nächsten Assistentenseite den Haken vor den gewünschten Optionen für die Übernahme unterschiedlicher Datenbereiche nach DaVinci. Bestätigen Sie Ihre Auswahl mit `Weiter`.

![Hier wählen Sie die Daten aus, die aus Magellan übernommen werden](/assets/images/Datenaustausch/datenaustausch3.png)

7. Drücken Sie auf der nächsten Assistentenseite die Schaltfläche Starten. Die Daten werden nun entsprechend der vorgenommenen Einstellungen in die DaVinci-Datei übertragen. Den Fortschritt des Datenimports können Sie anhand der Meldungen im Dialogfenster „Datei in Schuldatentransferdatei “ erkennen.

![Magellan Export](/assets/images/Datenaustausch/datenaustausch4.png)

### Sie können folgende Daten aus Magellan übernehmen

#### Abteilungen

| Felder                      | Hinweis                                                                                                                                                                                                                                                                                                                                 |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Kürzel**, **Bezeichnung** | Der Austausch erfolgt über das Kürzel. Ist das Kürzel bereits vorhanden, wird die Abteilung aktualisiert. Ist das Kürzel nicht vorhanden wird die Abteilung hinzugefügt. |

#### Lehrer

| Felder                                                                               | Hinweis                                                                                                                                                                                                                                                                                                           |
| ------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **ID, Kürzel, Nachname, Vorname, Titel, Schulnummer, Abteilungen: Abteilung.Kürzel** | Der Austausch erfolgt über ID und Kürzel. Bei gleicher ID wird aktualisiert. Ist in DaVinci keine ID vorhanden, wird über das Kürzel ausgetauscht. Bei gleichem Kürzel wird aktualisiert. Ist das Kürzel nicht vorhanden wird hinzugefügt. Es werden nur aktive Lehrer aus Magellan beim Abgleich berücksichtigt. |

#### Fächer

| Felder                                                             | Hinweis                                                                                                                                                                                                                                             |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **ID, Kürzel, Schlüssel, Bezeichnung, Kategorie, Aufgabenbereich** | Der Austausch erfolgt über ID und Kürzel. Bei gleicher ID wird aktualisiert. Ist in daVinci keine ID vorhanden, wird über das Kürzel ausgetauscht. Bei gleichem Kürzel wird aktualisiert. Ist das Kürzel nicht vorhanden wird das Fach hinzugefügt. |

#### Fachtafeln

| Felder                                                                       | Hinweis                                                                                                                                                                                                                 |
| ---------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Kürzel, Bezeichnung, Fächer der Fachtafel: Kürzel, Unterrichtsart.Kürzel** | Der Austausch erfolgt über das Kürzel. Ist das Kürzel bereits vorhanden, wird aktualisiert. Ist das Kürzel nicht vorhanden wird die Fachtafel hinzugefügt. Fachtafeln aus Magellan entsprechen Stundentafeln in DaVinci |

#### Klassen / Jahrgänge

| Felder                                                                                                                                                                             | Hinweis                                                                                                                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **ID, Kürzel, Klassenleiter 1, Klassenleiter 2, Klassenstufe, Klassenart (Kursmodus), Anzahl der Schüler, Schulnummer, Bildungsgang.Kürzel, Schulform.Kürzel, Schulstelle.Kürzel** | Der Austausch erfolgt über ID und Kürzel. Bei gleicher ID wird aktualisiert. Ist in DaVinci keine ID vorhanden, wird über das Kürzel ausgetauscht. Bei gleichem Kürzel wird aktualisiert. Ist das Kürzel nicht vorhanden wird die Klasse/der Jahrgang hinzugefügt. |
| Die Anzahl der Schüler wird nur für Oberstufenklassen übernommen.                                                                                                                  |

## Daten nach Magellan übergeben

Wenn Sie eine leere Magellan-Datenbank mit Daten aus DaVinci füllen möchten, müssen in Magellan mindestens ein Mandant und ein Zeitraum eingerichtet sein. Zum Erzeugen einer leeren Datenbank und Anlegen von Mandant und Zeitraum lesen Sie bitte in der [Magellan Dokumentation](https://doc.magellan7.stueber.de/schulverwaltung/howto/preparation/) nach.

### So übertragen Sie Daten von DaVinci nach Magellan

1. Klicken Sie im Menüband des Programmfensters auf die Schaltfläche `Plan` und wählen Sie im Planmenü den Befehl `Importieren und Exportieren`: der Assistent `Import/Export-Assistent` wird geöffnet.
2. Markieren Sie auf der ersten Assistentenseite im Bereich `Import` den Eintrag `Nach Magellan exportieren`. Bestätigen Sie Ihre Auswahl mit `Weiter`.
3. Geben Sie im erscheinenden Dialogfenster `Magellan-Anmeldung` Benutzername und Kennwort des Administratorkontos ein und bestätigen Sie Ihre Zugangsdaten mit `OK`: der Assistent `Magellan-Datenaustausch` wird geöffnet.
4. Bestätigen Sie auf der ersten Seite des Assistenten die Option `Daten aus einer SDTF-Datei nach Magellan schreiben` mit Weiter.
5. Wählen Sie in den Feldern `Übertrage Daten in folgenden Mandanten` und `Übertrage Daten in folgendem Zeitraum` den gewünschten Mandanten und Zeitraum aus dem Aufklappmenü. Bestätigen Sie Ihre Auswahl mit `Weiter`.

![Hier wählen Sie den Mandanten und den Zeitraum aus, in den die Daten übertragen werden.](/assets/images/Datenaustausch/datenaustausch5.png)

6. Setzen Sie auf der nächsten Assistentenseite den Haken vor den gewünschten Optionen für die Übernahme unterschiedlicher Datenbereiche nach Magellan. Bestätigen Sie Ihre Auswahl mit `Weiter`.

![Hier wählen Sie die Daten aus, die nach Magellan übertragen werden](/assets/images/Datenaustausch/datenaustausch6.png)

1. Drücken Sie auf der nächsten Assistentenseite die Schaltfläche `Starten`. Die Daten werden nun entsprechend der vorgenommenen Einstellungen in die DAVIDAV-Datei übertragen. Den Fortschritt des Datenimports können Sie anhand der Meldungen im Dialogfenster „Datei in Schuldatentransferdatei “ erkennen.

### Sie können folgende Daten nach Magellan übernehmen

#### Abteilungen

| Felder                      | Hinweis   |
| --------------------------- | ---------------------------- |
| **Kürzel**, **Bezeichnung** | Der Austausch erfolgt über das Kürzel. Ist das Kürzel bereits vorhanden, wird die Abteilung aktualisiert. Ist das Kürzel nicht vorhanden wird die Abteilung hinzugefügt. |

#### Lehrer

| Felder                                      | Hinweis                                                                                                                                                                                                                                                                                              |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Kürzel, Nachname, Name, Soll-Berechnung** | Der Austausch erfolgt über ID und Kürzel. Bei gleicher ID wird aktualisiert. Ist die ID in Magellan nicht vorhanden, wird hinzugefügt. Ist in daVinci keine ID vorhanden, wird über das Kürzel ausgetauscht. Bei gleichem Kürzel wird aktualisiert. Ist das Kürzel nicht vorhanden wird hinzugefügt. |

#### Lehrer-Unterricht

| Felder                                             | Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Zugewiesener Lehrer in der Veranstaltungsliste** | Durch die Übernahme des Lehrer-Unterrichts wird pro Schüler im Register `Zeugnis > Fächer` jedem Fach, entsprechend der Unterrichtsverteilung in DaVinci, der unterrichtende Fachlehrer zugeordnet. Pro Fach kann immer nur ein Lehrer übernommen werden. Voraussetzung für die Übernahme des Lehrer-Unterrichts ist, dass in Magellan den Schülern bereits Fächer zugeordnet wurden. Auch Kurswahlen der Schüler der Oberstufe müssen bereits vorhanden sein. Außerdem müssen in DaVinci und Magellan die Kürzel der Klassen, der Fächer und der Lehrer übereinstimmen. Die Übernahme funktioniert nur, wenn neben der Option `Übernehme Lehrer-Unterricht` keine weiteren Optionen markiert sind. Bei der Übernahme des Lehrer-Unterrichts aus DaVinci werden die in der Veranstaltungsliste der Klassen zugewiesenen Lehrer übernommen. |

#### Fächer

| Felder  | Hinweis       |
| ----------------|------------------------------------------ |
| **ID**, **Kürzel**,**Schlüssel**,**Bezeichnung**,**Kategorie**, **Aufgabenbereich** | Der Austausch erfolgt über ID oder Kürzel. Hat das Fach eine ID in DaVinci, so wird ein entsprechendes Fach mit gleicher ID in Magellan gesucht. Existiert ein solches Fach in Magellan, so wird es aktualisiert, andernfalls wird das Fach in Magellan hinzugefügt. Hat das Fach keine ID in DaVinci, so wird ein entsprechendes Fach mit gleichem Kürzel in Magellan gesucht. Existiert ein solches Fach in Magellan, so wird es aktualisiert, andernfalls wird das Fach in Magellan hinzugefügt.|

#### Stundentafeln

| Felder | Hinweis |
| ------------ | ----------------------------------------------------- |
| **Kürzel, Bezeichnung, Fächer der Stundentafel: Fachkürzel,Unterrichtsart.Kürzel** | Der Austausch erfolgt über das Kürzel. Ist das Kürzel bereits vorhanden, wird aktualisiert. Ist das Kürzel nicht vorhanden wird die Stundentafel hinzugefügt. Die Fächer werden mit Kürzel und Unterrichtart hinzugefügt. |


!!! info "Hinweis"

    Der Übertrag der Schülerkurswahlen nach Magellan ist nur relevant wenn Sie das Modul DaVinci Kursplan nutzen.