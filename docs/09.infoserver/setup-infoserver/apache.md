# DaVinci InfoServer und Apache

Dieses Kapitel beschreibt die Installation und Konfiguration des DaVinci InfoServer als ISAPI-Modul für Ihren Apache HTTP Server.

!!! info "Hinweis"

    Internet Server API (ISAPI) ist eine Programmierschnittstelle von Microsoft, die sowohl von den Microsoft Internetinformationsdiensten (IIS) wie auch vom Apache Web-Server unterstützt werden. ISAPI-Module erweiteren die Standardfunktionalität von Web-Servern.

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
3. Starten Sie das das Installationpaket `daVinci6Infoserver.msi` durch Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Nach der Beendigung der Installation finden Sie in Ihrem DaVinci-Verzeichnis einen neuen Unterordner mit Namen `ISAPI` und dort eine Datei namens `daVinciIS.dll`. Also z.B.

```txt
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

Dies ist der DaVinci-InfoServer, eine DLL, die Sie nun Ihrem Web-Server als ISAPI-Erweiterung bekannt machen müssen.

## Konfiguration des Apache HTTP Servers

Zunächst muss dem Apache HTTP Server beigebracht werden, dass er ISAPI-Erweiterungen auch also solche erkennt und richtig verarbeitet:

1. Öffnen Sie die Apache-Konfigurationsdatei `httpd.conf` in einem Texteditor.
2. Fügen Sie einen neuen Abschnitt `Directory` ein:

```conf
<Directory "C:/Program Files (x86)/Stueber Systems/daVinci 6/ISAPI/">
    AddHandler isapi-handler .dll
    Options ExecCGI
    AllowOverride None
    Require all granted
