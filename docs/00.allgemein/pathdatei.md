# Die Paths-Datei

Die Optionsdateien werden für jeden Benutzer eines Computers angelegt. Wenn Sie im Netzwerk mit verschiedenen Clients arbeiten, können Sie eine PATHS-Datei verwenden, um globale Konfigurationen für alle Benutzer herzustellen: Dazu können Sie die XML-Textdatei **daVinci.paths **für DAVINCI bzw. die Datei **daVinciLook.paths** für DAVINCI LOOK verwenden.

In diesen Dateien werden die Pfade für bestimmte Optionsdateien festgelegt. DAVINCI verwendet dann diese Pfadangaben, anstatt der Standardpfade.

Beispiel für eine PATH-Datei  

```xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<Preferences>
 <Paths>
  <Entry Name="daVinciPrintFormatFile" Value="D:\DAVINCI\DAVINCI.pfm"/>
  </Paths>
</Preferences> 
```

Unter der Angabe ``daVinciPrintFormatFile`` finden Sie diesen Pfad auch im Fenster `Extras > SystemInformationen`wieder. Sie können die PATHS-Datei im Programmordner oder in den Datenordnern ablegen, siehe dazu die folgende Tabelle. Diese Ordner können je nach Betriebssystemversion variieren. Um welche Ordner es sich genau handelt, können Sie in DAVINCI bzw. in DAVINCI LOOK dem Fenster `Hilfe > System-Informationen` entnehmen.

|Mögliche Ordner für die Datei ``daVinci.paths`` | Mögliche Ordner für die Datei ``daVinciLook.paths``| 
|--- | ---|
|daVinciBinFolder | daVinciLookBinFolder|
| daVinciDataFolder | daVinciLookDataFolder |
| daVinciCommonDataFolder | daVinciLookCommonDataFolder |

Die PATH-Datei `daVinci.paths` kann die Pfadangaben für folgende Dateien festlegen:

| Name | Datei | Beschreibung |
| --- | --- | --- |
| daVinciOptionFile | daVinci.opt | Optionsdatei |
| daVinciHTMLFormatFile | daVinci.hfm | HTML Exportformate |
| daVinciPrintFormatFile | daVinci.pfm | Druckformate |
| daVinciConfigurationFile | daVinci.cfg | Aktuelle Login-Daten |
| daVinciSiteFile | daVinci.site | Standortdaten (Schulname, Adresse, etc.) |
| daVinciServerListFile | daVinci.servers | Serververbindung und Startdatei |

Die PATH-Datei `daVinciLook.paths` kann die Pfadangaben für folgende Dateien festlegen:

| Name | Datei | Beschreibung |
| --- | --- | --- |
| daVinciOptionFile | daVinciLook.opt | Optionsdatei |
| daVinciPrintFormatFile | daVinci.pfm | Druckformate |
| daVinciConfigurationFile | daVinciLook.cfg | Aktuelle Login-Daten |
| daVinciServerListFile | daVinci.servers | Serververbindung und Startdatei |
