# DaVinci InfoServer und IIS 7.5

Dieses Kapitel beschreibt die Installation und Konfiguration des DaVinci InfoServer als ISAPI-Modul für Ihren IIS-Web-Server.

!!! info "Hinweis"

    Internet Server API (ISAPI) ist eine Programmierschnittstelle von Microsoft, die sowohl von den Microsoft Internetinformationsdiensten (IIS) wie auch vom Apache Web-Server unterstützt werden. ISAPI-Module erweiteren die Standardfunktionalität von Web-Servern.

Voraussetzung für den Einsatz von DaVinci InfoServer ist eine vorhandene IIS 7.5 Instanz. Details zur Installation Konfiguration von IIS 7.5 finden Sie [hier](/09.infoserver/setup-webserver/iis-7-5.md).

## Lizenzierung

Der DaVinci InfoServer arbeitet mit Daten, die er vom DaVinci Server erhält. Die Installation und Konfiguration von DaVinci und DaVinci Enterprise sind Voraussetzung.

Damit der DaVinci Server Daten an den InfoServer übergibt, muss für den DaVinci Enterprise Server die entsprechende Lizenz importiert werden.
Gehen Sie wie folgt vor:

1. Öffnen Sie auf dem Rechner, auf dem Ihr DaVinci Server läuft bitte den Punkt ```Systemsteuerung > daVinci-Server (32 bit) > Karte "Dienst"```.
2. Unten links öffen Sie den Punkt "Lizenz" und importieren Ihre Lizenzdatei.

[![Bitte importieren Sie die Lizenz im DaVinci Enterprise Control][1]][1] 

## Installation des DaVinci InfoServer

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite `http://download.davinci.stueber.de` in Ihrem Web-Browser.

2. Klicken Sie unterhalb von "DaVinci-InfoServer" auf `Download`. Ihr Web-Browser lädt jetzt das Installationpaket `daVinci6Infoserver.msi` herunter.

3. Starten Sie das Installationpaket `daVinci6Infoserver.msi` durch Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Nach der Beendigung der Installation finden Sie in Ihrem DaVinci-Verzeichnis einen neuen Unterordner mit Namen `ISAPI` und dort eine Datei namens `daVinciIS.dll`. Also z.B.

```txt
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

Dies ist der DaVinci-InfoServer, eine DLL, die Sie nun Ihrem Web-Server als ISAPI-Erweiterung bekannt machen müssen.

## Konfiguration des IIS-Web-Servers

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Systemsteuerung > Verwaltung > Internetinformationsdienste (IIS)-Manager`. Alternativ können Sie auch das Dialogfenster "Ausführen" durch der Tastenkombination Windows-Taste und [R] öffnen. Geben Sie dort unter "Öffnen" den Befehl **inetmgr** ein, und klicken Sie auf `OK`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DaVinci-InfoServer installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `Handlerzuordnungen`. Die Ansicht "Handlerzuordnungen" öffnet sich.

4. Klicken Sie nun auf `Modulzuordnung hinzufügen` auf der rechten Seite unter `Aktionen`. Ein Dialogfenster öffnet sich.

5. Tragen Sie in diesem Dialogfenster unter "Anforderungspfad" `daVinciIS.dll` ein, wählen Sie unter "Modul" `IsapiModule` aus, tragen Sie unter "Ausführbare Datei (optional)" den kompletten Pfad zur DaVinci-InfoServer-DLL ein, z.B.
   
