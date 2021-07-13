# Schlüsselverzeichnisse

An vielen Stellen in DAVINCI begegnen Ihnen Auswahlfelder, die mit Daten aus einem bestimmten Schlüsselverzeichnis vorbelegt sind. Die Schlüsselverzeichnisse tragen ihren Namen, weil sie in der Regel Angaben beinhalten, die für die statistische Auswertung der Stundenplandaten benötigt werden.

Alle diese Verzeichnisse enthalten eine Spalte `Schlüssel`, deren Felder mit den Schlüsselwerten versehen werden können, die die Landesstatistikämter für die jährlichen Schulstatistiken herausgeben. Derzeit stehen in DAVINCI verschiedene Schlüsselverzeichnisse zur Verfügung. Die meisten dieser Schlüsselverzeichnisse sind leer und können von den Schulen je nach dem schulform- und landesspezifischen Bedarf gefüllt werden. Einige Schlüsselverzeichnisse, die häufig benötigt werden und besonders typische Einträge aufweisen, sind bereits mit Standard-oder Beispielwerten versehen. Dies betrifft z.B. das Schlüsselverzeichnis `Unterrichtsarten`, dessen Einträge u. a. der Unterscheidung zwischen Leistungskursen, Grundkursen und anderen Kursen dienen. Die Schlüsselverzeichnisse, die bereits mit Daten gefüllt wurden, sind in der Liste der verfügbaren
Schlüsselverzeichnisse grün markiert.

Die Schlüsselverzeichnisse gehören nicht eigentlich zu den Stammdaten, vielmehr handelt es sich um Daten zweiter Ordnung, die im Wesentlichen der Beschreibung oder Kategorisierung anderer Daten dienen. Sie kommen nicht nur im Programmbereich „Stammdaten“, sondern auch in den anderen Programmbereichen zum Einsatz. Die vollständige Bearbeitung der Stammdaten setzt aber in der Regel voraus, dass bestimmte Schlüsselverzeichnisse im Vorfeld angepasst werden.
Die verfügbaren Schlüsselverzeichnisse sehen Sie im Dialogfenster ``Schlüsselverzeichnisse``, das Sie über die Schaltfläche `Schlüsselverzeichnisse` in der Menügruppe `Start > Stammdaten` öffnen können.

!!! info "Hinweis"

    Wenn Sie sich nicht mehr im Programmbereich **Stammdaten** befinden, können Sie die Schlüsselverzeichnisse alternativ über das Menüregister `Extras > Verwalten` öffnen. Die Schaltfläche `Schlüsselverzeichnisse` steht Ihnen hier in allen Programmbereichen zur Verfügung. 

![Aufruf Schlüsselverzeichnisse](/assets/images/Aufruf.Schlüsselverzeichnisse.png)

![Schlüsselverzeichnisse](/assets/images/Schlüsselverzeichnisse.png)

Klicken Sie auf das Schlüsselverzeichnis, welches Sie bearbeiten wollen und dann auf `Bearbeiten`, um das betreffende Schlüsselverzeichnis Dialogfenster zu öffnen. Alternativ kann der Bearbeiten-Modus des Verzeichnisses auch per ``Doppelklick`` auf das gewünschte Verzeichnis geöffnet werden.

## Neue Schlüssel anlegen und bearbeiten

![Schlüsselverzeichnis Lehrerfehlgründe](/assets/images/Lehrerfehlgruende01.png)

Spalte | Bedeutung
-|-
Kürzel |Kürzel des Eintrags, wird in der Regel in Aufklappmenüs angezeigt, muss eindeutig sein
Schlüssel |Schlüsselwert des Eintrags, wird für die Statistik verwendet, d.h. Sie können für verschiedene Kürzel denselben Schlüsselwert verwenden, um schulintern zu differenzieren. Die korrekten Schlüsselwerte entnehmen Sie der Statistik-Dokumentation, welche die zuständigen Landesstatistikämter in der Regel einmal im Jahr neu veröffentlichen.
Bezeichnung | Langname
Farbe |Hintergrundfarbe (nur in bestimmten Schlüsselverzeichnissen verfügbar)
Gültig von |Datum, von dem ab dieser Schlüssel gültig ist
Gültig bis |Datum, bis zu dem dieser Schlüssel gültig ist bzw. war
ID |Eindeutige ID für den Magellan Abgleich
Verrechnen |Standardeinstellung, ob beim Erfassen einer Lehrerfehlzeit bei Auswahl dieses Grundes negative Anrechenstunden verbucht werden sollen

Neue Einträge legen Sie mit `Neuer Schlüssel` oder mit der `EINFG-Taste` an. Mit `Schlüssel löschen` können Sie einen oder mehrere (durch ``UMSCHALT-Mausklick`` oder ``STRG+Mausklick``) Schlüssel wieder löschen.

## Schlüssel importieren

Über ``Importieren`` können Sie Schlüsselverzeichnisse importieren, die von DAVINCI oder von Ihrem Bundesland in einer entsprechenden Schlüsseldatei zur Verfügung gestellt werden. Beim Importieren werden Schlüssel anhand des Kürzels oder des Schlüssels identifiziert: Bestehende Schlüssel werden überschrieben, neue angefügt.

![Import Lehrerfehlgründe](/assets/images/Lehrerfehlgruende.Import01.png)

!!! info "Hinweis"

    DAVINCI erwartet Schlüsseldateien mit der Endung .KEYS und mit der Nummer des Schlüsselverzeichnisses – siehe Dialogfenster `Extras > Schlüsselverzeichnisse` – als Präfix im Dateinamen, also z.B. „23_Unterrichtsarten.keys“. Standardmäßig sollten die so benannten Schlüsseldateien im Schlüsseldateien Ordner liegen, siehe Dialogfenster `Extras > System-Informationen > Ordner daVinciKeysFolder`.

Die Einträge in einer Schlüsseldatei müssen in einer TXT-, CSV- oder KEYS-Datei in einem bestimmten Format gespeichert sein. Eine Zeile des Schlüsselverzeichnisses entspricht dabei einer Zeile in der Importdatei. Das Format der CSV-Datei können Sie dem folgenden Beispiel entnehmen:

```
"Kuerzel";"Schluessel";"Bezeichnung";"GueltigVon";"GueltigBis"
```
!!! tip Tip

    Wenn Sie Schlüsseldateien importieren möchten, beachten Sie bitte: Die Dateien müssen immer den Aufbau haben wie im Schlüsselverzeichnis und sie mpssen einem bestimmten Format entsprechen. Sie müssten aus Excel heraus eine Daten über "Speichern unter" als "CSV (Trennzeichen getrennt)" speichern.
    
!!! info Hinweis
    Eine Übersicht über die verwendeten Schlüsselverzeichnisse finden Sie [hier](/00.allgemein/schluesselverzeichnisse/)
