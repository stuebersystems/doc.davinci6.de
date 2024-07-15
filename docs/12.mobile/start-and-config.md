# Starten und einstellen

## Starten

Um DaVinci-Mobile zu starten, müssen Sie das Icon `DaVinci` auswählen.

![DaVinci Mobile Icon](/assets/images/appicon.png)

### Einführungstour

Beim ersten Aufruf wechselt die App in eine Einführungstour 

![Einführungstour](/assets/images/appappletour.png)
 
Diese Tour zeigt Ihnen mit einigen Slides die wichtigsten Schaltflächen von DaVinci-Mobile. Durch Wischen nach Links gelangen Sie zum jeweils nächsten Slide. Durch Klicken auf den Text `Tour beenden` beenden Sie die Einführungstour. Die Einführungstour können Sie jederzeit erneut starten, wenn Sie 

* auf dem Smartphone die Schaltflächen <img src="/assets/images/appiconmenu.svg" alt="Menü Icon" height="24" width="24">, anschließend <img src="/assets/images/appiconinfo.svg" alt="Info Icon" height="24" width="24"> und dann <img src="/assets/images/appiconintro.svg" alt="Intro Icon" height="24" width="24"> wählen bzw.

* auf dem Tablet die Schaltflächen <img src="/assets/images/appiconinfo.svg" alt="Info Icon" height="24" width="24"> und dann <img src="/assets/images/appiconintro.svg" alt="Intro Icon" height="24" width="24"> wählen.

### Demomodus

Wenn Sie die App erstmalig starten, so ist diese mit dem Demoserver von STÜBER SYSTEMS verbunden. Auf diese Weise können Sie die [grundsätzliche Funktionsweise von DaVinci-Mobile kennenlernen](usage.md). Wie Sie den Demomodus  verlassen können, um sich mit Ihrer Schule/Bildungsinstitution zu verbinden, erfahren Sie im nachfolgenden Abschnitt.

## Einstellen

Über die Einstellungen können Sie festlegen, mit welchem DaVinci-SERVER die App DaVinci-Mobile verbunden ist. 

* Auf Smartphones wechseln Sie in die Einstellungen über die Schaltfläche <img src="/assets/images/appiconmenu.svg" alt="Menü Icon" height="24" width="24"> links oben und dann <img src="/assets/images/appiconsettings.svg" alt="Setting Icon" height="24" width="24">.

* Auf Tablets wechseln Sie in die Einstellungen über die Schaltfläche <img src="/assets/images/appiconsettings.svg" alt="Setting Icon" height="24" width="24"> rechts unten.

![Einstellungen](/assets/images/appapplesetting.png)

Hier müssen Sie die Zugangdaten Ihrer Schule/Bildungsinstitution eintragen. Dazu müssen Sie zunächst den Demomodus deaktivieren, indem Sie 

1. unter `Demo Modus` den Wert `inaktiv` eintragen und
 
2. dann Ihre Zugangsdaten einfügen unter

    * DaVinci SERVER (z.B. `davinci.meineSchule.de` )
    * Benutzername
    * Kennwort

![Einstellungen Lehrer Demo](/assets/images/appapplesetting2.png)

Wenn Sie nach der Angabe der Daten die Schaltfläche `Zurück` wählen, werden aufgrund der Zugangsdaten die Daten vom Server zur Anzeige in der App geladen. In Abhängigkeit von den mit der Kennungen verbundenen Rechten (wie z.B. Schüler, Lehrer, Schulleitung) stellt die App [unterschiedliche Informationen zu Auswahl](usage.md).

!!! warning "Wichtig!"

    Zu Ihrer Sicherheit wird Ihr eingegebenes Passwort weder gespeichert noch übertragen. Stattdessen nutzen wir einen Hash-Wert, den wir bei der Eingabe Ihres Kennwortes erzeugen.
	
    Nach der Eingabe Ihres Kennwortes werden unabhängig von der Zeichenlänge 6 Punkte als Platzhalter dargestellt - die Länge der Eingabe ist dadurch nicht ableitbar.

### Mehrere Kennungen

DaVinci-Mobile ist in der Lage mehrere Benutzernamen in den Einstellungen zu verwenden. Wenn Sie z.B. als Eltern mehr als ein Kind oder als Ausbilder mehr als einen Auszubildenden in der Schule/Bildungsinstitution haben, so können Sie die Benutzernamen bzw. Kennwörter durch Komma konkateniert eintragen. 

#### Beispiel

Sie haben als Eltern zwei Kennungen für Ihre beiden Kinder in der gleichen Schule.

Erstes Kind:

Feld         | Wert
------------ |------
Benutzername | `Kind1`
Kennwort     | `Kind1pwd`

Zweites Kind:

Feld         | Wert
------------ |------
Benutzername | `Kind2`
Kennwort     | `Kind2pwd`

Um die Stundenpläne und Vertretungspläne beider Klasse sehen zu können, müssen Sie die Kennungen wie folgt in den Einstellungen eintragen:

Feld            | Wert
--------------- | ----
Benutzername    | `Kind1,Kind2`
Kennwort        | `Kind1pwd,Kind2pwd`

!!! warning "Wichtig!"

    Bitte achten Sie darauf bei der Aufzählung der Benutzernamen oder Kennworte nach dem Komma keine Leerzeichen einzufügen!

### Demomodus erneut aktivieren 

Um den Demomodus erneut zu aktiveren, müssen Sie zunächst unter `Demo Modus` den Wert von `Inaktiv` auf `Aktiv` stellen

Bitte geben Sie im Feld DAVINIC SERVER **demo-davinci.stueber.de** ein

* `Lehrer Demo`: Beispieleinstellung für eine Lehrerkennung

oder

* `Klassen Demo`: Beispieleinstellung für eine Klassenkennung

stellen.
