# Live-Daten im Internet

DAVINCI bietet Ihnen die folgenden Möglichkeiten, Ihre Plandaten publikumswirksam und ohne Zeitverzögerung via Internet auf Smart Phones, Tablets und Webseiten zur Verfügung zu stellen.

## 1. DAVINCI MOBILE

DAVINCI MOBILE ist eine App für die Betriebssysteme iOS und Android und setzt die Module DAVINCI ENTERPRISE (beinhaltet den DAVINCI SERVER) und DAVINCI INFOSERVER voraus.

DAVINCI MOBILE kommuniziert mit einem DAVINCI INFOSERVER. Dieser kommuniziert wiederum mit einem DAVINCI SERVER und liefert alle angeforderten Daten zurück an die App. Mit DAVINCI MOBILE bekommen Sie also stets Live-Daten angezeigt. Je nach dem welche Rechte Sie als Benutzer der App besitzen, bekommen Sie mehr oder weniger Daten angezeigt. Der Administrator vergibt die Rechte mit Hifle des DAVINCI EXPLORERS.

Voraussetzungen für den Einsatz von DAVINCI MOBILE:

1. [Installation eines Web-Servers](/09.infoserver/setup-webserver/README.md)
2. [Einrichten der Benutzer](/09.infoserver/user-management.md)
3. [Installation des DAVINCI INFOSERVERS](/09.infoserver/setup-infoserver/README.md)
4. [Installation von DAVINCI MOBILE auf Ihrem Mobilgerät](http://doc.davinci-app.stueber.de/)

!!! info "Hinweis"

    DAVINCI MOBILE kann von STÜBER SYSTEMS an Ihre Designvorgaben (Farben, Logo) angepasst und als eigene App für den jeweiligen App-Store vorbereitet werden. Bitte sprechen Sie uns dazu an.

## 2. DAVINCI WEBBOX

Die DAVINCI WEBBOX ist ein HTML5-basiertes Framework zur Live-Anzeige von DAVINCI-Stundenplänen und -Vertretungsplänen. DAVINCI-WEBBOX ist ein Open Source Projekt und kann in jede Webseite integriert werden.  

Die DAVINCI WEBBOX setzt die Module DAVINCI ENTERPRISE (beinhaltet den DAVINCI SERVER) und DAVINCI INFOSERVER voraus.

Die DAVINCI WEBBOX funktioniert ähnlich wie DAVINCI MOBILE und ist zum Einsatz auf Ihrer Webseite oder auf [E-Boards](http://eboard.stueber.de) gedacht. Für den Zugriff auf Ihrer Webseite kann sich der Benutzer bei Bedarf mit Kennung und Kennwort bei DAVINCI autorisieren. Der Zugriff erfolgt dann entsprechend der Benutzerrechte.  

Voraussetzungen für den Einsatz der DAVINCI WEBBOX:

1. [Installation eines Web-Servers](/09.infoserver/setup-webserver/README.md)
2. [Einrichten der Benutzer](/09.infoserver/user-management.md)
3. [Installation des DAVINCI INFOSERVERS](/09.infoserver/setup-infoserver/README.md)
4. [Installation der DAVINCI WEBBOX](/09.infoserver/setup-webbox/README.md)

!!! info "Hinweis"

    Über CSS-Dateien kann die DAVINCI-WEBBOX von Ihnen vollständig an Ihre Webdesign-Vorgaben angepasst werden. Wenn Sie es wünschen, führen wir die Anpassung an Ihr Corporate Design in Ihrem Auftrag durch.

## 3. Dynamische HTML-Seiten

!!! info "Hinweis"

    Im Gegensatz zur Nutzung der JSON-Daten für die DAVINCI-WEBBOX oder DAVINCI MOBILE erfolgt keine individuelle Benutzer-Autorisierung. **Wir empfehlen daher ausdrücklich den Einsatz der DAVINCI WEBBOX auf Ihren Webseiten.**

Mit Hilfe des DAVINCI INFOSERVERS können Sie auch ganz direkt dynamische Webseiten erzeugen. Diese Seiten werden vom DAVINCI SERVER zur Verfügung gestellt und können direkt in einem Web-Browser angezeigt werden. Sie müssen nichts weiter machen, also keine Daten nach jeder Planänderung exportieren. 

Das Erzeugen dynamischer HTML-Seiten setzt die Module DAVINCI ENTERPRISE (beinhaltet den DAVINCI SERVER) und DAVINC INFOSERVER voraus

Voraussetzungen für das Erzeugen dynamischer Webseiten:

1. [Installation eines Web-Servers](/09.infoserver/setup-webserver/allgemeines.md)
2. [Installation des DAVINCI INFOSERVERS](/09.infoserver/setup-infoserver/README.md)

!!! info "Hinweis"

    Im Gegensatz zur DAVINCI WEBBOX erfolgt hier keine individuelle Benutzer-Autorisierung. Wir empfehlen daher ausdrücklich den Einsatz der DAVINCI WEBBOX auf Ihren Webseiten.


## 4. E-Boards

Sie können den DAVINCI Vertretungsplan oder Stundenplan auf [E-Boards](http://eboard.stueber.de) in Ihrer Schule publizieren.

Durch die direkte Integration der DAVINCI WEBBOX in CONFIRE SHOWTIME ist die Umsetzung der Darstellung denkbar einfach.

## 5. Digitale Gebäudepläne

Sie können die Raumbelegungsdaten aus DAVINCI aufmerksamkeitswirksam in digitalen Gebäudeplänen verwenden. Der Gebäudeplan kann über über DAVINCI MOBILE auf Tablets oder per DAVINCI WEBBOX auf Ihrer Webseite angezeigt werden. Ein Beispiel finden Sie auf der [Webseite für Gebäudepläne](http://davinci.stueber.de/floorplan.php).
