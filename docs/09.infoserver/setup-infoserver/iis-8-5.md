# DAVINCI INFOSERVER und IIS 8.5

Dieses Kapitel beschreibt die Installation und Konfiguration des DAVINCI INFOSERVER als ISAPI-Modul für Ihren IIS-Web-Server.

!!! info "Hinweis"

  Internet Server API (ISAPI) ist eine Programmierschnittstelle von Microsoft, die sowohl von den Microsoft Internetinformationsdiensten (IIS) wie auch vom Apache Web-Server unterstützt werden. ISAPI-Module erweiteren die Standardfunktionalität von Web-Servern.

## Installation des DAVINCI INFOSERVER

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite `http://download.davinci.stueber.de` in Ihrem Web-Browser.

2. Klicken Sie unterhalb von "DAVINCI-INFOSERVER" auf `Download`. Ihr Web-Browser lädt jetzt das Installationpaket `daVinci6Infoserver.msi` herunter.

3. Starten Sie das Installationpaket `daVinci6Infoserver.msi` durch Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Nach der Beendigung der Installation finden Sie in Ihrem DAVINCI-Verzeichnis einen neuen Unterordner mit Namen `ISAPI` und dort eine Datei namens `daVinciIS.dll`. Also z.B.

```
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

Dies ist der DAVINCI-INFOSERVER, eine DLL, die Sie nun Ihrem Web-Server als ISAPI-Erweiterung bekannt machen müssen.

## Konfiguration des IIS-Web-Servers

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Alle Apps > Windows-Verwaltungsprogramme > Internetinformationsdienste (IIS)-Manager`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DAVINCI-INFOSERVER installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `Handlerzuordnungen`. Die Ansicht "Handlerzuordnungen" öffnet sich.

4. Klicken Sie nun auf `Modulzuordnung hinzufügen` auf der rechten Seite unter `Aktionen`. Ein Dialogfenster öffnet sich.

5. Tragen Sie in diesem Dialogfenster unter "Anforderungspfad" `daVinciIS.dll` ein, wählen Sie unter "Modul" `IsapiModule` aus, tragen Sie unter "Ausführbare Datei (optional)" den kompletten Pfad zur DAVINCI-INFOSERVER-DLL ein, z.B.

```
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

6. Zu guter letzt vergeben Sie dieser Zuordnung noch einen aussagekräftigen Namen (z.B. `DAVINCI-INFOSERVER 6`)
  
![ "Modulzuordnung hinzufügen"](/assets/images/iis-win10-add-module.png)

7. Klicken Sie zusätzlich auf die Schaltfläche `Einschränkungen` und entfernen Sie die Markierung `Handler nur bei folgender Zuordnung aufrufen` auf der Registerkarte "Zuordnung".
  
![ "Einschränkungen der Modulzuordnung"](/assets/images/iis-win10-add-module-limitations.png)

* Bestätigen Sie beide Dialogfenster mit `OK`.

Sollten Sie eine 64-bit-Version von Windows einsetzen, müssen Sie zusätzlich noch folgende Einstellungen im IIS-Manager vornehmen:

1. Markieren Sie in der linken Navigation den Eintrag "Anwendungspool" und klicken Sie anschließend auf der rechten Seite unter "Aktionen" auf `Erweiterte Einstellungen`. Ein Dialogfenster öffnet sich.

2. Setzen Sie die Eigenschaft "32-Bit Anwendungen aktivieren" auf `True` und klicken Sie anschließend auf `OK`.

![ "32-Bit-Anwendungen aktivieren"](/assets/images/iis-win10-32bit.png)

## Ein erster Test

Unser DAVINCI INFOSERVER ist nun installiert, aber noch nicht konfiguriert. Wir haben ihm nämlich noch nicht gesagt, mit welchem DAVINCI SERVER er kommunizieren soll. Bevor wir dies tun, wollen wir aber zunächst einmal testen, ob der DAVINCI INFOSERVER überhaupt auf Anfragen reagiert.

1. Öffnen Sie Ihren Web-Browser und tippen Sie ein:

```
http://localhost/isapi/davinciis.dll
```

1. 2. Wenn Ihr Web-Browser nun folgende vom DAVINCI INFOSERVER generierte Meldung anzeigt, ist der DAVINCI INFOSERVER bereit auf Anfragen zu reagieren:
  
  ![Fehlerseite des DAVINCI INFOSERVERS](/assets/images/davinciis-first-test.png)

## Den DAVINCI INFOSERVER konfigurieren

Wie bereist erwähnt, ist der DAVINCI INFOSERVER nur ein Vermittler zwsischen einem Client wie z.B. dem Web-Browswer oder DAVINCI MOBILE und einem DAVINCI SERVER. Voraussetzung für einen sinnvollen Einsatz des DAVINCI INFOSERVERS ist also eine Installation des DAVINCI SERVERS in Ihrem Netzwerk.

Ist dies der Fall, können Sie den DAVINCI INFOSERVER konfigurieren:

1. Öffnen Sie die Windows-Systemsteuerung und klicken Sie auf `daVinci-Infoserver`. Ein Dialogfenster öffnet sich

2. Wechseln Sie auf die Registerkarte `Server-Verbindung` und tragen Sie dort die Verbindungsdaten zu Ihrem DAVINCI SERVER ein. Für die Kommunikation mit dem DAVINCI-SERVER ist ein Benutzerkonto mit entsprechenden Rechten notwendig. Verwenden Sie bitte als Benutzer Ihren zuvor definierten "Webuser" und das dazugehörige Passwort. Weitere Informationen zum Benutzer "Webuser" finden Sie im Kapitel "Benutzerverwaltung".

![Server-Verbindung](/assets/images/server-verbindung.jpg)

4. Der Pfad unter `Webseiten-Pfad` ist in der Regel bereits ausgefüllt und muss nicht geändert werden:

```txt
C:\ProgramData\Stueber Systems\daVinci 6 Infoserver
```

1. Wechseln Sie zur Registerkarte `Plandatei`. Hier tragen Sie den Namen der Datei, die Sie auf dem DAVINCI SERVER ansprechen wollen, sowie deren eindeutige GUID ein. In DAVINCI können Sie beide Angaben unter `Plan > Eigenschaften > Allgemein` einsehen, sobald Sie mit dem DAVINCI-SERVER verbunden sind und die Datei geöffnet haben. Alternativ können Sie diese Angaben auch im DAVINCI-EXPLORER durch Aufruf der Eigenschaften einer Plandatei (rechte Maustaste und Eigenschaften) nachschauen.

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

## Den DAVINCI INFOSERVER aktualisieren

Möchten Sie eine neue Version des DAVINCI INFOSERVER einspielen, gehen Sie wie folgt vor:

1. Stoppen Sie den IIS-Web-Server.

2. Führen Sie die Installation mit einem aktuelleren Installationspaket des DAVINCI INFOSERVERS erneut aus. Das Setup ersetzt dabei automatisch Ihre bisherigen DAVINCI INFOSERVER Dateien.

3. Starten Sie den Apache IIS-Web-Server neu.

4. Testen Sie mit Ihrem Web-Browser, ob der DAVINCI INFOSERVER wie erwartet reagiert (siehe vorherigen Abschnnitt)
