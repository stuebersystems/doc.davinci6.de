# Änderungen verfolgen und bearbeiten

Durch Fehlzeiten entstehen für betroffene Termine Änderungselemente, welche die Grundlage für Vertretungen sind. Zu diesen Änderungen zählen auch Zusatzunterricht, Fehlstellen und Raumbuchungen und weitere Änderungen am regulären Plan. Alle Änderungen, die Sie in den verschiedenen Ansichten eingeben, werden in der Änderungsliste chronologisch aufgelistet. Gehen Sie dazu in die Ansicht `Vertretungsplan > Änderungen`. Sie können dort auch gelöscht bzw. teilweise geändert werden. Wenn Sie mit dem DAVINCI ENTERPRISE Server arbeiten, können Sie in den Spalten `Geändert Zeit` und `Geändert von` erkennen, wer wann die letzte Modifikation am jeweiligen Änderungselement durchgeführt hat.

![Dies ist die Ansicht „Änderungen“](/assets/images/vertretungsplan/sub-plan88.png)

## Änderungen nachvollziehen

Die zentrale Änderungsliste ist in drei grundlegende Bereiche geteilt, die jeweils mehrere Spalten umfassen:

* **Zeitpunkt der Änderung:** Dieser Spaltenbereich umfasst alle Informationen, die den Zeitpunkt eines geänderten Termins betreffen, insbesondere Datum, Wochentag, Stundenplanposition und Uhrzeit.Darüber hinaus erhalten Sie hier Informationen über den Typ der Terminänderung sowie Hinweise auf Widersprüche.

* **Betroffener Termin und seine Änderung:** Dieser Spaltenbereich gibt Auskunft über die zentralen Elemente des geänderten Termins, insbesondere Block, Lehrer, Fach, Raum und Klasse sowie die damit verbunden Änderungen bei Klasse, Lehrer, Fach bzw. Raum.

* **Zusätzliche Informationen zur Änderung:** Dieser Spaltenbereich dokumentiert zusätzliche Informationselemente zur Änderungen, die der Vertretungsplaner im Zusammenhang mit einer Terminänderung hinterlegen kann, z.B. Infotexte, Mitteilungen und Bemerkungen.

!!! info "Hinweis"

    Sie können darüber hinaus die Änderungsliste nach einzelnen Spalten gruppieren, Spalten ein-/ausblenden und nach verschiedenen Kriterien filtern, so dass Sie den angezeigten Ausschnitt der eingetragenen Änderungen sehr flexibel an Ihre konkreten Erfordernisse anpassen können. Wie Sie die Listenfunktionen des Filterns und Gruppierens nutzen können, entnehmen Sie bitte dem Kapitel „Arbeiten in Listen“ des Benutzerhandbuchs zu daVinci-Stundenplan (siehe Abschnitt „Weitere Informationen“).

## Inhalt der Änderungsliste

Spalten | Bedeutung
-|-
Änderungsgrund|Änderungsgrund
Anrechnen| Hier werden die die Änderung betreffenden Anrechenstunden gezeigt.
Art| Zeigt an ob es sich um <br> • eine zu erstellende Lehrer-  <br>• ein Raum- <br>• eine Aufsichtsänderung  <br>• eine Fehlstelle <br> • Mitteilung <br> • Zusatzunterricht oder <br>• freigestellten Unterricht handelt
Bemerkung|bei der Vertretungserstellung eingetragene Bemerkung
Block| Hier wird im Fall von geblocktem Unterricht die Blocknummer des Termins aufgeführt.
Datum | Dies ist das Datum der Fehlzeit/Vertretung, Änderung, Zusatzunterricht, Mitteilung.
Fach|Zeigt das Fach und ggf. das Vertretungsfach an
Fehlgrund | bei der fehlerzeit erfasster Lehrer,- Klassen-, Raumfehlgrund siehe `Extras > Schlüsselverzeichnisse > Lehrer-, Klassen-, Raumfehlgründe`
Fehlt|Zeigt den fehlenden Lehrer
Geändert Zeit|Datum der Eintragung der Änderung
Geändert von|Nutzerkennung der Eintragung der Änderung
Info|bei der Vertretungserstellung eingetragene Info
Klasse|Zeigt die Klasse, die von der Änderung betroffen ist.
Konflikt|Konfklikt der Planung
Lehrer|Zeigt den Lehrer und ggf. den Vertretungslehrer an
Lehrerart|bei der Vertretungserstellung eingetragene Lehrerart siehe `Extras > Schlüsselverzeichnisse > Lehrerarten`Kürzel
LehrerartLang|bei der Vertretungserstellung eingetragene Lehrerart siehe `Extras > Schlüsselverzeichnisse > Lehrerarten` Bezeichnung
Mitteilung|bei der Vertretungserstellung eingetragene Mitteilung
Pos|Hier wird die Position der Änderung angezeigt.
Qualität|bei der Vertretungserstellung eingetragene Lehrerart siehe `Extras > Schlüsselverzeichnisse > Vertretungsqualitäten` Kürzel
QualitätLang|bei der Vertretungserstellung eingetragene Lehrerart siehe `Extras > Schlüsselverzeichnisse > Vertretungsqualitäten` Bezeichnung
Raum|Zeigt den Raum und ggf. den Vertretungsraum an
Ressourcen|zugewiesene Ressourcen
Schulform|der Klasse zugewiesene Schulforma `Stammdaten > Klasse > Schulform` siehe `Extras > Schlüsselverzeichnisse > Schulformen`
Status|Zeigt an, ob es sich um eine offene oder erledigte Änderunghandelt.
Tag|Hier wird der Wochentag der Änderung angezeigt.
Typ|Typ der änderung (Mitteilung, Aufsichtsänderung, Raumänderung, Fehlstelle)
Vertreter|Vertretungslehrer, -raum
Zeit|Hier wird die Zeitspanne der Änderung angezeigt.

