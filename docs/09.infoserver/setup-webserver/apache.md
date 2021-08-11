# Der Apache HTTP Server

Der Apache HTTP Server ist ein quelloffener und freier Web-Server der Apache Software Foundation und gilt als der meistbenutzte Web-Server im Internet. Der große Vorteil des Apache HTTP Servers ist, dass dieser kostenlos ist und unter nahezu jeder Version von Windows installiert werden kann.

Dieses Kapitel beschreibt die Grundinstallation des Apache HTTP Server. Diese Grundinstallation ist Voraussetzung für alle weiteren Installations- oder Konfigurationsschritte (z.B. Installation des DAVINCI INFOSERVER, Intstallation der DAVINCI WEBBOX).

## Inhalte

* [Installation](#Installation)
* [Testen](#Testen)
* [Optionale Konfiguration](#Konfiguration)

## Installation{#Installation}

Es gibt verschiedene Möglichkeiten, den Apache HTTP Server zu installieren. Eine einfache und effektive Möglichkeit ist die Benutzung von XAMPP. XAMPP ist eine ebenfalls freie Software, die verschiedene Open-Source-Lösungen zu einem leicht zu konfigurierenden Paket zusammenfasst. Eine dieser Lösungen ist eben der Apache HTTP Server

!!! warning "Wichtig"

    Apache unterstützt ISAPI-Module nur in der 32-Bit-Version. Bei einer Installation von XAMPP daher unbedingt die 32-bit-Version benutzen.

Gehen Sie wie folgt vor:

1. Öffnen Sie die Webseite `https://www.apachefriends.org` und laden Sie sich das aktuelle 32-bit-Version des XAMPP-Setup herunter.

2. Starten Sie das Setup und beantworten Sie die Fragen des Assistenten 
  
[![XAMPP-Setup][1]][1] 

3. Für eine minimale Installation von Apache kreuzen Sie unter `Select Components` die folgenden Einträge an: 

[![Beschriftung][2]][2] 

4. Bei der Frage nach dem Installationsordner belassen Sie unter `Installation folder` die Vorgabeeinstellung. Die Installation im Programme-Verzeichis von Windows wird nicht empfohlen. 

[![XAMPP-Standardordner][3]][3] 

5. Nach Abschluss der Installation meldet sich unter Umständen die Windows-Firewall. Diese fragt Sie, ob der Apache HTTP Server Zugriff auf das Netzwerk bekommen soll. Bestätigen Sie dies bitte. 

[![Beschriftung][4]][4] 

6. Zu guter Letzt werden sie gefragt, ob Sie das XAMPP Control Panel starten möchten. Ja, das wollen wir. 

## Testen{#Testen}

Der Apache HTTP Server ist nun installiert. Starten Sie ihn und probieren Sie ihn aus:

1. Klicken Sie im XAMPP Control Panel in der ersten Zeile hinter `Apache` auf `Starten`. Der Apache HTTP Server wird nun gestartet.  

[![Beschriftung][5]][5] 

2. Öffnen Sie Ihren Web-Browser auf dem gleichen Computer, auf dem Sie soeben Apache installiert haben und tippen Sie `http://localhost` ein. Wenn die folgende Seite in Ihrem Browser erscheint, haben Sie alles richtig gemacht:  

[![Beschriftung][6]][6] 

Bis jetzt hat sich alles nur auf dem Computer abgespielt, auf dem Sie Apache installiert haben. Sinn und Zweck der ganzen Arbeit ist es jedoch, dass Ihr Web-Server im Netzwerk erreichbar ist. Daher sollten Sie auch den Zugriff von einem entfernten Computer aus testen:

1. Klären Sie zunächst ab, unter welcher IP-Adresse der Computer mit der Apache-Installation in Ihrem  Netzwerk zu erreichen ist. Eine von vielen Möglichkeiten ist die folgende:
 
  * Starten Sie die Windows-Kommandozeile
  * Tippen Sie den Befehl `ipconfig` ein und drücken Sie die Eingabetaste.
  * Lesen Sie die angezeigte IP-Adresse ab. 

2. Öffnen Sie nun einen Web-Browser auf einem anderen Computer in Ihrem Netzwerk und tippen Sie `http://<Ihre IP-Adresse>` (also z.B. `http://172.1.1.1`) ein. Es sollte wieder die Standardwebseite des Apache HTTP Servers erscheinen.

Waren alle Tests positiv, haben Sie einen einsatzbereiten Apache HTTP Server in Ihrem Netzwerk laufen. 

Möchten Sie, dass Ihr Web-Server auch im Internet, also auch außerhalb Ihres lokalen Netzwerk, erreichbar ist, müssen Sie noch ein paar weitere Details beachten. Das Kapitel [Tipps zum Einrichten Ihres Netzwerks] gibt Ihnen dazu nützliche Hinweise.

## Optionale Konfiguration

Möchten Sie die Standardeinstellungen Ihres Apache ändern, so müssen Sie die Datei `httpd.conf` in einem Texteditor öffnenn und editieren. Bei einer Standardinstallation mit XAMPP befindet sich die Datei im folgenden Verzeichnius:

```
C:\xampp\apache\conf\httpd.conf 
```

Ein typisches Beispiel für eine Konfigurierung ist die Änderung der Port-Nummer. Standardmäßig horcht der Apache HTTP Server auf den Port 80. Dies ist der Stanardport für das HTTP-Protokoll. Wenn Sie parallel auf dem gleichen Computer auch den IIS als Web-Server laufen lassen, kann dies zu Konflikten führen. Beide Web-Server können nicht auf den gleichen Port reagieren. In diesem Fall könnten Sie für den Apache HTTP Server einen anderen Port vergeben:

1. Öffnen Sie die Datei `httpd.conf`. 

2. Suchen Sie den folgenden Abschnitt
```
#
# Listen: Allows you to bind Apache to specific IP addresses and/or
# ports, instead of the default. See also the <VirtualHost>
# directive.
#
# Change this to Listen on specific IP addresses as shown below to 
# prevent Apache from glomming onto all bound IP addresses.
#
#Listen 12.34.56.78:80
Listen 80
```

3. Vergeben Sie eine neue Portnummer, beispielsweise 8888.
```
#
# Listen: Allows you to bind Apache to specific IP addresses and/or
# ports, instead of the default. See also the <VirtualHost>
# directive.
#
# Change this to Listen on specific IP addresses as shown below to 
# prevent Apache from glomming onto all bound IP addresses.
#
#Listen 12.34.56.78:80
Listen 8888
```

4. Speichern Sie die Datei in Ihrem Texteditor.

5. Starten Sie das XAMPP Control Panel und starten Sie dort den Apache HTTP Server neu, damit dieser Ihre Änderung berücksichtigen kann.

6. Wenn Sie jetzt in Ihrem Web-Browser `http:\\localhost:8888` eintippen, sollte Ihnen wieder die Standardwebseite des Apache HTTP Servers erscheinen.

## Firewall-Einstellung

Falls Ihr Web-Server im Netzwerk nicht erreichbar ist, prüfen Sie, ob die eingehenden Regeln in Windows-Firewall aktiviert wurden:
1. Drücken die Tasten `Win` + `R` zusammen und geben Sie **wf.msc** ein, anschließend klicken Sie `OK`.
2. Wählen Sie die Option `Eingehende Regeln` aus der linken Seite.
3. Wählen Sie die Regeln "Apache HTTP Server" aus und aktivieren Sie sie per Rechts-Klick.

[![Eingehende Regeln  "Apache HTTP Server" aktivieren][7]][7] 

[Tipps zum Einrichten Ihres Netzwerks]: ../network-configuration.md

[1]:/assets/images/is/xampp-installer.png
[2]:/assets/images/is/xampp-installer-minimal.png
[3]:/assets/images/is/xampp-installer-folder.png
[4]:/assets/images/is/xampp-installer-firewall.png
[5]:/assets/images/is/xampp-control-panel.png
[6]:/assets/images/is/apache-test.png
[7]:/assets/images/is/Eingehende-Regeln-Apache.png
