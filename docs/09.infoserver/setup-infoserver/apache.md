# DAVINCI INFOSERVER und Apache

Dieses Kapitel beschreibt die Installation und Konfiguration des DAVINCI INFOSERVER als ISAPI-Modul für Ihren Apache HTTP Server.

!!! info "Hinweis"

    Internet Server API (ISAPI) ist eine Programmierschnittstelle von Microsoft, die sowohl von den Microsoft Internetinformationsdiensten (IIS) wie auch vom Apache Web-Server unterstützt werden. ISAPI-Module erweiteren die Standardfunktionalität von Web-Servern.

## Lizenzierung

Der DAVINCI INFOSERVER arbeitet mit Daten, die er vom DAVINCI Server erhält. Die Installation und Konfiguration von DAVINCI und DAVINCI ENTERPRISE sind Voraussetzung.

Damit der DAVINCI Server Daten an den INFOSERVER übergibt, muss für den DAVINCI ENTERPRISE SERVER die entsprechende Lizenz importiert werden.
Gehen Sie wie folgt vor:

1. Öffnen Sie auf dem Rechner, auf dem Ihr DAVINCI Server läuft bitte den Punkt ```Systemsteuerung > daVinci-Server (32 bit) > Karte "Dienst"```. 
2. Unten links öffen Sie den Punkt "Lizenz" und importieren Ihre Lizenzdatei.

[![Bitte importieren Sie die Lizenz im DAVINCI ENTERPRISE Control][1]][1] 

## Installation des DAVINCI INFOSERVER

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite `http://download.davinci.stueber.de` in Ihrem Web-Browser.
2. Klicken Sie unterhalb von "DAVINCI-INFOSERVER" auf `Download`. Ihr Web-Browser lädt jetzt das Installationpaket `daVinci6Infoserver.msi` herunter.
3. Starten Sie das das Installationpaket `daVinci6Infoserver.msi` durch Doppelklick und folgen Sie den Anweisungen des Installationsprogramms.

Nach der Beendigung der Installation finden Sie in Ihrem DAVINCI-Verzeichnis einen neuen Unterordner mit Namen `ISAPI` und dort eine Datei namens `daVinciIS.dll`. Also z.B.

```txt
C:\Program Files (x86)\Stueber Systems\daVinci 6\ISAPI\daVinciIS.dll
```

Dies ist der DAVINCI-INFOSERVER, eine DLL, die Sie nun Ihrem Web-Server als ISAPI-Erweiterung bekannt machen müssen.

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

Die Pfadangabe entspricht dem Installationpfad des DAVINCI INFOSERVERS. Sollten Sie diesen unter einem anderem Pfad installiert haben, müssen Sie die Pfadangabe entsprechend korrigieren.

1. Fügen Sie eine neue Zeile mit dem Schlüsselwort `ScriptAliasMatch` ein

```script
ScriptAliasMatch "(?i)^/davinciis.dll" "C:/Program Files (x86)/Stueber Systems/daVinci 6/ISAPI/daVinciIS.dll"
```

Diese Angabe definiert, unter welcher URL der DAVINCI INFOSERVER erreichbar ist. In diesem Fall wäre dies die URL:

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

Unser DAVINCI INFOSERVER ist nun installiert, aber noch nicht konfiguriert. Wir haben ihm nämlich noch nicht gesagt, mit welchem DAVINCI SERVER er kommunizieren soll. Bevor wir dies tun, wollen wir aber zunächst  einmal testen, ob der DAVINCI INFOSERVER überhaupt auf Anfragen reagiert.

1. Öffnen Sie Ihren Web-Browser und tippen Sie ein:

```txt
http://localhost/davinciis.dll
```

1. Wenn Ihr Web-Browser nun folgende vom DAVINCI INFOSERVER generierte Meldung anzeigt, ist der DAVINCI INFOSERVER bereit auf Anfragen zu reagieren:

[![Fehlerseite des DAVINCI INFOSERVERS][2]][2] 

## Den DAVINCI INFOSERVER konfigurieren

