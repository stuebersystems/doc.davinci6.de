#	Die Paths-Datei

Die Konfigurationsdateien werden für jeden Benutzer eines Computers angelegt. Wenn Sie im Netzwerk mit verschiedenen Clients arbeiten, können Sie eine PATHS-Datei verwenden, um globale Konfigurationen für alle Benutzer herzustellen, beispielsweise eine gemeinsame Druckformatedatei verwenden: Dazu können Sie die XML-Textdatei daVinci.paths für daVinci bzw. die Datei daVinciLook.paths für daVinci LOOK verwenden. 

In diesen Dateien werden die Pfade für bestimmte Konfigurationsdateien festgelegt. DAVINCI verwendet dann diese Pfadangaben, anstatt der Standardpfade. Beispielsweise unter der Angabe „daVinciPrintFormatFile“ finden Sie diesen Pfad auch im Fenster `Extras > System-Informationen` wieder.

## Wie funktioniert es

Sie kopieren die gewünschten Konfigurationdateien von einem eingerichteten System in ein Verzeichnis, auf das die Nutzer zugreifen können, beispielsweise auf ein freigegebenes Verzeichnis auf Ihrem Server. Die Ablagestellen der einzelen Dateien finden Sie aus DAVINCI oder DAVINCI LOOK heraus unter `Hilfe > Systeminfo`. Sie kopieren die gewünschte nachstehende Vorlage, löschen die nicht benötigten Zeilen, und passen den Pfad so an, dass auf Ihr freigegebenes Serververzeichnis verwiesen wird. Der Pfad endet mit dem jeweiligen Dateinamen, wie in der Vorlage.
Die fertige Datei benennen Sie dann je nach Vorlage in `daVinciLook.paths` oder `daVinci.paths`, bitte achten Sie darauf, dass die Dateiendung auch `*.paths` ist, und nicht versehentlich durch ausgeblendete Dateierweiterungen noch `*.txt` lautet. 
Im Abschnitt "Ablagepfade für daVinci.paths und davinciLook.paths" werden die Stellen aufgezählt, an denen die Dateien erkennen würde. 

Ein Beispiel:<br/> Sie legen Ihre angepasste `daVinci.paths` parallel zur `daVinci.exe` unter `C:\Program Files (x86)\Stueber Systems\daVinci 6` ab. Beim Programmstart erkennt die DAVINCI die Datei anhand des Dateinames und liest erst die Pfade aus der Datei aus, im Anschluss die Inhalte der Konfigurationsdateien. 

## Vorlagen 

Die nachfolgenden Beispiele können Sie als Vorlage in eine Textdatei kopieren und dann den Pfad auf Ihr selbst angelegtes und freigegebenes Serververzeichnis anpassen - nicht benötigte Zeilen löschen Sie.

### für DAVINCI

```
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<Preferences>
 <Paths>
  <Entry Name="daVinciOptionFile" Value="\\Mein_Server\...\Pathsdateien\daVinciLook.lic"/>
  <Entry Name="daVinciPrintFormatFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.pfm"/>
  <Entry Name="daVinciOptionFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.opt"/>
  <Entry Name="daVinciHTMLFormatFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.hfm"/>
  <Entry Name="daVinciConfigurationFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.cfg"/>
  <Entry Name="daVinciSiteFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.site"/>
  <Entry Name="daVinciServerListFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.servers"/>
  </Paths>
</Preferences>
```

**Bitte beachten Sie, dass anders als bei MAGELLAN, der Verweispfad jeweils mit dem Dateinamen enden muss.**

### für DAVINCI LOOK

```
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<Preferences>
 <Paths>
  <Entry Name="daVinciOptionFile" Value="\\Mein_Server\...\Pathsdateien\daVinciLook.opt"/>
  <Entry Name="daVinciPrintFormatFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.pfm"/>
  <Entry Name="daVinciConfigurationFile" Value="\\Mein_Server\...\Pathsdateien\daVinciLook.cfg"/>
  <Entry Name="daVinciServerListFile" Value="\\Mein_Server\...\Pathsdateien\daVinci.servers"/>
  </Paths>
</Preferences>
```

**Bitte beachten Sie, dass anders als bei MAGELLAN, der Verweispfad jeweils mit dem Dateinamen enden muss.**

## Ablagepfade für daVinci.paths und davinciLook.paths

Sie können die PATHS-Datei im Programmordner oder in den Datenordnern ablegen, siehe dazu die folgende Tabelle. Diese Ordner können je nach Betriebssystemversion variieren. Um welche Ordner es sich genau handelt, können Sie in daVinci bzw. in daVinci LOOK dem Fenster `Hilfe > System-Informationen` entnehmen.

Mögliche Ordner für die Datei “daVinci.paths“ |Mögliche Ordner für die Datei “daVinciLook.paths“ 
---|---
daVinciBinFolder	|daVinciLookBinFolder
daVinciDataFolder	|daVinciLookDataFolder
daVinciCommonDataFolder	|daVinciLookCommonDataFolder

> Die vollständige Pfadangabe zur aktuell verwendeten PATHS-Datei können Sie dem Eintrag „daVinciCustomPathsFile“ im Fenster `Hilfe > System-Informationen` entnehmen.

Die PATH-Datei kann die Pfadangaben für folgende Dateien festlegen:

**daVinci.paths**

Name|Datei|Beschreibung
---|---|---
daVinciOptionFile|daVinci.opt|Optionsdatei
daVinciHTMLFormatFile|daVinci.hfm|HTML Exportformate
daVinciPrintFormatFile|daVinci.pfm|Druckformate
daVinciConfigurationFile|daVinci.cfg|Aktuelle Login-Daten
daVinciSiteFile	|daVinci.site|Standortdaten (Schulname, Adresse, etc.)
daVinciServerListFile|daVinci.servers|Serververbindung und Startdatei

**daVinciLook.paths**

Name	|Datei	|Beschreibung
---|---|---
daVinciOptionFile|	daVinciLook.opt |	Optionsdatei
daVinciPrintFormatFile	|daVinci.pfm |	Druckformate
daVinciConfigurationFile	|daVinciLook.cfg|	Aktuelle Login-Daten
daVinciServerListFile|	daVinci.servers|	Serververbindung und Startdatei
