[![Build Status](https://dev.azure.com/stuebersystems/Websites/_apis/build/status/docs/doc.davinci6.de?branchName=master)](https://dev.azure.com/stuebersystems/Websites/_build/latest?definitionId=50&branchName=master)
![Deployment status](https://vsrm.dev.azure.com/stuebersystems/_apis/public/Release/badge/2cc87afa-9a3b-472b-8a3c-3eca48b22dd6/9/10)

# DaVinci 6 Dokumentation

Dies ist die deutsche Dokumentation zu [DaVinci 6](https://davinci.stueber.de). Die Dokumentation ist Open Source und wir haben sie mit [MkDocs](https://www.mkdocs.org) und [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) realisiert. 

## MkDocs unter Windows installieren

1. Installiere [Python](https://www.python.org). Gehe dazu auf die [Python-Download-Seite](https://www.python.org/downloads/) und lade Dir die aktuellste Version für Windows herunter. 

2. Starte das Installationspaket und beantworte alle Fragen.

3. Öffne die Eingabeaufforderung als Administrator.

4. Tippe die Befehle `python --version` und `pip --version` ein, um die Python-Installation zu überprüfen. In beiden Fällen sollte eine Versionsnummer als Ausgabe in der Eingabeaufforderung erscheinen.

5. Tippe jetzt den Befehl `pip install mkdocs mkdocs-material`, um das Python-Package *MkDocs* und das Theme *Material for MkDocs* zu installieren.

6. Tippe anschließend Befehl `pip install mkdocs-img2fig-plugin` ein, um das MkDocs-Plugin [mkdocs-img2fig-plugin](https://github.com/stuebersystems/mkdocs-img2fig-plugin) zu installieren.

7. Ein letzter Test: Tippe den Befehl `mkdocs --version` ein. Eine Versionsnummer in der Eingabeaufforderung zeigt Dir erneut, dass alles korrekt installiert wurde.

## Repository klonen

Dieses Repository ist ein Git-Repository. Um das Repository auf deinem lokalen Computer zu klonen, benötigst Du einen Git-Client. Entweder Du installierst Dir [Git für Windows](https://gitforwindows.org/) und arbeitest mit der Eingabeaufforderung, oder Du installierst Dir eine der zahlreichen GUIs. Zu empfehlen wären [GitHub Desktop](https://desktop.github.com) oder [SourceTree](https://www.sourcetreeapp.com).

1. Erstelle einen lokalen Ordner für die Dokumentation, z.B. `c:\docs\davinci`.

2. Starte die Eingabeaufforderung und wechsle in den Ordner `c:\docs\davinci`.

3. Tippe den Befehl `git clone https://github.com/stuebersystems/doc.davinci6.de.git` ein, um das Repository zu klonen.

## Repository als Zip-Archiv herunterladen

Willst du mit Git erstmal nichts zu tun haben, kannst Du das Repository auch als Zip-Archiv herunterladen:

1. Öffne die URL `https://github.com/stuebersystems/doc.davinci6.de` in deinem Webbrowser

2. Klicke auf die Schaltfläche `Clone or download` und dann auf `Download ZIP`.

3. Entpacke das Zip-Archiv in einen lokalen Ordner Deiner Wahl, z.B. `c:\docs\davinci`.

## Mit MkDocs arbeiten

Du hast Python und das Package MkDocs installiert, Du hast dieses Repository geklont oder als Zip-Archiv heruntergeladen. Jetzt kannst Du die Dokumentation lokal auf deinem Rechner generieren:

1. Starte die Eingabeaufforderung und wechsle in den Ordner `c:\docs\davinci`.

2. Tippe den Befehl `mkdocs build` ein. Die DAVINCI Dokumentation wird neu generiert.

3. Um Dir das Ergebnis anzeigen zu lassen, tippe den Befehl `mkdocs serve` ein und öffne die Url `http://127.0.0.1:8000` in Deinem Webbrowser.

Das Inhaltsverzeichnis findest Du in der Datei `mkdocs.yml`, die einzelnen Kapitel im Unterordner `docs`. 

## Kann ich mithelfen?

Ja, sehr gerne. Der beste Weg mitzuhelfen ist es, Rückmeldung per Issue-Tracker zu geben und/oder Korrekturen per Pull-Request zu übermitteln.