## Änderungsliste bearbeiten

In der Ansicht `Änderungen` stehen Ihnen folgende Instrumente zur Verfügung, mit denen Sie die Einträge in der Änderungsliste bearbeiten können:

* Einträge in den Spalten Bemerkung, Mitteilung und Info ändern oder hinzufügen.
* Zusatzunterricht bearbeiten oder neuen Zusatzunterricht hinzufügen.
* Mitteilungen bearbeiten oder neue Mitteilungen hinzufügen
* Raumbuchungen bearbeiten oder neue Raumbuchungen hinzufügen
* Eine oder mehrere Zeilen markieren und endgültig löschen.
* Änderungen zurücksetzen

### Bemerkungen, Mitteilungen, Infozeile einfügen

Im Spaltenbereich der zusätzlichen Informationen zur Änderung ermöglichen die Felder Bemerkung, Mitteilung und Info das Eingeben zusätzlicher Informationen zu einer bestehenden Terminänderung. Um hier einen Eintrag vorzunehmen, platzieren Sie einfach den Cursor in eines dieser Felder und wählen `Start > Änderung > Bearbeiten`.  Im Dialogfenster können Sie die entsprechenden Werte eintragen. Sie können hier Freitext eintragen oder die Vorgabewerte aus `Extras Optionen > Vertretungsplan`.
![Bemerkungen, Mitteilungen, Infozeile einfügen](/assets/images/vertretungsplan/vp01.png)

### Neuen Zusatzunterricht einfügen

Sie haben bereits die Möglichkeit kennengelernt im Bereich `Vertratzungsplan > Stundenplan > Änderungen`Zusatzunterricht in Plänen einzufügen. Die gleiche Möglichkeit steht Ihnen auch in der Ansicht `Vertrtungsplan > Änderungen` zur Verfügung.  

Um in der Ansicht „Änderungen“ neuen Zusatzunterricht einzufügen gehen Sie bitte folgendermaßen vor:

1. Klicken Sie in der Menügruppe `Start > Änderungen` auf die Schaltfläche `Neu`.  
2. Wählen Sie den Eintrag `Neuer Zusatzunterricht` aus dem Aufklappmenü.
3. Markieren Sie in den Auswahlfeldern Fach und Unterrichtsart des erscheinenden Dialogfensters jeweils das zutreffende Kürzel. Bei Bedarf können Sie unter Kurs-Nr auch eine bestimmte Kursnummer angeben.  
4. Tragen Sie in den Eingabefeldern Von und Bis, die Anfangs- und die Endzeit des Zusatzunterrichts ein. Unter Anrechnen können Sie bei Bedarf eintragen, mit welchem Wert der Zusatzunterricht als positive oder negative Anrechenstunde festgehalten werden soll.
5. Legen Sie die Teilnehmer am Zusatzunterricht aus der Liste der Klasse, Lehrer bzw. Räume fest.
6. Tragen Sie optional in den Eingabefeldern Mitteilung und Bemerkung einen Text ein. Der unter Mitteilung angegebene Text wird als Information in Ihren publizierten Plänen mit ausgegeben werden soll.  
7. Bestätigen Sie Ihre Angaben im Dialogfenster „Zusatzunterricht“ mit `Ok`.
![Zusatzunterricht einfügen](/assets/images/vertretungsplan/vp02.png)

Der eingetragene Zusatzunterricht wird nun in der Änderungsliste hinterlegt. Er wird ebenfalls im Planungsfenster der betroffenen Einzelpläne angezeigt.  
![Zusatzunterricht einfügen](/assets/images/vertretungsplan/vp03.png)

!!! info "Hinweis"
    Das Dialogfenster „Zusatzunterricht“ können Sie auch über das Kontextmenü der rechten Maustaste aufrufen. Drücken Sie dazu die rechte Maustaste und wählen Sie den Befehl `Neuer Zusatzunterricht`