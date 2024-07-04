# DaVinci Updates

In regelmäßigen Abständen werden für DaVinci Service-Updates veröffentlicht, die neue oder erweiterte Programmfunktionen beinhalten. Um diese Funktionen laut Ihrer Lizenz nutzen zu können, müssen Sie ein Update für DaVinci ausführen.

!!! warning "Wichtig"

    Sollten Sie neben DaVinci 6 auch andere DaVinci  Programme benutzen (z.B.: DaVinci Look, DaVinci InfoServer oder DaVinci Enterprise) müssen die Updates für alle genutzten Programmteile eingespielt werden.

## So aktualisieren Sie DaVinci

### Manuelles Einspielen von Updates

In der Regel werden aktuelle Updates zu DaVinci auf unserer Internetseite im Downloadbereich bereitgestellt, die Sie auf Ihren Rechner herunterladen und per Doppelklick ausführen. Zu finden unter: [https://davinci.stueber.de/download.php](https://davinci.stueber.de/download.php)

Gehen Sie wie folgt vor:

* Öffnen Sie die Webseite [download.davinci.stueber.de](https://davinci.stueber.de/download.php) in Ihrem Web-Browser.

* Klicken Sie unterhalb von DaVinci auf die Schaltfläche `Download`, um die aktuellste Installationsdatei `davinci6.msi` herunterzuladen.
* Starten Sie die Installationsdatei `davinci6.msi` per Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Sie können den Download auch aus dem Programm heraus starten. Öffnen Sie dazu DaVinci 6 und wählen `Hilfe > Auf Aktualisierung prüfen`. Das Programm wird nun automatisch prüfen, ob für Ihre Installation ein Update vorliegt und bei Bedarf herunterladen.

!!! warning "Wichtig"

    Das Installationsprogramm erkennt automatisch, ob es eine bestehende DaVinci-Version aktualisieren oder eine Neuinstallation durchführen muss.

### Automatisches Update – Online

Sie können in DaVinci das automatische Update aktivieren, wenn Sie den Updatevorgang  
automatisieren möchten. Aktivieren Sie diese Option unter `Extras > Optionen > Auto-Update`. Das Update wird über die Update-Infodatei gesteuert, die Sie auf dieser Registerkarte ebenfalls angeben müssen. Standardmäßig liegt diese Date bzw. Die Updatedatei selbst auf den STÜBER SYSTEMS Website, klicken sie dazu ggf. auf `Standardvorgabe wiederherstellen`.

![Die Ansicht `Auto-Update` im Dialogfenster DaVinci Optionen](/assets/images/allgemein/AutoUpdate.png)

### Automatisches Update – im Netzwerk

Sie können die Updateinformationen so anpassen, dass DaVinci das aktuelle Update nicht von unseren Internetseiten, sondern von einem Netzwerkpfad Ihres Netzwerks bezieht. Laden Sie dazu das Installationspaket von unseren Internetseiten herunter, und legen dieses zentral in einem für jeden Nutzer erreichbaren Ordner des Netzwerks ab.  
Laden Sie anschließend die zur Verfügung stehende ``.UPDATEINFO`` Datei von unserer Internetseite und legen diese in den selben Ordner. Öffnen Sie die ``.UPDATEINFO`` Datei mit einem einfachen Textbearbeitungsprogramm (z.B.: den Windows Editor) und passen Sie den Pfad des Installationspaketes an.

!!! info "Hinweis"

    Die ``.UPDATEINFO`` Datei enthält die Informationen zum Pfad des Installationspakets und  zur Versionsnummer des Updates. Diese Informationen liest DaVinci aus und kann somit dem Benutzer melden, ob das Update eine höhere Versionsnummer als seine Installation besitzt oder nicht. 

Nun müssen Sie bei den einzelnen Clients unter `Extras > Optionen > Auto-Update`den Pfad zur soeben geänderten ``.UPDATEINFO`` Datei eintragen.

## DaVinci-Look updaten

Ein ausführliche Beschreibung des Updates von DaVinci-Look finden Sie im Kapitel [DaVinci-Look installieren](https://doc.davinci6.stueber.de/05.look/01.installation/#update)

## DaVinci-Server updaten

Ein ausführliche Beschreibung des Updates von DaVinci-SERVERS finden Sie im Kapitel [DaVinci-Server installieren](https://doc.davinci6.stueber.de/06.enterprise/01.installation/#update)

## DaVinci-InfoServer updaten

Ein ausführliche Beschreibung des Updates des DaVinci-INFOSERVERS finden Sie im Kapitel [DaVinci-InfoServer installieren](https://doc.davinci6.stueber.de/06.enterprise/01.installation/#update)
