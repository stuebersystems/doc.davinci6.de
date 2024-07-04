# DAVINCI für mehrere Schulen auf einem Server

Situation: Die Installation von DAVINCI für mehrere Schulen soll auf einem gemeinsamen Server geschehen, somit soll der administrative Aufwand eingeschränkt und auch verlagert werden. 

Nachstehend beschreiben wir einige Punkte, die zu bedenken sind. 

**Sollten die nachstehenden Punkte dennoch Fragen offen lassen, können Sie uns für eine genauere Beratung beauftragen. Bitte wenden Sie sich für ein Angebot an unsere Office-Team unter `office@stueber.de`.**

## DAVINCI Server

Über den DAVINCI Server hat man die Möglichkeit einer Mandantenverwaltung über den DAVINC Explorer. In der Regel wäre hier eine Schule ein Mandant. Über den DAVINCI-Explorer kann man mehrere Mandanten verwalten.

Benutzerzuordnung:Jeder Benutzer und jede Benutzergruppe kann einem Mandanten zugeordnet werden. Es gibt verschiedene Stufen von Administratoren. Super-Administrator (mandantenunabhängig) und Sub-Administrator (mandantenspezifisch):

Es gibt eine Datei, welcher die Benutzerrechte für alle Mandanten gespeichert werden. 

## Infoserver/Webbox/mobile App

Die Einrichtung der Webbox zur Publikation von Stunden- und Vertretungsplänen bedingt die Installation des DAVINCI Infoserver. Da dieser immer nur eine DAVINCI Datei ansprechen kann, gaher ist eine zentrale Installation hier nicht möglich.

## Updates

Soll DAVINCI aktualisiert werden, muss das auf **allen** eingesetzten Rechnern, also auf dem Server und auf allen DAVINCI Clients (in allen Schulen) geschehen.

## Dateien

Einige DAVINCI - Dateien siehe `Hilfe > Systeminformationen`im Programm sind standardmäßig je DAVINCI-Installation unter `C:\ProgramData\Stueber Systems\DAVINCI` gespeichert, existieren also eigentlich je DAVINCI-Client. Arbeiten die Nutzer in einer Terminal-Server-Umgebung, muss beim Konfigurieren beachtet werden, dass diese Daten oder die `DAVINCI.paths` je Nutzer individuell geladen werden können.

!!! tipp "Hinweis!"

    Es ist zusätzlich möglich diese Dateien auch von einer selbstvorgegebenen zentralen Stelle zu laden, die Information wird aus der `MAGELLAN.paths` ausgelesen. Eine Anleitung zum Einsatz einer MAGELLAN.paths beschreiben wir [hier](https://doc.davinci6.stueber.de/00.allgemein/pathdatei/).

## Terminal-Server oder Virtuelle Maschine?

Soll DAVINCI aktualisiert werden, muss das auf allen eingesetzten Rechnern, also auf dem Server und auf allen DAVINCI Clients (in allen Schulen) geschehen. Eine Ausnahme wäre hier der Einsatz eines Terminalservers, bei dem jeder Nutzer eine eigene Sitzung auf dem Server öffnet, die Sitzungen anderer Nutzer parallel laufen. In diesem Fall müsste nur der Terminalserver aktualisiert werden.