```txt
   C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

6. Zu guter letzt vergeben Sie dieser Zuordnung noch einen aussagekräftigen Namen (z.B. `DaVinci-InfoServer 6`)

[![Modulzuordnung hinzufügen][2]][2] 

7. Klicken Sie zusätzlich auf die Schaltfläche `Einschränkungen` und entfernen Sie die Markierung `Händler nur bei folgender Zuordnung aufrufen` auf der Registerkarte "Zuordnung".

[!["Einschränkungen der Modulzuordnung"][3]][3] 

* Bestätigen Sie beide Dialogfenster mit `OK`.

## Verwenden Sie eine 64-bit-Version von Windows

Sollten Sie eine 64-bit-Version von Windows einsetzen, gibt es zwei Möglichkeiten.

### 1. Verwenden Sie den Webserver nur für den DaVinci InfoServer

Dann genügt die folgende Einstellung im IIS-Manager:

1. Markieren Sie in der linken Navigation den Eintrag "Anwendungspool", wählen Sie in der mittleren Navigation Ihren Anwendungspool aus. Standardmäßig ist dies der Eintrag "DefaultAppPool". Klicken Sie anschließend auf der rechten Seite unter "Aktionen" auf `Erweiterte Einstellungen`. Ein Dialogfenster öffnet sich.

2. Setzen Sie die Eigenschaft "32-Bit Anwendungen aktivieren" auf `True` und klicken Sie anschließend auf `OK`.

[!["32-Bit-Anwendungen aktivieren"][4]][4] 

### 2. Andere Anwendungen nutzen parallel den Webserver

Seit der Version DaVinci 6.5.11 wird bei der DaVinci InfoServer-Installation ein zweites ISAPI-Verzeichnis (ISAPI64) mit angelegt. In dem Verzeichnis befindet sich eine 64-bit-fähige daVinciIS.dll, auf die Sie verweisen können.

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Alle Apps > Windows-Verwaltungsprogramme > Internetinformationsdienste (IIS)-Manager`. Alternativ können Sie auch das Dialogfenster "Ausführen" durch der Tastenkombination Windows-Taste und [R] öffnen. Geben Sie dort unter "Öffnen" den Befehl **inetmgr** ein, und klicken Sie auf `OK`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DaVinci-InfoServer installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `Handlerzuordnungen`. Die Ansicht "Handlerzuordnungen" öffnet sich.

4. Doppelklicken Sie nun auf die von Ihnen erstellte `Modulzuordnung` auf der linken Seite standardmäßig heißt sie "DaVinci-InfoServer 6". Das Dialogfenster öffnet sich.

5. Ändern Sie unter "Ausführbare Datei" den Pfad zur DaVinci-InfoServer-DLL das Verzeichnis ISAPI64 und die darin enthaltene Datei "daVinciIS.dll" ab.

```txt
   ...\Stueber Systems\daVinci 6\ISAPI64\daVinciIS.dll
```
[![Verweisen Sie auf die Datei unter ```... > Stueber Systems > daVinci 6 > ISAPI64```][5]][5] 

## Ein erster Test

Unser DaVinci InfoServer ist nun installiert, aber noch nicht konfiguriert. Wir haben ihm nämlich noch nicht gesagt, mit welchem DaVinci Server er kommunizieren soll. Bevor wir dies tun, wollen wir aber zunächst einmal testen, ob der DaVinci InfoServer überhaupt auf Anfragen reagiert.

1. Öffnen Sie Ihren Web-Browser und tippen Sie ein:

```txt
   http://localhost/davinciis.dll
```

2. Wenn Ihr Web-Browser nun folgende vom DaVinci InfoServer generierte Meldung anzeigt, ist der DaVinci InfoServer bereit auf Anfragen zu reagieren:

[![Fehlerseite des DaVinci INFOSERVERS][6]][6] 

## Den DaVinci InfoServer konfigurieren

Wie bereits erwähnt, ist der DaVinci InfoServer nur ein Vermittler zwischen einem Client wie z.B. dem Web-Browser oder DaVinci Mobile und einem DaVinci Server. Voraussetzung für einen sinnvollen Einsatz des DaVinci INFOSERVERS ist also eine Installation des DaVinci SERVERS in Ihrem Netzwerk. 

Ist dies der Fall, können Sie den DaVinci InfoServer konfigurieren:

1. Öffnen Sie die Windows-Systemsteuerung und klicken Sie auf `daVinci-InfoServer`. Ein Dialogfenster öffnet sich

2. Wechseln Sie auf die Registerkarte `Server-Verbindung` und tragen Sie dort die Verbindungsdaten zu Ihrem DaVinci Server ein. Für die Kommunikation mit dem DaVinci-Server ist ein Benutzerkonto mit entsprechenden Rechten notwendig. Verwenden Sie bitte als Benutzer Ihren zuvor definierten "Webuser" und das dazugehörige Passwort. Weitere Informationen zum Benutzer "Webuser" finden Sie im Kapitel "Benutzerverwaltung".

