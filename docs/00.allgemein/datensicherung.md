# Datensicherung

## Lokaler Betrieb

### Sicherungskopie erstellen 

Um bei jedem Speichern eine Sicherungskopie Ihrer Datei zu erstellen, öffnen Sie die Programm Optionen unter  `Plan > DAVINCI-Optionen` oder `Extras > Optionen` im Reiter `Plandatei`.

Wählen Sie im unteren Drittel die Option ``Sicherungskopie (.Backup-Datei) der Datei anlegen`` wenn Sie im lokalen Betrieb (ohne den Einsatz von DAVINCI ENTERPRISE arbeiten). Nun wird bei jedem Speichern von Ihrer Datei eine Sicherungskopie angelegt, welche als Dateierweiterung das Datum und die Endung ``.BACKUP`` trägt.

Generell sollten Sie in regelmäßigen Abständen, mindestens täglich, externe Sicherungskopien Ihrer Daten erstellen. Dazu sollten Sie folgende Daten sichern:

Datei| Inhalt
 --- | ---
Ihre aktuelle .daVinci | Datei Ihr Stundenplan
daVinci.hfm | Exportformate Datei
daVinci.pfm | Druckformate Datei
daVinci.opt | Ihre persönlichen Einstellungen für Farben, Ansichten, Dialogfenster

Das Erstellen der externen Sicherungskopien sollte in die Cloud (das Internet), auf Bandlaufwerke oder auf USB-Sticks erfolgen.

!!! info "Hinweis"
    Sorgen Sie unbedingt dafür, dass mindestens einmal täglich Sicherungskopien Ihrer
    Daten auf externe Datenträger erstellt  werden. Andernfalls können Sie z.B. in Folge eines Hardwarefehlers Ihre gesamten Daten verlieren.

### Sicherungskopie wiederherstellen

Ihre Sicherungskopie enthält den Namen Ihrer ursprünglichen Datei, das aktuelle Jahr, die Nummer des Tages im Jahr und die Endung ``.BACKUP``. (z.B. Beispiel.2018-04-20-00.backup)
Um eine Sicherungskopie wieder herzustellen müssen Sie Ihre Datei im Windows-Explorer in eine ``*.daVinci`` Datei umbenennen. Löschen Sie dazu den Punkt, die Zahl und die .BACKUP-Endung.

## Mehrbenutzerbetrieb

### Sicherungskopie erstellen 

Um im Mehrbenutzerbetrieb eine Sicherungskopie Ihrer Datei zu erstellen, öffnen Sie auf dem DAVINCI Serverrechner das Server Control `Systemsteuerrung > DAVINCI SERVER > Backups`.

Wählen Sie `täglich eine Sicherungskopie anlegen, falls eine Änderung vorliegt` Nun wird wenn eine Änderung der Datei vorliget, maximal einmal täglich von Ihrer Datei eine Sicherungskopie angelegt, welche als Dateierweiterung das Datum und die Endung ``.BACKUP`` trägt. Diese befindet sich an dem unter  `Systemsteuerrung > DAVINCI SERVER > Arbeitsumgebung` definiertem Pfad. Auf dem DAVINCI-SERVERS wird hier angegeben, in welchem Verzeichnis die DAVINCI Plandateien liegen.

Generell sollten Sie in regelmäßigen Abständen, mindestens täglich, externe Sicherungskopien Ihrer Daten erstellen. Dazu sollten Sie folgende Daten sichern:

Datei| Inhalt
 --- | ---
Ihre aktuelle .daVinci | Datei Ihr Stundenplan
daVinci.hfm | Exportformate Datei
daVinci.pfm | Druckformate Datei
daVinci.opt | Ihre persönlichen Einstellungen für Farben, Ansichten, Dialogfenster

Das Erstellen der externen Sicherungskopien sollte in die Cloud (das Internet), auf Bandlaufwerke oder auf USB-Sticks erfolgen.

!!! info "Hinweis"
    Sorgen Sie unbedingt dafür, dass mindestens einmal täglich Sicherungskopien Ihrer
    Daten auf externe Datenträger erstellt  werden. Andernfalls können Sie z.B. in Folge eines Hardwarefehlers Ihre gesamten Daten verlieren.

### Sicherungskopie wiederherstellen

Ihre Sicherungskopie enthält den Namen Ihrer ursprünglichen Datei, das aktuelle Jahr, die Nummer des Tages im Jahr und die Endung ``.BACKUP``. (z.B. Beispiel.2018-04-20-00.backup)
Um eine Sicherungskopie wieder herzustellen müssen Sie Ihre Datei im Windows-Explorer in eine ``*.daVinci`` Datei umbenennen. Löschen Sie dazu den Punkt, die Zahl und die .BACKUP-Endung.

Soll die Datei für alle Nutzer wieder zur Verfügung gestellt werden, laden Sie diese bitte über den  DAVINCI Explorer hoch. Bitte laden Sie die Datei über das Modul `DAVINCI Explorer >  Plandateien` über die Schaltfläche Hochladen auf den den bestehenden Platzhalter.  

