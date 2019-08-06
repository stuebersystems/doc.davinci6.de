# Der IIS 10 Web-Server

Die Internetinformationsdienste 10 (kurz IIS 10) sind Bestandteil von Windows 2016 (und Windows 10). Sie stellen u.a. einen vollständigen Web-Server bereit.

Dieses Kapitel beschreibt die Grundinstallation des IIS-Web-Servers. Diese Grundinstallation ist Voraussetzung für alle weiteren Installations- oder Konfigurationsschritte (z.B. Installation des DAVINCI INFOSERVERS, Installation der DAVINCI WEBBOX).

## Installation

Gehen Sie wie folgt vor:

1. Öffnen Sie in der Windows-Systemsteuerung den Punkt `Windows-Features aktivieren oder deaktivieren`. Ein Dialogfenster "Assistent zum Hinzufügen von Rollen und Features" öffnet sich automatisch, wenn nicht wählen Sie `2. Rollen und Features hinzufügen` aus dem Menü "Schnellstart".

2. Wählen Sie `Weiter`, anschließend wählen Sie `Rollenbasierte oder featurebasierte Installation` und `Weiter`. Wählen Sie die Checkbox `Einen Server aus dem Serverpool auswählen` und wählen Sie Ihren Server aus dem Serverpool aus. Wählen Sie 'Weiter', um fortzufahren.

3. Nun wählen Sie den Dienst "Webserver (IIS)" aus. Wenn ein Dialogfenster mit der Aufforderung "Sollen für Webserver (IIS) erforderlichen Features hinzufügt werden" erscheint, wählen Sie einfach `Features hinzufügen`, anschließend wählen Sie `Weiter`. Unter `Features auswählen` klicken Sie einfach `Weiter` und nocheinmal `Weiter` unter `Rolle Webserver (IIS)`.

4. Überprüfen Sie, ob folgende Features installiert sind:

   * Webserver / Allgemeine HTTP-Features / Statischer Inhalt
   * Webserver / Anwendungsentwicklung / ISAPI-Erweiterungen
   * Webserver / Sicherheit / Anforderungsfilterung  

![Internetinformationsdienste als Windows-Feature](/assets/images/IIS8-Windows-Features.png)

5. Zum Schluss wählen Sie `Weiter`, anschließend `Installieren`.

## Testen

Der IIS-Web-Server ist nun installiert. Probieren Sie ihn aus:

* Öffnen Sie Ihren Web-Browser auf dem gleichen Computer, auf dem Sie soeben den IIS-Web-Server installiert haben und tippen Sie `http://localhost` ein. Wenn die folgende Seite in Ihrem Browser erscheint, haben Sie alles richtig gemacht:

  ![IIS 10-Standardwebseite](/assets/images/iis-10-test.png)

Wenn die Seite nicht erscheint, kann ein Neustart des Rechners notwendig sein.

Bis jetzt hat sich alles nur auf dem Computer abgespielt, auf dem Sie den IIS-Web-Server installiert haben. Sinn und Zweck der ganzen Arbeit ist es jedoch, dass Ihr Web-Server im Netzwerk erreichbar ist. Daher sollten Sie auch den Zugriff von einem entfernten Computer aus testen:

1. Klären Sie zunächst ab, unter welcher IP-Adresse der Computer mit der IIS-Installation in Ihrem  Netzwerk zu erreichen ist. Eine von vielen Möglichkeiten ist die folgende:

   * Starten Sie die Windows-Kommandozeile `cmd`.
   * Tippen Sie den Befehl `ipconfig` ein und drücken Sie die Eingabetaste.
   * Lesen Sie die angezeigte IP-Adresse ab. 

2. Öffnen Sie nun einen Web-Browser auf einem anderen Computer in Ihrem Netzwerk und tippen Sie `http://<Ihre IP-Adresse>` (also z.B. `http://172.1.1.1`) ein. Es sollte wieder die Standardwebseite des IIS erscheinen.

Waren alle Tests positiv, haben Sie einen einsatzbereiten IIS-Web-Server in Ihrem Netzwerk laufen.

Möchten Sie, dass Ihr Web-Server auch im Internet, also auch außerhalb Ihres lokalen Netzwerk, erreichbar ist, müssen Sie noch ein paar weitere Details beachten. Das Kapitel [Tipps zum Einrichten Ihres Netzwerks] gibt Ihnen dazu nützliche Hinweise.

## Firewall-Einstellung

Falls Ihr Web-Server im Netzwerk nicht erreichbar ist, prüfen Sie, ob die eingehenden Regeln in Windows-Firewall aktiviert wurden:

1. Drücken die Tasten `Win` + `R` zusammen und geben Sie **wf.msc** ein, anschließend klicken Sie `OK`.  

2. Wählen Sie die Option `Eingehende Regeln` aus der linken Seite.  

3. Wählen Sie die Regeln "WWW-Dienste (Eingehender HTTP-Datenverkehr)" und falls gewünscht "WWW-Dienste (Eingehender HTTPS-Datenverkehr)" aus und aktivieren Sie sie per Rechts-Klick.

![Eingehende Regeln  &quot;WWW-Dienste (Eingehender HTTP-Datenverkehr)&quot; aktivieren](/assets/images/Eingehende-Regeln-IIS.png)

[Tipps zum Einrichten Ihres Netzwerks]: ../network-configuration.md
