# DAVINCI-Installation als Terminalserver

Terminalserver stellen innerhalb Ihres Netzwerks sogenannte Terminals bereit. Das sind Sitzungen, die der Nutzer per Remotezugriff auf dem Terminalserver öffnet.
Jeder Nutzer hat dabei seine eigene Sitzung und arbeitet unbeeinflusst von anderen Nutzern, die sich auch am Server anmelden. Das System hat Vorteile (bspw. Updates müssen nur auf dem Terminalserver eingespielt werden) und Nachteile (bspw. Bildschirminhalte und Eingaben die per Internet übertragen werden, sind immer durch eine gewisse Latenz gekennzeichnet), die von den Schulen abgewägt werden müssen.

## Installation

Es ist möglich DAVINCI als Server-/Einzelplatzinstallation auf einem Terminalserver zu installieren und die Nutzer per Terminal darauf zugreifen zulassen.

## Updates

Soll DAVINCI aktualisiert werden, müsste das auf allen eingesetzten Rechnern, also auf dem DAVINCI Server Rechner und auf den DAVINCI Clients geschehen. Setzen Sie DAVINCI in einer Terminalserverumgebung ein, müsste nur der Terminalserver aktualisiert werden.

## Benutzerindividuelle Daten

Einige DAVINCI - Dateien siehe `Hilfe > Systeminformationen`im Programm sind standardmäßig je DAVINCI-Installation unter `C:\ProgramData\Stueber Systems\DAVINCI` gespeichert, existieren also eigentlich je DAVINCI-Client. Arbeiten die Nutzer in einer Terminal-Server-Umgebung, muss beim Konfigurieren beachtet werden, dass diese Daten oder die `DAVINCI.paths` je Nutzer individuell geladen werden können.

!!! tipp "Hinweis!"

    Es ist zusätzlich möglich diese Dateien auch von einer selbstvorgegebenen zentralen Stelle zu laden, die Information wird aus der `DAVINCI.paths` ausgelesen. Eine Anleitung zum Einsatz einer DAVINCI.paths beschreiben wir [hier](https://doc.davinci6.stueber.de/00.allgemein/pathdatei/).
