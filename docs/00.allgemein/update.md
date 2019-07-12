# DAVINCI Updates

In regelmäßigen Abständen werden für DAVINCI Service-Updates veröffentlicht, die neue oder erweiterte Programmfunktionen beinhalten. Um diese Funktionen laut Ihrer Lizenz nutzen zu können, müssen Sie ein Update für DAVINCI ausführen.

!!! warning "Wichtig"

    Sollten Sie neben DAVINCI 6 auch andere DAVINCI  Programme benutzen (z.B.: DAVINCI LOOK, DAVINCI INFOSERVER oder DAVINCI ENTERPRISE) müssen die Updates für alle genutzten Programmteile eingespielt werden.

## So aktualisieren Sie DAVINCI

### Manuelles Einspielen von Updates

In der Regel werden aktuelle Updates zu DAVINCI auf unserer Internetseite im Downloadbereich bereitgestellt, die Sie auf Ihren Rechner herunterladen und per Doppelklick ausführen. Zu finden unter: [https://davinci.stueber.de/download.php](https://davinci.stueber.de/download.php)

Gehen Sie wie folgt vor:

* Öffnen Sie die Webseite [download.davinci.stueber.de](https://davinci.stueber.de/download.php) in Ihrem Web-Browser.

* Klicken Sie unterhalb von DAVINCI auf die Schaltfläche `Download`, um die aktuellste Installationsdatei `davinci6.msi` herunterzuladen.

* Starten Sie die Installationsdatei ``davinci6.msi`` per Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Sie können den Download auch aus dem Programm heraus starten. Öffnen Sie dazu DAVINCI 6 und wählen `Hilfe > Auf Aktualisierung prüfen`. Das Programm wird nun automatisch prüfen, ob für Ihre Installation ein Update vorliegt und bei Bedarf herunterladen.

!!! warning "Wichtig"

    Das Installationsprogramm erkennt automatisch, ob es eine bestehende DAVINCI-Version aktualisieren oder eine Neuinstallation durchführen muss.

### Automatisches Update – Online

Sie können in DAVINCI das automatische Update aktivieren, wenn Sie den Updatevorgang  
automatisieren möchten. Aktivieren Sie diese Option unter `Extras > Optionen > Auto-Update`. Das Update wird über die Update-Infodatei gesteuert, die Sie auf dieser Registerkarte ebenfalls angeben müssen. Standardmäßig liegt diese Date bzw. Die Updatedatei selbst auf den STÜBER SYSTEMS Website, klicken sie dazu ggf. auf `Standardvorgabe wiederherstellen`.

![Die Ansicht `Auto-Update` im Dialogfenster DAVINCI Optionen](/assets/images/AutoUpdate.png)

### Automatisches Update – im Netzwerk

Sie können die Updateinformationen so anpassen, dass DAVINCI das aktuelle Update nicht von unseren Internetseiten, sondern von einem Netzwerkpfad Ihres Netzwerks bezieht. Laden Sie dazu das Installationspaket von unseren Internetseiten herunter, und legen dieses zentral in einem für jeden Nutzer erreichbaren Ordner des Netzwerks ab.  
Laden Sie anschließend die zur Verfügung stehende ``.UPDATEINFO`` Datei von unserer Internetseite und legen diese in den selben Ordner. Öffnen Sie die ``.UPDATEINFO`` Datei mit einem einfachen Textbearbeitungsprogramm (z.B.: den Windows Editor) und passen Sie den Pfad des Installationspaketes an.

!!! info "Hinweis"

    Die ``.UPDATEINFO`` Datei enthält die Informationen zum Pfad des Installationspakets und  zur Versionsnummer des Updates. Diese Informationen liest DAVINCI aus und kann somit dem Benutzer melden, ob das Update eine höhere Versionsnummer als seine Installation besitzt oder nicht. 

Nun müssen Sie bei den einzelnen Clients unter `Extras > Optionen > Auto-Update`den Pfad zur soeben geänderten ``.UPDATEINFO`` Datei eintragen.

## DAVINCI-LOOK updaten

Ein ausführliche Beschreibung der Installation von DAVINCI-LOOK finden Sie im Kapitel [DAVINCI-LOOK installieren]

## DAVINCI-SERVER updaten

Ein ausführliche Beschreibung der Installation von DAVINCI-SERVERS finden Sie im Kapitel [DAVINCI-SERVER installieren]

## DAVINCI-INFOSERVER updaten

Ein ausführliche Beschreibung der Installation des DAVINCI-INFOSERVERS finden Sie im Kapitel [DAVINCI-INFOSERVER installieren]