Wie bereits erwähnt, ist der DAVINCI INFOSERVER nur ein Vermittler zwischen einem CLient wie z.B. der Web-Browswer oder DAVINCI MOBILE und einem DAVINCI SERVER. Voraussetzung für einen sinnvollen Einsatz des DAVINCI INFOSERVERS ist also eine Installation des DAVINCI SERVERS in Ihrem Netzwerk.

Ist dies der Fall, können Sie den DAVINCI INFOSERVER konfigurieren:

1. Öffnen Sie die Windows-Systemsteuerung und klicken Sie auf `daVinci-Infoserver`. Ein Dialogfenster öffnet sich.

2. Wechseln Sie auf die Registerkarte `Server-Verbindung` und tragen Sie dort die Verbindungsdaten zu Ihrem DAVINCI SERVER ein. Für die Kommunikation mit dem DAVINCI-SERVER ist ein Benutzerkonto mit entsprechenden Rechten notwendig. Verwenden Sie bitte als Benutzer Ihren zuvor definierten "Webuser" und das dazugehörige Passwort. Weitere Informationen zum Benutzer "Webuser" finden Sie im Kapitel "Benutzerverwaltung".

[![Server-Verbindung][3]][3] 

3. Der Pfad unter `Webseiten-Pfad` ist in der Regel bereits ausgefüllt und muss nicht geändert werden:

```txt
c:\ProgramData\Stueber Systems\daVinci 6 Infoserver
```

1. Wechseln Sie zur Registerkarte `Plandatei`. Hier tragen Sie den Namen der Datei, die Sie auf dem DAVINCI SERVER ansprechen wollen, sowie deren eindeutige GUID ein. In DAVINCI können Sie beide Angaben unter `Plan > Eigenschaften > Allgemein` einsehen, sobald Sie mit dem DAVINCI-SERVER verbunden sind und die Datei geöffnet haben. Alternativ können Sie diese Angaben auch im DAVINCI-EXPLORER durch Aufruf der Eigenschaften einer Plandatei (rechte Maustaste und Eigenschaften) nachschauen.

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

    Sollten Sie bereits den Benutzer `Webuser` eingerichtet und im DAVINCI INFOSERVER Control hinterlegt haben, ist die Meldung `GeIndexPage: User access denied` ebenfalls korrekt und ein Zeichen für einen funktionierenden DAVINCI INFOSERVER.

## Übertragungsgeschwindigkeit steigern

Je nach Schulart kann die Menge der übertragene Menge an Daten recht unterschiedlich ausfallen. Infolgedessen kann die Ladezeit bis zur Anzeige in der WEBBOX oder in der App DAVINCI MOBILE auch in einer Berufsschule deutlich mehr Zeit in Anspruch nehmen, als die Ladezeit für die Daten einer Grundschule.

Um die Ladezeiten möglichst kurz zu halten, kann man einen Parameter aktivieren, der das Datenpaket vor der Übergabe komprimiert.

Um diesen Parameter zu aktivieren, öffnen Sie auf dem Rechner, auf dem Ihr DAVINCI INFOSERVER läuft bitte den Pfad:

`C:\ProgramData\Stueber Systems\daVinci 6 InfoServer`

Sie finden in diesem Verzeichnis die Datei `daVinciInfoServerConfig.xml`.

[![daVinciInfoServerConfig.xml][4]][4] 

Öffnen Sie diese Datei bitte nicht per Doppelklick, sondern über `Rechtsklick > Öffnen mit > Editor`. Passen Sie den Wert für den Tag "CompressionEnabled" von 0 (deaktiviert) auf 1 (aktiviert) an.
Starten Sie anschließend den Webserver bitte einmal neu.

[![Wechseln Sie zum Tag "CompressionEnabled"][5]][5] 

[1]:/assets/images/is/islizenz.png
[2]:/ssets/images/is/davinciis-first-test.png
[3]:/assets/images/is/server-verbindung.jpg
[4]:/assets/images/is/infoserver.config.png
[5]:/assets/images/is/infoserver.config01.png