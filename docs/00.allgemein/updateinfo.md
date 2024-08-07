# Die Update-Infodatei

Jedes Installationspaket von DaVinci besitzt eine korrespondierende Update-Infodatei. Dies ist eine kleine XML-Datei, die es DaVinci ermöglicht, eine neuere Version automatisch zu erkennen, herunterzuladen und zu installieren. Update-Infodateien besitzen die Dateiendung `.UPDATEINFO`.

Die Update-Infodateien für DaVinci und DaVinci-Look finden Sie hier:

* [Update-Infodatei für DaVinci-Setup]
* [Update-Infodatei für DaVinci Look-Setup]

Sie können die DaVinci so anpassen, dass aktuelle Updates nicht von unseren Internetseiten, sondern von einem Netzwerkpfad Ihres Netzwerks bezogen werden.

## Lokales Ablegen des Setups

Laden Sie dazu das Installationspaket von unseren Internetseiten herunter, und legen Sie dieses zentral in einem für jeden Nutzer erreichbaren Ordner des Netzwerks ab. Laden Sie anschließend die zur Verfügung stehende Update-Infodatei von unserer Internetseite und legen diese in den selben Ordner. Öffnen Sie die Datei mit einem einfachen Textbearbeitungsprogramm (z.B. Windows Notepad) und passen Sie den Pfad des Installationspaketes an, indem Sie die URL gegen Ihren Netzwerkpfad austauschen.

Ein Beispiel für eine Update-Infodatei:

``` xml
<?xml version="1.0" encoding="UTF-8"?>
<UpdateInfo>
  <UpdatePackage 
     Product="daVinci6" 
     ProductVersion="6.0.210" 
     SetupFileName="daVinci6.msi"
     SetupURL="https://download.stueber.de/bin/de/davinci/v6/davinci6.msi"
     SetupSize="128726016" />
</UpdateInfo>
```

## Anpassen der Clients

Damit DaVinci weiß, dass es nicht auf unseren Internetseiten sondern in Ihrem Netzwerk nach neuen Updates suchen soll, müssen Sie bei allen Clients unter `Extras > Optionen > Auto-Update` den Pfad zu Ihrer Update-Infodatei eintragen.

[Update-Infodatei für DaVinci-Setup]: https://download.stueber.de/bin/de/davinci/v6/davinci6.updateinfo
[Update-Infodatei für DaVinci Look-Setup]:  https://download.stueber.de/bin/de/davinci/v6/davinci6look.updateinfo
