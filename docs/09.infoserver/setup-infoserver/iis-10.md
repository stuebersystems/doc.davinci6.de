# DAVINCI INFOSERVER und IIS 10

Dieses Kapitel beschreibt die Installation und Konfiguration des DAVINCI INFOSERVER als ISAPI-Modul für Ihren IIS-Web-Server.

!!! info "Hinweis"

    Internet Server API (ISAPI) ist eine Programmierschnittstelle von Microsoft, die sowohl von den Microsoft Internetinformationsdiensten (IIS) wie auch vom Apache Web-Server unterstützt werden. ISAPI-Module erweiteren die Standardfunktionalität von Web-Servern.

Voraussetzung für den Einsatz von DAVINCI INFOSERVER ist eine vorhandene IIS 10 Instanz. Details zur Installation Konfiguration von IIS 10 finden Sie [hier](/09.infoserver/setup-webserver/iis-10.md).

## Lizenzierung

Der DAVINCI INFOSERVER arbeitet mit Daten, die er vom DAVINCI Server erhält. Die Installation und Konfiguration von DAVINCI und DAVINCI ENTERPRISE sind Voraussetzung.

Damit der DAVINCI Server Daten an den INFOSERVER übergibt, muss für den DAVINCI ENTERPRISE SERVER die entsprechende Lizenz importiert werden.  
Gehen Sie wie folgt vor:

1. Öffnen Sie auf dem Rechner, auf dem Ihr DAVINCI Server läuft bitte den Punkt `Systemsteuerung > daVinci-Server (32 bit) > Karte "Dienst"`. 
2. Unten links öffen Sie den Punkt "Lizenz" und importieren Ihre Lizenzdatei.

![Bitte importieren Sie die Lizenz im DAVINCI ENTERPRISE Control](/assets/images/islizenz.png)

## Installation des DAVINCI INFOSERVER

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite `http://download.davinci.stueber.de` in Ihrem Web-Browser.

2. Klicken Sie unterhalb von "DAVINCI-INFOSERVER" auf `Download`. Ihr Web-Browser lädt jetzt das Installationpaket `daVinci6Infoserver.msi` herunter.

3. Starten Sie das Installationpaket `daVinci6Infoserver.msi` durch Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Nach der Beendigung der Installation finden Sie in Ihrem DAVINCI-Verzeichnis einen neuen Unterordner mit Namen `ISAPI` und dort eine Datei namens `daVinciIS.dll`. Also z.B.

```txt
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

Dies ist der DAVINCI-INFOSERVER, eine DLL, die Sie nun Ihrem Web-Server als ISAPI-Erweiterung bekannt machen müssen.

## Konfiguration des IIS-Web-Servers

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Alle Apps > Windows-Verwaltungsprogramme > Internetinformationsdienste (IIS)-Manager`. Alternativ können Sie auch das Dialogfenster "Ausführen" durch der Tastenkombination Windows-Taste und \[R\] öffnen. Geben Sie dort unter "Öffnen" den Befehl **inetmgr** ein, und klicken Sie auf `OK`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DAVINCI-INFOSERVER installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `Handlerzuordnungen`. Die Ansicht "Handlerzuordnungen" öffnet sich.

4. Klicken Sie nun auf `Modulzuordnung hinzufügen` auf der rechten Seite unter `Aktionen`. Ein Dialogfenster öffnet sich.

5. Tragen Sie in diesem Dialogfenster unter "Anforderungspfad" `daVinciIS.dll` ein, wählen Sie unter "Modul" `IsapiModule` aus, tragen Sie unter "Ausführbare Datei (optional)" den kompletten Pfad zur DAVINCI-INFOSERVER-DLL ein, z.B.

```txt
   C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI64\daVinciIS.dll
```