[!["Server-Verbindung"][7]][7] 

4. Der Pfad unter `Webseiten-Pfad` ist in der Regel bereits ausgefüllt und muss nicht geändert werden:

```txt
   c:\ProgramData\Stueber Systems\daVinci 6 InfoServer
```

5. Wechseln Sie zur Registerkarte `Plandatei`. Hier tragen Sie den Namen der Datei, die Sie auf dem DaVinci Server ansprechen wollen, sowie deren eindeutige GUID ein. In DaVinci können Sie beide Angaben unter `Plan > Eigenschaften > Allgemein` einsehen, sobald Sie mit dem DaVinci-Server verbunden sind und die Datei geöffnet haben. Alternativ können Sie diese Angaben auch im DaVinci-Explorer durch Aufruf der Eigenschaften einer Plandatei (rechte Maustaste und Eigenschaften) nachschauen.

6. Wechseln Sie zur Registerkarte `Protokollierung`. Hier können Sie optional die Protollierung an- bzw. ausschalten.

7. Tragen Sie unter `Pfad zur Logdatei` den Pfad zur Datei ein, in der alle Protokollierungsvermerke gespeichert werden sollen. Sie können zusätzlich bestimmen, welche Felder pro Anfrage protokolliert werden sollen.

8. Haben Sie alles konfiguriert, bestätigen Sie mit OK und starten Sie den Apache HTTP Server neu.

## Ein abschließender Test

Alles ist installiert und konfiguriert. Der folgende Test soll uns bestätigen, dass wir nichts übersehen haben:

* Öffnen Sie Ihren Web-Browser und tippen Sie folgende URL ein:
  
```
  http://localhost/davinciIS.dll?type=class
```
  
Ihr Web-Browser sollte Ihnen nun eine Indexseite mit allen Klassen in Ihrem Web-Browser anzeigen. 


!!! info "Hinweis"

    Sollten Sie bereits den Benutzer `Webuser` eingerichtet und im DaVinci InfoServer Control hinterlegt haben, ist die Meldung `GeIndexPage: User access denied` ebenfalls korrekt und ein Zeichen für einen funktionierenden DaVinci InfoServer.

## Die Übertragungsgeschwindigkeit steigern

Je nach Schulart kann die Menge der übertragene Menge an Daten recht unterschiedlich ausfallen. Infolgedessen kann die Ladezeit bis zur Anzeige in der WebBox oder in der App DaVinci Mobile auch in einer Berufsschule deutlich mehr Zeit in Anspruch nehmen, als die Ladezeit für die Daten einer Grundschule.

Um die Ladezeiten möglichst kurz zu halten, kann man einen Parameter aktivieren, der das Datenpaket vor der Übergabe komprimiert.

Um diesen Parameter zu aktivieren, öffnen Sie auf dem Rechner, auf dem Ihr DaVinci InfoServer läuft bitte den Pfad:

`C:\ProgramData\Stueber Systems\daVinci 6 InfoServer`

Sie finden in diesem Verzeichnis die Datei `daVinciInfoServerConfig.xml`.

[![daVinciInfoServerConfig.xml][8]][8] 

Öffnen Sie diese Datei bitte nicht per Doppelklick, sondern über `Rechtsklick > Öffnen mit > Editor`. Passen Sie den Wert für den Tag "CompressionEnabled" von 0 (deaktiviert) auf 1 (aktiviert) an.
Starten Sie anschließend den Webserver bitte einmal neu.

[![Wechseln Sie zum Tag "CompressionEnabled"][9]][9]

[1]:/assets/images/is/islizenz.png
[2]:/assets/images/is/iis-win75-add-module.png
[3]:/assets/images/is/iis-win75-add-module-limitations.png
[4]:/assets/images/is/iis-win10-32bit.png
[5]:/assets/images/is/_infoserver.dll.64.png
[6]:/assets/images/is/davinciis-first-test-ie.png
[7]:/assets/images/is/server-verbindung.jpg
[8]:/assets/images/is/infoserver.config.png
[9]:/assets/images/is/infoserver.config01.png