# Ausfallstatistik Sachsen

Die Übersicht `Übersichten > Ausfallstatistik` liefert die für die Landesstatistik Sachsen benötigten Daten.

Die grundlegende Beschreibung der Ausfallstatistik finden Sie [hier](https://doc.davinci6.stueber.de/08.analytics/ausfallstatistik/)

Damit die Ausfallstatistik korrekt erstellt werden kann, müssen Sie in DAVINCI

1. die entsprechenden Schulformen (berufsbildenden Schulen) bzw. Fächer (allgemeinbildende Schulen) verwenden
2. die entsprechenden Lehrerfehlgründe verwenden
3. die entsprechenden Klassenfehlgründe verwenden
4. die entsprechenden Vertretungsentfallgründe verwenden

## Schulformen

![Dialog unter Plan > DAVINCI-Optionen > Meine Daten](/assets/images/sac.optionen.png)

Sie erhalten von der Sächsischen Bildungsagentur ein Vorlage für die zu nutzenden Fächern und Schulformen für Sachsen:

1. Geben Sie unter `Plan > DAVINCI-Optionen > Meine Daten`

* bei `Schultyp` Ihr Schulartkürzel ein
* bei `Dienststelle/SchulNr` Ihre Dienststellenummer ein
  
2. Tragen Sie in den `Stammdaten > Fächer` die Fächer entsprechend ein
  
3. Weisen Sie in den `Stammdaten > Klassen > Schulform`die entsprechende Schulform zu. Grundlage ist das Schlüsslverzeichnis `Schulformen` welches vorher entsrpechend der Vorgabe zu füllen ist. 


!!! info "Hinweis"

  Beim Importieren wird über das jeweilige Kürzel synchronisiert, d.h. falls das Kürzel bereits vorhanden ist, wird der Datensatz modifiziert (Schlüssel und Bezeichnungen  werden übernommen), sonst wird der Datensatz hinzugefügt. Wenn Sie die Daten in einen schon fertigen Plan importieren in dem bereits Fächer, Schulformen, Fehlgründe und Entfallgründe verwendet werden, sollten Sie die entsprechenden Angaben in den Verzeichnissen manuell nachtragen. 

### Lehrerfehlgründe und Klassenfehlgründe

Kürzel  | Schlüssel| Kommentar
--------------|----------|---------
Krank| krankheit  | -|
Fortbildung| fortbildung  | -  |
Gremienarbeit | gremienarbeit | - |
Klassenfahrt  | klassenfahrt | - |
Wandertag  | wandertag | -|
Theater | theater| -|
Sonstiges  | sonstiges| sammelt alle anderen Gründe|

### Vertretungsentfallgründe

Kürzel  | Schlüssel
--------------------|-------------------
Stillbeschäftigung  | stillbeschaeftigung
Ausfall | ausfall  

!!! info "Hinweis"

     Die Schlüssel werden von DAVINCI zur Identifiktation der korrekten Daten für die Landesstatistik verwendet und müssen genauso geschrieben werden wie in den beiden Tabellen angegeben, dies gilt insbesondere für die Groß- und Kleinschreibung. Das Kürzel ist dafür nicht relevant, Sie können es daher auch anders benennen bzw. anders schreiben. 

Anschließend können Sie bei `Von`und `Bis` den Zeitraum einstellen, für den die Statistik erstellt werden soll. Klicken Sie dann auf `Aktualisieren` um die Summen von DAVINCI berechnen zu lassen. Speichern Sie das Ergebnis mit `Exportieren` als XML-Datei und senden Sie diese an die Sächsische Bildungsagentur.
