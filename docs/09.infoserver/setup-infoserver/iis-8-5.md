# DaVinci InfoServer und IIS 8.5

Dieses Kapitel beschreibt die Installation und Konfiguration des DaVinci InfoServer als ISAPI-Modul für Ihren IIS-Web-Server.

!!! info "Hinweis"

    Internet Server API (ISAPI) ist eine Programmierschnittstelle von Microsoft, die sowohl von den Microsoft Internetinformationsdiensten (IIS) wie auch vom Apache Web-Server unterstützt werden. ISAPI-Module erweiteren die Standardfunktionalität von Web-Servern.

## Installation des DaVinci InfoServer

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite `http://download.davinci.stueber.de` in Ihrem Web-Browser.

2. Klicken Sie unterhalb von "DaVinci-InfoServer" auf `Download`. Ihr Web-Browser lädt jetzt das Installationpaket `daVinci6Infoserver.msi` herunter.

3. Starten Sie das Installationpaket `daVinci6Infoserver.msi` durch Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Nach der Beendigung der Installation finden Sie in Ihrem DaVinci-Verzeichnis einen neuen Unterordner mit Namen `ISAPI` und dort eine Datei namens `daVinciIS.dll`. Also z.B.

```
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

Dies ist der DaVinci-InfoServer, eine DLL, die Sie nun Ihrem Web-Server als ISAPI-Erweiterung bekannt machen müssen.

## Konfiguration des IIS-Web-Servers

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Alle Apps > Windows-Verwaltungsprogramme > Internetinformationsdienste (IIS)-Manager`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DaVinci-InfoServer installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `Handlerzuordnungen`. Die Ansicht "Handlerzuordnungen" öffnet sich.

4. Klicken Sie nun auf `Modulzuordnung hinzufügen` auf der rechten Seite unter `Aktionen`. Ein Dialogfenster öffnet sich.

5. Tragen Sie in diesem Dialogfenster unter "Anforderungspfad" `daVinciIS.dll` ein, wählen Sie unter "Modul" `IsapiModule` aus, tragen Sie unter "Ausführbare Datei (optional)" den kompletten Pfad zur DaVinci-InfoServer-DLL ein, z.B.

