# Planwechsel

[1]:/assets/images/is/001.png
[2]:/assets/images/is/002.png
[3]:/assets/images/is/003.png
[4]:/assets/images/is/004.png
[5]:/assets/images/is/005.png

Wenn ein neuer Plan veröffentlicht werden soll, dann gibt es zwei Möglichkeiten:

1. Sie verwenden den gleichen Platzhalter für die neue Plandatei unter `DAVINCI Explorer > Plandateien` wie zuvor.
2. Sie legen einen neuen Platzhalter `DAVINCI Explorer > Plandateien` an und laden dort die neue Plandatei hoch.

!!! Tip "Empfehlung!"

    Wir empfehlen denselben Platzhalter weiterzunutzen, hierbei können die Eintragungen im `DAVINCI INFOSERVER Control` weiterverwendet werden und auch die bereits definierten und auf die Struktur festgelegten Rechte können ohne Anpassung weiterverwendet werden.

## Selben Platzhalter weiternutzen

1. Öffnen Sie das Modul `DAVINCI Explorer` und rufen den Unterpunkt `Plandateien` auf.
[![Plandatei auf Platzhalter hochladen][1]][1]

2. Laden Sie die vorbereitete Plandatei über die Schaltfläche `Hochladen` auf den bestehenden Platzhalter. Wenn Sie die alte Plandatei gern archivieren möchten, dann laden Sie diese zuvor herunter. 

3. Beenden Sie den `DAVINCI Explorer` und stoppen und starten den DAVINCI Serverdienst einmal neu. Fertig!
[![DAVINCI Serverdienst stoppen und neu starten][2]][2] 

## Neuen Platzhalter anlegen

1. Öffnen Sie das Modul `DAVINCI Explorer` und rufen den Unterpunkt `Plandateien` auf.
2. Klicken Sie auf `Hinzufügen` um einen neuen Platzhalter zu erzeugen, tragen Sie einen Namen ein und verweisen auf Ihre zu ladende Datei.
[![Neuen Platzhalter hinzufügen][3]][3]
3. Klicken Sie anschließend mit rechter Maustaste auf den neuen Platzhalter und wählen `Eigenschaften`.
[![GUID kopieren][4]][4]
4. Kopieren Sie die GUID, öffnen in der Systemsteuerung das `DAVINCI INFOSERVER-Control` und fügen die GUID und den Namen des Platzhalters ein.
[![GUID einfügen][5]][5]
1. Beenden Sie den `DAVINCI Explorer` und stoppen und starten den DAVINCI Serverdienst einmal neu.
[![DAVINCI Serverdienst stoppen und neu starten][2]][2]
6. Starten Sie Ihren Webserver neu.
7. Sollten Sie die Rechte auf Höhe des Platzhalters vergeben haben, müssen Sie die Rechte noch für den neuen Platzhalter ergänzen.

!!! Warning "Wichtig!"

    Bitte prüfen Sie in der neuen Stundenplandatei, ob die Benutzernamen in den Stammdaten der Lehrer und Klassen, ggfs. Schüler, vorbelegt sind und auch als Benutzer im `DAVINCI Explorer` angelegt sind. Hinweise zum Anlegen von Benutzern finden Sie im Abschnitt [Benutzerverwaltung](https://doc.davinci6.stueber.de/09.infoserver/user-management/).