!!! info "Hinweis"

    Bei 64-Bit-Betriebssystemen schauen Sie bitte diesen [Abschnitt](/09.infoserver/setup-infoserver/iis-10.md#verwenden-sie-eine-64-bit-version-von-windows) an!

1. Zu guter letzt vergeben Sie dieser Zuordnung noch einen aussagekräftigen Namen (z.B. `DAVINCI-INFOSERVER 6`)

![ "Modulzuordnung hinzufügen"](/assets/images/iis-win10-add-module.png)

7. Klicken Sie zusätzlich auf die Schaltfläche `Einschränkungen` und entfernen Sie die Markierung `Handler nur bei folgender Zuordnung aufrufen` auf der Registerkarte "Zuordnung".

![ "Einschränkungen der Modulzuordnung"](/assets/images/iis-win10-add-module-limitations.png)

8. Bestätigen Sie beide Dialogfenster mit `OK`.

## Verwenden Sie eine 64-bit-Version von Windows?

Sollten Sie eine 64-bit-Version von Windows einsetzen, gibt es zwei Möglichkeiten.

!!! info "Hinweis"

    Bitte verwenden Sie nur eine der nachstehenden Varianten!

### 1. Verwenden Sie den Webserver nur für den DAVINCI Infoserver?

Dann genügt die folgende Einstellung im IIS-Manager:

1. Markieren Sie in der linken Navigation den Eintrag "Anwendungspool", wählen Sie in der mittleren Navigation Ihren Anwendungspool aus. Standardmäßig ist dies der Eintrag "DefaultAppPool". Klicken Sie anschließend auf der rechten Seite unter "Aktionen" auf `Erweiterte Einstellungen`. Ein Dialogfenster öffnet sich.

2. Setzen Sie die Eigenschaft "32-Bit Anwendungen aktivieren" auf `True` und klicken Sie anschließend auf `OK`.

![ "32-Bit-Anwendungen aktivieren"](/assets/images/iis-win10-32bit.png)

### 2. Andere Anwendungen nutzen parallel den Webserver

Seit der Version DAVINCI 6.5.11 wird bei der DAVINCI Infoserver-Installation ein zweites ISAPI-Verzeichnis (ISAPI64) mit angelegt. In dem Verzeichnis befindet sich eine 64-bit-fähige daVinciIS.dll, auf die Sie verweisen können.

Gehen Sie wie folgt vor:

1. Starten Sie den IIS-Manager durch Klicken auf `Start > Alle Apps > Windows-Verwaltungsprogramme > Internetinformationsdienste (IIS)-Manager`. Alternativ können Sie auch das Dialogfenster "Ausführen" durch der Tastenkombination Windows-Taste und \[R\] öffnen. Geben Sie dort unter "Öffnen" den Befehl **inetmgr** ein, und klicken Sie auf `OK`.

2. Markieren Sie in der linken Navigation Ihre Webseite, in der Sie den DAVINCI-INFOSERVER installieren wollen. Standardmäßig ist dies der Eintrag "Default Web Site".

3. Auf der rechten Seite doppelklicken Sie auf das Symbol `Handlerzuordnungen`. Die Ansicht "Handlerzuordnungen" öffnet sich.

4. Doppelklicken Sie nun auf die von Ihnen erstellte `Modulzuordnung` auf der linken Seite standardmäßig heißt sie "DAVINCI-INFOSERVER 6". Das Dialogfenster öffnet sich.

5. Ändern Sie unter "Ausführbare Datei" den Pfad zur DAVINCI-INFOSERVER-DLL das Verzeichnis ISAPI64 und die darin enthaltene Datei "daVinciIS.dll" ab.

```
...\Stueber Systems\daVinci 6\ISAPI64\daVinciIS.dll
```

![Verweisen Sie auf die Datei unter ```... > Stueber Systems > daVinci 6 > ISAPI64```](/assets/images/_infoserver.dll.64.png)

## Ein erster Test

Unser DAVINCI INFOSERVER ist nun installiert, aber noch nicht konfiguriert. Wir haben ihm nämlich noch nicht gesagt, mit welchem DAVINCI SERVER er kommunizieren soll. Bevor wir dies tun, wollen wir aber zunächst einmal testen, ob der DAVINCI INFOSERVER überhaupt auf Anfragen reagiert.

1. Öffnen Sie Ihren Web-Browser und tippen Sie ein:

```
   http://localhost/davinciis.dll
```

2. Wenn Ihr Web-Browser nun folgende vom DAVINCI INFOSERVER generierte Meldung anzeigt, ist der DAVINCI INFOSERVER bereit auf Anfragen zu reagieren:

![Fehlerseite des DAVINCI INFOSERVERS](/assets/images/davinciis-first-test.png)

## Den DAVINCI INFOSERVER konfigurieren

Wie bereits erwähnt, ist der DAVINCI INFOSERVER nur ein Vermittler zwischen einem Client wie z.B. dem Web-Browser oder DAVINCI MOBILE und einem DAVINCI SERVER. Voraussetzung für einen sinnvollen Einsatz des DAVINCI INFOSERVERS ist also eine Installation des DAVINCI SERVERS in Ihrem Netzwerk.

Ist dies der Fall, können Sie den DAVINCI INFOSERVER konfigurieren:

1. Öffnen Sie die Windows-Systemsteuerung und klicken Sie auf `daVinci-Infoserver`. Ein Dialogfenster öffnet sich

2. Wechseln Sie auf die Registerkarte `Server-Verbindung` und tragen Sie dort die Verbindungsdaten zu Ihrem DAVINCI SERVER ein. Für die Kommunikation mit dem DAVINCI-SERVER ist ein Benutzerkonto mit entsprechenden Rechten notwendig. Verwenden Sie bitte als Benutzer Ihren zuvor definierten "Webuser" und das dazugehörige Passwort. Weitere Informationen zum Benutzer "Webuser" finden Sie im Kapitel "Benutzerverwaltung".

![ "Server-Verbindung"](/assets/images/server-verbindung.jpg)

3. Der Pfad unter `Webseiten-Pfad` ist in der Regel bereits ausgefüllt und muss nicht geändert werden:

```
   c:\ProgramData\Stueber Systems\daVinci 6 Infoserver
```

4. Wechseln Sie zur Registerkarte `Plandatei`. Hier tragen Sie den Namen der Datei, die Sie auf dem DAVINCI SERVER ansprechen wollen, sowie deren eindeutige GUID ein. In DAVINCI können Sie beide Angaben unter `Plan > Eigenschaften > Allgemein` einsehen, sobald Sie mit dem DAVINCI-SERVER verbunden sind und die Datei geöffnet haben. Alternativ können Sie diese Angaben auch im DAVINCI-EXPLORER durch Aufruf der Eigenschaften einer Plandatei (rechte Maustaste und Eigenschaften) nachschauen.

![ "Namen und GUID der Plandatei eintragen"](/assets/images/guid.png)

5. Wechseln Sie zur Registerkarte `Protokollierung`. Hier können Sie optional die Protollierung an- bzw. ausschalten.

6. Tragen Sie unter `Pfad zur Logdatei` den Pfad zur Datei ein, in der alle Protokollierungsvermerke gespeichert werden sollen. Sie können zusätzlich bestimmen, welche Felder pro Anfrage protokolliert werden sollen.

7. Haben Sie alles konfiguriert, bestätigen Sie mit OK und starten Sie den Apache HTTP Server neu.

## Ein abschließender Test

Alles ist installiert und konfiguriert. Der folgende Test soll uns bestätigen, dass wir nichts übersehen haben:

* Öffnen Sie Ihren Web-Browser und tippen Sie folgende URL ein:

```
http://localhost/davinciIS.dll?type=class
```

  Ihr Web-Browser sollte Ihnen nun eine Indexseite mit allen Klassen in Ihrem Web-Browser anzeigen.

## Die Übertragungsgeschwindigkeit steigern

Je nach Schulart kann die Menge der übertragene Menge an Daten recht unterschiedlich ausfallen. Infolgedessen kann die Ladezeit bis zur Anzeige in der WEBBOX oder in der App DAVINCI MOBILE auch in einer Berufsschule deutlich mehr Zeit in Anspruch nehmen, als die Ladezeit für die Daten einer Grundschule.

Um die Ladezeiten möglichst kurz zu halten, kann man einen Parameter aktivieren, der das Datenpaket vor der Übergabe komprimiert.

Um diesen Parameter zu aktivieren, öffnen Sie auf dem Rechner, auf dem Ihr DAVINCI INFOSERVER läuft bitte den Pfad:

`C:\ProgramData\Stueber Systems\daVinci 6 InfoServer`

Sie finden in diesem Verzeichnis die Datei `daVinciInfoServerConfig.xml`.

![daVinciInfoServerConfig.xml](/assets/images/infoserver.config.png)

Öffnen Sie diese Datei bitte nicht per Doppelklick, sondern über `Rechtsklick > Öffnen mit > Editor`. Passen Sie den Wert für den Tag "CompressionEnabled" von 0 (deaktiviert) auf 1 (aktiviert) an.
Starten Sie anschließend den Webserver bitte einmal neu.

![Wechseln Sie zum Tag "CompressionEnabled"](/assets/images/infoserver.config01.png)
