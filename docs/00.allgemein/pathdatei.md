# Mehrere Arbeitsplatzrechner einrichten: Die Paths-Datei

Beim Start von DAVINCI werden Informationen wie zum Beispiel Optionen, Lizenzdaten oder Pfade zur Datei, den Datenordnern uws. aus Dateien gelesen. Diese Dateien werden standardmäßig an einem betriebssystemspezifischen Ort pro DAVINCI-Installation angelegt und dort auch ausgelesen. Alternativ können diese Dateien auch an einer beliebigen anderen Stelle in Ihrem Netzwerk liegen und DAVINCI liest den Pfad zu den Dateien aus der Paths-Datei (daVinci.paths) aus.

Der Vorteil einer Paths-Datei ist, dass Sie mehreren Nutzern die identischen Einstellungen in einem Arbeitsschritt an einem zentralen Ort zur Verfügung stellen können.

Beispiel: Die DAVINCI Lizenz wird nur an einer einzigen Stelle im Netzwerk eingespielt, ist aber für alle Kollegen erreichbar. Auch beim Einrichten einer neuen Arbeitsplatzsituation spart man sich einzelne Schritte: es genügt die Installation durchzuführen und die DAVINCI.paths im Programmverzeichnis abzulegen.

Folgende Dateien werden beim Programmstart von DAVINCI gelesen:

| Datei           | Inhalt                                               |
| --------------- | ---------------------------------------------------- |
| daVinci.lic     | enthält die Lizenzierungsdaten                       |
| daVinci.opt     | enthält die DAVINCI-Optionseinstellungen             |
| daVinci.hfm     | enthält die HTML Exportformate                       |
| daVinci.pfm     | enthält die Druckformate                             |
| daVinci.cfg     | enthält die Aktuelle Login-Daten                     |
| daVinci.site    | enthält die Standortdaten (Schulname, Adresse, etc.) |
| daVinci.servers | enthält die Serververbindung und Startdatei          |

Diese Dateien liegen je nach Betriebssystem an folgenden voreingestellten Speicherorten:

| Betriebssystem      | Pfad                                     |
| ------------------- | ---------------------------------------- |
| Windows Vista       | C:\ProgramData\Stueber Systems\DAVINCI 7 |
| Windows 7/8         | C:\ProgramData\Stueber Systems\DAVINCI 7 |
| Windows Server 2008 | C:\ProgramData\Stueber Systems\DAVINCI 7 |
| Windows 10          | C:\ProgramData\Stueber Systems\DAVINCI 7 |

Über `Hilfe > System Informationen` finden Sie in DAVINCI die Pfade der entsprechenden Dateien:

*  daVinciOptionFile > daVinci.opt
*  daVinciPrintFormatFile > daVinci.pfm
*  daVinciConfigurationFile > daVinciLook.cfg 
* etc.
  
Möchten Sie abweichende Speicherorte für diese Dateien angeben, zum Beispiel damit alle DAVINCI-Arbeitsplatzinstallationen auf dieselben Dateien zugreifen, sind folgende Schritte nötig:

1. Richten Sie einen Arbeitsplatz vollständig ein, damit Sie von diesem Arbeitsplatz aus die ``daVinci.pfm``, die ``daVinci.lic`` und die ``daVinci.opt`` kopieren können. 

2. Wählen Sie einen Speicherort für die Konfigurationsdateien aus. Die Dateien können in einem gemeinsamen Verzeichnis liegen oder Sie wählen für ``daVinci.lic``, die Optionsdatei (`daVinci.opt` und die `daVinci.pfm`,getrennte Verzeichnisse und speichern dort die Dateien.

3. Erstellen Sie mit einem Texteditor eine neue Textdatei und kopieren den nachfolgenden Text in diese Datei. Passen Sie die Pfade bitte auf Ihre angelegten Verzeichnisse an, diese können sich lokal auf dem Rechner oder in Ihrem Netzwerk befinden.

Beispiel:

``` xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<Preferences>
  <Paths>
    <Entry Name="daVinciPrintFormatFile" Value="D:\Mein Verzeichnis\daVinci.pfm"/>
    <Entry Name="daVinciOptionsFolder" Value="D:\Mein Verzeichnis\daVinci.opt"/>
    <Entry Name="daVinciLicenseFolder" Value="D:\Mein Verzeichnis\daVinci.lic"/>
  </Paths>
</Preferences>
```

Weiter geht's:

1. Speichern Sie diese Textdatei und benennen die Datei anschließend in „daVinci.paths“ um.

2. Legen Sie diese Datei pro Arbeitsplatzinstallation im Programmverzeichnis (parallel zur daVinci.exe) ab. Beim Programmstart von DAVINCI wird geprüft, ob sich eine Datei mit diesem Namen im Programmverzeichnis befindet und gegebenenfalls ausgelesen.

!!! warning "Wichtig"

    Wenn Sie per DAVINCI.paths auch auf die Optionsdatei verweisen und wünschen, dass die Benutzer Optionen selbst einstellen dürfen, müssen die Benutzer auch die Rechte haben an der Ablagestelle der daVinci.opt Änderungen vorzunehmen.

Die Paths-Datei `daVinci.paths` kann für DAVINCI die Pfadangaben für folgende Dateien festlegen:

| Name                     | Datei           | Beschreibung                             |
| ------------------------ | --------------- | ---------------------------------------- |
| daVinci.lic              | daVinci.lic     | Lizenzdatei                              |
| daVinciOptionFile        | daVinci.opt     | Optionsdatei                             |
| daVinciHTMLFormatFile    | daVinci.hfm     | HTML Exportformate                       |
| daVinciPrintFormatFile   | daVinci.pfm     | Druckformate                             |
| daVinciConfigurationFile | daVinci.cfg     | Aktuelle Login-Daten                     |
| daVinciSiteFile          | daVinci.site    | Standortdaten (Schulname, Adresse, etc.) |
| daVinciServerListFile    | daVinci.servers | Serververbindung und Startdatei          |

Die Paths-Datei `daVinciLook.paths` kann für DAVINCI LOOK die Pfadangaben für folgende Dateien festlegen:

| Name                     | Datei           | Beschreibung                    |
| ------------------------ | --------------- | ------------------------------- |
| daVinciOptionFile        | daVinciLook.opt | Optionsdatei                    |
| daVinciPrintFormatFile   | daVinci.pfm     | Druckformate                    |
| daVinciConfigurationFile | daVinciLook.cfg | Aktuelle Login-Daten            |
| daVinciServerListFile    | daVinci.servers | Serververbindung und Startdatei |
