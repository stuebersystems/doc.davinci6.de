# Datenaustausch mit MAGELLAN

Wenn Sie MAGELLAN  und DAVINCI gemeinsam einsetzen, so haben Sie den Vorteil, dass viele Daten nur einmal eingegeben werden müssen. Dadurch können Doppelerfassungen von Daten minimiert bzw. vermieden werden. Bittte beachten Sie auch folgendes:

* Von MAGELLAN können die Abteilungen, die Lehrer, die Fächer, die Fachtafeln, die Klassen und die Schüler der Oberstufe an daVinci übergeben werden.
* Von DAVINCI können die Abteilungen, die Lehrer, die Fächer, die Stundentafeln, die Kurswahlen der Schüler der Oberstufe und der Fach- bzw. Kurslehrer an Magellan übergeben werden.
* Der Datenaustausch wird grundsätzlich (egal in welche Richtung) von DAVINCI aus gestartet.
* Sie benötigen die MAGELLAN-Administrator-Kennung, da der Austausch nur mit Administrator-Rechten erfolgen kann.

**Wenn Sie Magellan und daVinci einsetzen, sollten Sie wie folgt vorgehen:**

1. Geben Sie die Klassen, Lehrer, Fächer und Schüler in MAGELLAN ein und übertragen Sie diese Daten anschließend nach DAVINCI.
2. Geben Sie die Unterrichtsverteilung in DAVINCI ein und erstellen Sie mit DAVINCI den Stundenplan.
3. Geben Sie ggf. die Schülerfachwahlen in DAVINCI ein und übertragen Sie die Kurswahlen nach MAGELLAN. Wenn Sie Schüler-Fachwahlen nach MAGELLAN übertragen wollen und Sie neue Fächer in DAVINCI eingegeben haben, die noch nicht in MAGELLAN vorhanden sind, dann müssen Sie beim Datenabgleich neben den Schülerfachwahlen auch markieren, dass die Fächer übernommen werden sollen.

**Für den Datenabgleich mit MAGELLAN gelten folgende Regeln:**

* Stammdaten (Klassen, Lehrer, Fächer usw.) werden anhand der ID (Spalte „ID“) bzw. des Kürzels (falls die ID nicht vorhanden ist) synchronisiert. Beim Austausch über das Kürzel wird die Groß- und Kleinschreibung beachtet. Neue Stammdaten werden hinzugefügt. In MAGELLAN gelöschte Stammdaten werden in DAVINCI nicht gelöscht, müssen also ggf. nachträglich in DAVINCI von Ihnen gelöscht werden.
* `Unterrichtsart` und `Fachstatus` in DAVINCI müssen die gleichen Kürzel besitzen wie in MAGELLAN.
* Schüler in DAVINCI müssen Fächer mit den gleichen zugeordneten Eigenschaften Unterrichtsart, `Fachstatus` und `Kursnummer` besitzen wie in MAGELLAN.
* Die Feldlängen in DAVINCI sind praktisch unbegrenzt, die in Magellan sind begrenzt, Z.B ist kann das Kürzel einer Fachtafel (Stundentafel) in MAGELLAN nur 8 Zeichen lang sein kann. Sind die Stundentafel-Kürzel in DAVINCI länger als 8 Zeichen, kommt es zu einer Fehlermeldung beim Datenabgleich. Daher sollten Sie darauf achten, wenn Sie die Stunden- bzw. Fachtafeln abgleichen wollen, dass die Kürzel jeweils maximal 8 Zeichen lang sind.

!!! info "Hinweis"

    Vor jedem Datenaustausch sollten Sie eine Datensicherung der MAGELLAN-Datenbank (Magellan6.fdb) und der DAVINCI-Plandatei (*.daVinci) durchführen.

Nicht alle Stammdatenfelder aus DAVINCI sind auch in MAGELLAN vorhanden und umgekehrt. Werden die vorhandenen Daten beim Austausch aktualisiert (überschrieben), können vorhandene Einträge verloren gehen, z.B. bei den Klassen der Klassenraum oder bei den Stundentafeln die Soll-Stunden. Bitte entscheiden Sie mit Bedacht, welche Daten Sie austauschen.

## Daten von MAGELLAN übernehmen

Sie können die MAGELLAN-Daten in eine leere oder eine DAVINCI-Datei, die bereits Daten enthält, übernehmen. Wenn Sie einen neuen, bisher leeren Plan, mit Daten aus MAGELLAN füllen möchten, müssen Sie in DAVINCI eine neue Plandatei anlegen. Wenn in der DAVINCI-Datei bereits Daten enthalten sind, werden die vorhandenen Stammdaten ergänzt bzw. aktualisiert (mit den Daten aus MAGELLAN überschrieben).

## So übertragen Sie Daten von MAGELLAN nach DAVINCI

1. Öffnen Sie DAVINCI und klicken Sie im Menüband des Programmfensters auf die Schaltfläche `Plan` und wählen Sie im Planmenü den Befehl `Importieren und Exportieren`: der Assistent `Import/Export-Assistent` wird geöffnet.
2. Markieren Sie auf der ersten Assistentenseite im Bereich `Importieren` den Eintrag `Von MAGELLAN importieren`. Bestätigen Sie Ihre Auswahl mit `Weiter`.
3. Geben Sie im erscheinenden Dialogfenster `MAGELLAN-Anmeldung` Benutzername und Kennwort des Administratorkontos ein und bestätigen Sie Ihre Zugangsdaten mit `OK`: der Assistent `MAGELLAN-Datenaustausch` wird geöffnet.

![Hier sehen Sie die erste Seite des Assistenten "Magellan-Datenaustausch"](/assets/images/Datenaustausch/datenaustausch2.png)

4. Bestätigen Sie auf der ersten Seite des Assistenten die Option `Daten aus MAGELLAN in eine SDTF-6.Datei schreiben` mit `Weiter`.
5. Wählen Sie auf der folgenden Assistentenseite in den Feldern `Übertrage Daten aus folgendem Mandanten` und `Übertrage Daten aus folgendem Zeitraum` den gewünschten Mandanten und Zeitraum aus dem Aufklappmenü. Bestätigen Sie Ihre Auswahl mit `Weiter`.

## Daten nach MAGELLAN übergeben