</Directory>
```

Die Pfadangabe entspricht dem Installationpfad des DaVinci INFOSERVERS. Sollten Sie diesen unter einem anderem Pfad installiert haben, müssen Sie die Pfadangabe entsprechend korrigieren.

1. Fügen Sie eine neue Zeile mit dem Schlüsselwort `ScriptAliasMatch` ein

```script
ScriptAliasMatch "(?i)^/davinciis.dll" "C:/Program Files (x86)/Stueber Systems/daVinci 6/ISAPI/daVinciIS.dll"
```

Diese Angabe definiert, unter welcher URL der DaVinci InfoServer erreichbar ist. In diesem Fall wäre dies die URL:

```txt
http://localhost/davinciis.dll
```

Die etwas kryptische Angabe `(?i)^/davinciis.dll` ist ein regulärer Ausdruck und bedeutet, dass man `davinciis.dll` unabhängig von der Groß- und Kleinschreibung eingeben kann. Die folgenden URLs sind also alle gültig:

```txt
http://localhost/davinciis.dll
http://localhost/davinciis.DLL
http://localhost/daVinciIS.dll
```

1. Speichern Sie die Textdatei und starten Sie den Apache HTTP Server neu.

!!! info "Hinweis"

    Bitte beachten Sie, dass Pfadangaben unter Apache immer mit einem `/`definiert werden und nicht mit einem `\`. Dies liegt in der Linux-Herkunft des Apache-Projekts begründet.

## Ein erster Test

Unser DaVinci InfoServer ist nun installiert, aber noch nicht konfiguriert. Wir haben ihm nämlich noch nicht gesagt, mit welchem DaVinci Server er kommunizieren soll. Bevor wir dies tun, wollen wir aber zunächst  einmal testen, ob der DaVinci InfoServer überhaupt auf Anfragen reagiert.

1. Öffnen Sie Ihren Web-Browser und tippen Sie ein:

```txt
http://localhost/davinciis.dll
```

1. Wenn Ihr Web-Browser nun folgende vom DaVinci InfoServer generierte Meldung anzeigt, ist der DaVinci InfoServer bereit auf Anfragen zu reagieren:

[![Fehlerseite des DaVinci INFOSERVERS][2]][2] 

## Den DaVinci InfoServer konfigurieren

Wie bereits erwähnt, ist der DaVinci InfoServer nur ein Vermittler zwischen einem CLient wie z.B. der Web-Browswer oder DaVinci Mobile und einem DaVinci Server. Voraussetzung für einen sinnvollen Einsatz des DaVinci INFOSERVERS ist also eine Installation des DaVinci SERVERS in Ihrem Netzwerk.

Ist dies der Fall, können Sie den DaVinci InfoServer konfigurieren:

1. Öffnen Sie die Windows-Systemsteuerung und klicken Sie auf `daVinci-InfoServer`. Ein Dialogfenster öffnet sich.

2. Wechseln Sie auf die Registerkarte `Server-Verbindung` und tragen Sie dort die Verbindungsdaten zu Ihrem DaVinci Server ein. Für die Kommunikation mit dem DaVinci-Server ist ein Benutzerkonto mit entsprechenden Rechten notwendig. Verwenden Sie bitte als Benutzer Ihren zuvor definierten "Webuser" und das dazugehörige Passwort. Weitere Informationen zum Benutzer "Webuser" finden Sie im Kapitel "Benutzerverwaltung".

[![Server-Verbindung][3]][3] 

3. Der Pfad unter `Webseiten-Pfad` ist in der Regel bereits ausgefüllt und muss nicht geändert werden:

```txt
c:\ProgramData\Stueber Systems\daVinci 6 InfoServer
```

1. Wechseln Sie zur Registerkarte `Plandatei`. Hier tragen Sie den Namen der Datei, die Sie auf dem DaVinci Server ansprechen wollen, sowie deren eindeutige GUID ein. In DaVinci können Sie beide Angaben unter `Plan > Eigenschaften > Allgemein` einsehen, sobald Sie mit dem DaVinci-Server verbunden sind und die Datei geöffnet haben. Alternativ können Sie diese Angaben auch im DaVinci-Explorer durch Aufruf der Eigenschaften einer Plandatei (rechte Maustaste und Eigenschaften) nachschauen.

2. Wechseln Sie zur Registerkarte `Protokollierung`. Hier können Sie òptional die Protollierung an- bzw. auszuschalten.

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

## Übertragungsgeschwindigkeit steigern

Je nach Schulart kann die Menge der übertragene Menge an Daten recht unterschiedlich ausfallen. Infolgedessen kann die Ladezeit bis zur Anzeige in der WebBox oder in der App DaVinci Mobile auch in einer Berufsschule deutlich mehr Zeit in Anspruch nehmen, als die Ladezeit für die Daten einer Grundschule.

Um die Ladezeiten möglichst kurz zu halten, kann man einen Parameter aktivieren, der das Datenpaket vor der Übergabe komprimiert.

Um diesen Parameter zu aktivieren, öffnen Sie auf dem Rechner, auf dem Ihr DaVinci InfoServer läuft bitte den Pfad:

`C:\ProgramData\Stueber Systems\daVinci 6 InfoServer`

Sie finden in diesem Verzeichnis die Datei `daVinciInfoServerConfig.xml`.

[![daVinciInfoServerConfig.xml][4]][4] 

Öffnen Sie diese Datei bitte nicht per Doppelklick, sondern über `Rechtsklick > Öffnen mit > Editor`. Passen Sie den Wert für den Tag "CompressionEnabled" von 0 (deaktiviert) auf 1 (aktiviert) an.
Starten Sie anschließend den Webserver bitte einmal neu.

[![Wechseln Sie zum Tag "CompressionEnabled"][5]][5] 

[1]:/assets/images/is/islizenz.png
[2]:/assets/images/is/davinciis-first-test.png
[3]:/assets/images/is/server-verbindung.jpg
[4]:/assets/images/is/infoserver.config.png
[5]:/assets/images/is/infoserver.config01.png