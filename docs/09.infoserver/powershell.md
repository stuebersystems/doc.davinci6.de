# Netzwerke miteinander verbinden

In vielen Schulen kann kein öffentlicher Web-Server im Verwaltungsnetz betrieben werden. Das bedeutet u.a., dass der DAVINCI INFOSERVER nicht von außen zugreifbar ist. Die Lösung besteht darin, den DAVINCI INFOSERVER auf einem Web-Server in einem anderen öffentlich zugänglichen Netzwerk zu installieren. Dazu muss sichergestellt werden, dass der DAVINCI INFOSERVER von dort auf Daten eines DAVINCI SERVER im Verwaltungsnetzwerk zugreifen kann.

[![Netzwerke verbinden][1]][1] 

## Grundlegende Vorgehensweise

Die Antwort umfasst den Einsatz einiger zusätzlicher Software-Komponenten und soll im folgenden Kapitel genauer beschrieben werden. Die grundsätzliche Vorgehensweise sieht wie folgt aus:

1. Im öffentlich zugänglichen Netzwerk wird der DAVINCI SERVER und der DAVINCI INFOSERVER installiert. Eine Kopie der DAVINCI-Datei sowie eine Kopie der DAVINCI-Benutzerdatei (daVinci.users) aus dem Verwaltungsnetzwerk wird als Startkonfiguration angelegt.

2. Auf dem öffentlich zugänglichen Netzwerk wird ein FTP-Dienst installiert, der Dateien aus dem Verwaltungsnetzwerk entgegennehmen darf. Dieser FTP-Dienst erlaubt den direkten Zugriff auf den Arbeitsbereich des DAVINCI SERVER im öffentlich zugänglichen Netzwerk. Natürlich ist dieser Zugriff kennwortgeschützt.

3. Im Verwaltungsnetzwerk wird ein Automatismus implementiert, der sowohl die gewünschte DAVINCI-Plandatei als auch die DAVINCI-Benutzerdatei aus dem Arbeitsbereich des DAVINCI SERVER in regelmäßigen Abständen auf den FTP-Server kopiert.

4. Im öffentlich zugänglichen Netzwerk wird ebenfalls ein Automatismus implementiert, der beim Austausch der DAVINCI-Benutzerdatei den DAVINCI-Serverdienst neu startet. Der Austausch der DAVINCI-Plandatei wird vom DAVINCI SERVER selbst erkannt.

Zusammengefasst: Durch regelmäßiges Kopieren der DAVINCI-Plandatei sowie der DAVINCI-Benutzerdatei aus dem Verwaltungsnetzwerk in das öffentlich zugängliche Netzwerk wird eine Synchronisierung implementiert, die es erlaubt, einen DAVINCI-INFOSERVER außerhalb des Verwaltungsnetzwerkes zu betreiben.

[![Daten übertragen][2]][2] 

Bleibt noch die Frage zu klären, wie genau dieser Automatismus aussieht. Wir bieten hierzu eine Skript-basierte Lösung auf Basis von Powershell an. Sie ist frei verfügbar und Open Source.

## Ein kompletter Workflow mit Powershell

In unserem GitHub-Repository [davinci.powershell](https://github.com/stuebersystems/davinci.powershell) finden Sie [Powershell-Skripte](https://docs.microsoft.com/de-de/powershell/scripting/getting-started/getting-started-with-windows-powershell) zur Automation von Aufgaben rund um DAVINCI.

Powershell ist Bestandteil von Windows und ist u.a. speziell für die Automation von administrativen Aufgaben konzipiert.

Im Folgenden zeigen wir Ihnen einen kompletten Workflow für unser oben beschriebenes Szenario:

[![Workflow][3]][3]

### Schritt 1: Vorbereitung

1. Installieren Sie in Ihrem öffentlich zugänglichen Netzwerk den DAVINCI SERVER genauso, wie Sie es auch in Ihrem Verwaltungsnetzwerk bereits getan haben.

2. Speichern Sie mit Hilfe des DAVINCI EXPLORERS eine Kopie Ihrer DAVINCI-Plandatei auf diesem DAVINCI SERVER. 

3. Öffnen Sie in der Systemsteuerung das DAVINCI Server Control, wählen die Unterkarte `Arbeitsbereich` und setzen das Häkchen für `Sensitiv für Dateiänderungen`.

 [![Sensitiv für Dateiänderung][4]][4] 

1. [Installieren Sie den DAVINCI INFOSERVER](/09.infoserver/setup-infoserver/README.md).

2. Testen Sie, ob Sie per Web-Browser oder DAVINCI APP die gewünschten Daten angezeigt bekommen. Ist dies der Fall, sind Ihre Vorbereitungen fast abgeschlossen.

3. Installieren Sie nun auf dem selben Computer einen FTP-Dienst oder noch besser einen WebDAV-Server und konfigurieren Sie diesen so, dass er einen direkten Zugriff auf den Arbeitsbereich von DAVINCI erlaubt. Standardmäßig ist dies das Verzeichnis `C:\Users\Public\Documents\Stueber Systems\daVinci 6\Arbeitsbereich`.

!!! info "Hinweis"

    Die Option `Sensitiv für Dateiänderungen` aktivieren Sie bitte nicht für DAVINCI SERVER im Verwaltungsnetzwerk, sondern nur für den DAVINCI SERVER in Ihrem öffentlich zugänglichen Netzwerk (`Systemsteuerung > DAVINCI Server Control > Arbeitsbereich`)!

### Schritt 2: Der Datei-Workflow im Verwaltungsnetzwerk

Wir benötigen ein Skript, das in gewissen Zeitabständen prüft, ob sich die DAVINCI-Plandatei und/oder die DAVINCI-Benutzerdatei verändert haben. Ist dies der Fall, werden die Dateien per FTP oder WebDAV auf den Computer im öffentlichen Netzwerk übertragen.

Perfekt dafür geeignet ist das Powershell-Skript [uploadDavFiles.ps1](https://github.com/stuebersystems/davinci.powershell/wiki/uploadDavFiles.ps1).

### Schritt 3: Der Datei-Workflow im öffentlich zugänglichen Netzwerk

Wir benötigen ein Skript, das in gewissen Zeitabständen prüft, ob sich die DAVINCI-Benutzerdatei verändert hat. Ist dies der Fall, wird der DAVINCI SERVER neu gestartet.

Perfekt dafür geeignet ist das Powershell-Skript [restartDavServer.ps1](https://github.com/stuebersystems/davinci.powershell/wiki/restartDavServer.ps1).

## Schritt 4: Kontrolle

Das war's! Sie können den Workflow testen, indem Sie im Verwaltungsnetzwerk eine Änderung in der entsprechenden DAVINCI-Plandatei vornehmen. Einige Sekunden später sollte diese auch vom DAVINCI INFOSERVER publiziert werden.

[1]:/assets/images/is/sigma1.svg
[2]:/assets/images/is/sigma2.svg
[3]:/assets/images/is/sigma3.svg
[4]:/assets/images/issensitiv.haken.png