```
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

6. Zu guter letzt vergeben Sie dieser Zuordnung noch einen aussagekräftigen Namen (z.B. `DaVinci-InfoServer 6`)

[![Modulzuordnung hinzufügen][1]][1] 

7. Klicken Sie zusätzlich auf die Schaltfläche `Einschränkungen` und entfernen Sie die Markierung `Handler nur bei folgender Zuordnung aufrufen` auf der Registerkarte "Zuordnung".

[![Beschriftung][2]][2] 

* Bestätigen Sie beide Dialogfenster mit `OK`.

Sollten Sie eine 64-bit-Version von Windows einsetzen, müssen Sie zusätzlich noch folgende Einstellungen im IIS-Manager vornehmen:

1. Markieren Sie in der linken Navigation den Eintrag "Anwendungspool" und klicken Sie anschließend auf der rechten Seite unter "Aktionen" auf `Erweiterte Einstellungen`. Ein Dialogfenster öffnet sich.

2. Setzen Sie die Eigenschaft "32-Bit Anwendungen aktivieren" auf `True` und klicken Sie anschließend auf `OK`.

[!["32-Bit-Anwendungen aktivieren"][3]][3] 

## Ein erster Test

Unser DaVinci InfoServer ist nun installiert, aber noch nicht konfiguriert. Wir haben ihm nämlich noch nicht gesagt, mit welchem DaVinci Server er kommunizieren soll. Bevor wir dies tun, wollen wir aber zunächst einmal testen, ob der DaVinci InfoServer überhaupt auf Anfragen reagiert.

1. Öffnen Sie Ihren Web-Browser und tippen Sie ein:

```
http://localhost/isapi/davinciis.dll
```

1. 2. Wenn Ihr Web-Browser nun folgende vom DaVinci InfoServer generierte Meldung anzeigt, ist der DaVinci InfoServer bereit auf Anfragen zu reagieren:

[![Fehlerseite des DaVinci INFOSERVERS][4]][4] 

## Den DaVinci InfoServer konfigurieren

Wie bereist erwähnt, ist der DaVinci InfoServer nur ein Vermittler zwsischen einem Client wie z.B. dem Web-Browswer oder DaVinci Mobile und einem DaVinci Server. Voraussetzung für einen sinnvollen Einsatz des DaVinci INFOSERVERS ist also eine Installation des DaVinci SERVERS in Ihrem Netzwerk.

Ist dies der Fall, können Sie den DaVinci InfoServer konfigurieren:

1. Öffnen Sie die Windows-Systemsteuerung und klicken Sie auf `daVinci-InfoServer`. Ein Dialogfenster öffnet sich

2. Wechseln Sie auf die Registerkarte `Server-Verbindung` und tragen Sie dort die Verbindungsdaten zu Ihrem DaVinci Server ein. Für die Kommunikation mit dem DaVinci-Server ist ein Benutzerkonto mit entsprechenden Rechten notwendig. Verwenden Sie bitte als Benutzer Ihren zuvor definierten "Webuser" und das dazugehörige Passwort. Weitere Informationen zum Benutzer "Webuser" finden Sie im Kapitel "Benutzerverwaltung".

[![Server-Verbindung][5]][5]

4. Der Pfad unter `Webseiten-Pfad` ist in der Regel bereits ausgefüllt und muss nicht geändert werden:

```txt
C:\ProgramData\Stueber Systems\daVinci 6 InfoServer
```

1. Wechseln Sie zur Registerkarte `Plandatei`. Hier tragen Sie den Namen der Datei, die Sie auf dem DaVinci Server ansprechen wollen, sowie deren eindeutige GUID ein. In DaVinci können Sie beide Angaben unter `Plan > Eigenschaften > Allgemein` einsehen, sobald Sie mit dem DaVinci-Server verbunden sind und die Datei geöffnet haben. Alternativ können Sie diese Angaben auch im DaVinci-Explorer durch Aufruf der Eigenschaften einer Plandatei (rechte Maustaste und Eigenschaften) nachschauen.

2. Wechseln Sie zur Registerkarte `Protokollierung`. Hier können Sie optional die Protollierung an- bzw. ausschalten.

3. Tragen Sie unter `Pfad zur Logdatei` den Pfad zur Datei ein, in der alle Protokollierungsvermerke gespeichert werden sollen. Sie können zusätzlich bestimmen, welche Felder pro Anfrage protokolliert werden sollen.

4. Haben Sie alles konfiguriert, bestätigen Sie mit OK und starten Sie den Apache HTTP Server neu.

## Ein abschließender Test

Alles ist installiert und konfiguriert. Der folgende Test soll uns bestätigen, dass wir nichts übersehen haben:

* Öffnen Sie Ihren Web-Browser und tippen Sie folgende URL ein:

```txt
http://localhost/davinciIS.dll?type=class
```

Ihr Web-Browser sollte Ihnen nun eine Indexseite mit allen Klassen in Ihrem Web-Browser anzeigen. 


!!! info "Hinweis"

    Sollten Sie bereits den Benutzer `Webuser` eingerichtet und im DaVinci InfoServer Control hinterlegt haben, ist die Meldung `GeIndexPage: User access denied` ebenfalls korrekt und ein Zeichen für einen funktionierenden DaVinci InfoServer.

## Den DaVinci InfoServer aktualisieren

Möchten Sie eine neue Version des DaVinci InfoServer einspielen, gehen Sie wie folgt vor:

1. Stoppen Sie den IIS-Web-Server.

2. Führen Sie die Installation mit einem aktuelleren Installationspaket des DaVinci INFOSERVERS erneut aus. Das Setup ersetzt dabei automatisch Ihre bisherigen DaVinci InfoServer Dateien.

3. Starten Sie den Apache IIS-Web-Server neu.

4. Testen Sie mit Ihrem Web-Browser, ob der DaVinci InfoServer wie erwartet reagiert (siehe vorherigen Abschnnitt)

[1]:/assets/images/is/iis-win10-add-module.png
[2]:/assets/images/is/iis-win10-add-module-limitations.png
[3]:/assets/images/is/iis-win10-32bit.png
[4]:/assets/images/is/davinciis-first-test.png
 [5]:/assets/images/is/server-verbindung.jpg
