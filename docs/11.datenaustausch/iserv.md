# Datenaustausch mit IServ

IServ ist eine Schulplattform für die Digitalisierung von Prozessen in der Schule. DaVinci kann Stundenplandaten mit IServ abgleichen. Diese werden dann in IServ angezeigt. Die Übertragung kann manuell oder automatisiert erfolgen.

## Manueller Datenaustausch mit IServ

### Workflow in DaVinci

Die Daten aus DaVinci werden üblicherweise in einer einzelnene JSON-Datei exportiert.

Wählen Sie in DaVinci über `Plan > Importieren und Exportieren` im Import/Export-Assistent unter Exportieren `DaVinci JSON-Daten exportieren` aus.

Folgendes Fenster öffnet sich:

![DaVinci JSON-Daten exportieren](/assets/images/datenaustausch/export1.png)

* Geben Sie die Datei an, in die Sie Daten exportieren wollen: Das Ergebis ist hier eine Datei mit der Endung .json

* Zieladresse: in den DaVinci Optionen `Extras > Optionen > Upload` können Sie Vorgaben für den automatischen Upload für Dateien machen. Wenn Sie den Haken setzen, werden die Daten automatische beim Export auch an die Zieladresse übertragen

![Upload](/assets/images/datenaustausch/export2.png)

!!! info "Hinweis"

	Bei Iserv erfolgt damit jedoch kein automatischer Datenupload. In IServ muss die Datei damit immer nochmals hochgeladen werden.

* Zeitraum: Auswahl des zu exportierenden Zeitraumes

* Auswahl: Wählen Sie, ob Sie Alle Daten oder Klasse, Lehrer, Schüler exportieren möchten. Sie können zusätzlich wählen ob Termine, Änderungen, Fehlzeiten, Kalendereinträge, Schülernamen mitexportiert werden sollen.

### Was ist in IServ zu tun?

Klicken Sie auf `Hochladen`, navigieren zur entsprechenden Exportdatei aus DaVinci und klicken dann auf `OK`.

Wählen Sie anschließend unter Format den Wert `DaVinci` aus und bestätigen mit `Hochladen`.

Informationen dazu finden Sie [hier.](https://iserv.eu/doc/modules/timetable/#davinci)

!!! info "Hinweis"

    Bitte beachten Sie, dass in ISERV nur die Einträge angezeigt werden, auf die alle Filter zutreffen. Wenn man also zum Beispiel den Stundenplan einer bestimmten Klasse ansehen möchte, muss man den mittleren und rechten Filter auf "Alle Lehrer" bzw. "Alle Räume" und den linken Filter auf die entsprechende Klasse stellen.

## Automatisierter Datenaustausch mit IServ - Aktuell in Bearbeitung für die Umsetzung

Der Workflow sieht grob wie folgt aus:

+ Die **DaVinci Console** liest Daten direkt aus einer DaVinci-Datei oder von einem DaVinci-Server und überträgt diese in Ihre IServ-Instanz

+ Mit dem **PowerShell-Modul PSDaVinci** können Sie den Workflow mit einem einzigen Befehl ausführen.

### Voraussetzungen

Es werden PowerShell 7, das PowerShell-Modul PSDaVinci und natürlich eine Installation von DaVinci benötigt.

#### PowerShell 7

Die Systemvoraussetzungen für eine erfolgreiche Ausführung der PowerShell-Skripte ist **PowerShell 7**. [PowerShell 7][1] ist nicht Teil des Betriebssystems und muss separat installiert werden. 

1. Öffnen Sie die [Download-Webseite für PowerShell 7 auf GitHub][2] in Ihrem Web-Browser.

2. Laden Sie das passende Installationpaket herunter. In der Regel wird dies das MSI-Paket für Windows 64bit sein (z.B. PowerShell-7.1.3-win-x64.msi).

    [![PowerShell-Setup (Windows x64)][3]][3]
	
3. Starten Sie das MSI-Paket auf Ihrem Computer und folgen Sie den Anweisungen.

Die Ausführung von lokalen PowerShell-Skripten unter Windows Server 2019 ist standardmäßig erlaubt, unter Windows 10 jedoch nicht. In der Regel kann man mit der Ausführungsrichtlinie `RemoteSigned` gut leben. 

1. Tippen Sie im Suchfeld der Windows-Taskleiste `powershell 7` oder `pwsh` ein und starten Sie PowerShell als Administrator.

    [![PowerShell als Administrator ausführen][4]][4]

2. Tippen Sie `Set-ExecutionPolicy RemoteSigned` ein und bestätigen Sie.

    [![Ausführungsrichtlinie anpassen][5]][5]

Jetzt können Sie lokale PowerShell-Skripte problemlos starten. 

!!! tip "Hinweis"

	Einen ausführlicheren Blog-Artikel zur Installation und Nutzung von PowerShell 7 [finden Sie hier][6]. 

[1]: https://docs.microsoft.com/de-de/powershell/
[2]: https://github.com/PowerShell/PowerShell/releases/latest
[3]: /assets/images/datenaustausch/iserv/requirements-04.png "PowerShell-Setup (Windows x64)"
[4]: /assets/images/datenaustausch/iserv/requirements-02.png "PowerShell als Administrator ausführen"
[5]: /assets/images/datenaustausch/iserv/requirements-03.png "Ausführungsrichtlinie anpassen"
[6]: https://blog.stueber.de/posts/powershell7-unter-windows-10/

#### PSDaVinci

Installieren Sie das PowerShell-Modul [PSDaVinci][7]:

1. Tippen Sie im Suchfeld der Windows-Taskleiste `powershell 7` oder `pwsh` ein und starten Sie PowerShell.

    [![PowerShell ausführen][8]][8]

2. Tippen Sie `Install-Module PSDaVinci` ein und bestätigen Sie mit der Eingabetaste.

3. Beantwortn Sie die anschließende Frage, ob Sie der [PowerShell Gallery][9] (PSGallery) vertrauen möchten mit `Yes`.

	[![PowerShell: Untrusted repository][10]][10]

Das PowerShell-Modul wird nun installiert.

!!! tip "Hinweis"

	Die *PowerShell Gallery* ist ein öffentliches Repository für PowerShell-Skripte und -Module, das von Microsoft bereitgestellt wird. Da derartige Skripte theoretisch auch Unfug treiben können, wird bei jeder Installation eines PowerShell-Moduls explizit gefragt, ob man der Quelle trauen möchte. Da wir nett sind, kann man uns natürlich trauen. Im Zweifel kann man aber auch den [Quellcode inspizieren][11]. 

[7]: https://www.powershellgallery.com/packages/PsDaVinci
[8]: /assets/images/datenaustausch/iserv/requirements-05.png "PowerShell ausführen"
[9]: https://www.powershellgallery.com/
[10]: /assets/images/datenaustausch/iserv/requirements-06.png "Untrusted repository"
[11]: https://github.com/stuebersystems/psdavinci

### Konfiguration

1. Legen Sie im Windows-Explorer ein neues Verzeichnis `c:\davinci` an (das Verzeichnis kann natürlich auch anders heißen).

3. Starten Sie PowerShell 7 über das Windows-Menü: `Start > Windows Powershell > Windows Powershell`

4. Wechseln Sie mit folgendem Befehl in das soeben angelegte Verzeichnis mit:

    ```
    cd c:\davinci
    ```
5. Tippen Sie nun folgenden PowerShell-Befehl ein:

    ```
	Initialize-DaVinciExport iserv davinci.json
	```
Es wird jetzt eine Konfigurationsdatei `davinci.json` angelegt, die als Vorlage für die weitere Konfiguration dient.

Die gesamte Konfiguration des Imports befindet sich in der Textdatei `davinci.json`. Öffnen Sie diese Datei in einem Texteditor und überschreiben die gewünschten Eigenschaften.

Die folgende Eigenschaft *muss* angepasst werden. Sie konfiguriert den individuellen Zugang zu IServ:

Eigenschaft                          | Bedeutung                      
------------------------------------ | -------------------------------
`daVinci.IServExport.IServUrl `      |  URL Deiner IServ-Instanz
`daVinci.IServExport.IServApiToken`  |  API-Token aus IServ

Den API-Token für IServ finden Sie in IServ unter `Verwaltung > Module > Stundenplan`.

#### Lokale DaVinci-Datei

Die folgenden Eigenschaften *müssen* beim Abgleich von **einer lokalen DaVinci-Datei** überschrieben werden:

Eigenschaft                          | Bedeutung
------------------------------------ | ---------
`daVinci.IServExport.SourceProvider` | Wert = `File`
`daVinci.IServExport.SourceFileName` | Vollständiger Dateiname der DaVinci-Datei

#### DaVinci-Datei auf einem DaVinci-Server

Die folgenden Eigenschaften *müssen* beim Abgleich von **einer DaVinci-Datei, die auf einem DaVinci-Server gehostet wird** auf alle Fälle überschrieben werden:

Eigenschaft                          | Bedeutung
------------------------------------ | ---------
`daVinci.IServExport.SourceProvider` | Wert = `Server`
`daVinci.IServExport.ServerName`     | Servername des DaVinci-Servers im lokalen Netzwerk.
`daVinci.IServExport.ServerPort`     | Portnummer des DaVinci-Servers im lokalen Netzwerk.<br/>(Standard ist 8100)
`daVinci.IServExport.ServerUserName` | Ein DaVinci-Benutzername.
`daVinci.IServExport.ServerPassword` | Ein DaVinci-Benutzerkennwort.
`daVinci.IServExport.ServerFileID`   | Die GUID der DaVinci-Datei auf dem DaVinci-Server.

Es empfiehlt sich einen seperaten DaVinci-Benutzer für diese Funktion anzulegen, er muss lediglich das Recht haben, sich an DaVinci anmelden zu können.

![Benutzer](/assets/images/datenaustausch/iserv/iserv01.png)

Alle anderen Eigenschaften sind schon vorkonfiguriert, können aber natürlich jederzeit überschrieben werden.

!!! warning "Hinweise"

	* Der Backslash (= umgedrehter Schrägstrich) in Dateipfaden muss in einer JSON-Datei stets gedoppelt werden, also **\\\\** statt **\\**. 
	
	* Einige Zeilen in der json Datei sind mit einem "-" versehen. Diese Zeilen sind auskommentiert. Je nachdem, ob Du nun mit einer lokalen DaVinci Datei oder mit einer Datei auf dem DaVinci Server arbeitest, musst Du die "-" entsprechend setzen oder löschen. Bitte schauen dazu auch die nachfolgenden Beispiele an, dort sind für beide Beispiele die benötigten Zeilen enthalten und das "-" ist jeweils entfernt.

#### Beispiel für eine lokale DaVinci-Datei

Das Ergebnis für den Abgleich mit einer **lokalen DaVinci-Datei** könnte wie folgt aussehen:

```json
{
	"daVinci": {
		"IServExport": {
			"IServUrl": "https://mein-iserv.de",
			"IServApiToken": "01234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345==",
			"SourceProvider": "File",
			"SourceFileName": "davinci\\beispiel.daVinci",
		}
	}
}
```

#### Beispiel für eine DaVinci-Serverdatei

Das Ergebnis für den Abgleich mit **einer DaVinci-Datei, die auf einem DaVinci-Server gehostet wird**, könnte wie folgt aussehen:

```json
{
	"daVinci": {
		"IServExport": {
			"IServUrl": "https://mein-iserv.de",
			"IServApiToken": "01234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345==",
			"SourceProvider": "Server",
			"ServerName" : "localhost",
			"ServerPort" : "8100",
			"ServerUserName" : "admin",
			"ServerPassword" : "qwertz",
			"ServerFileID" : "{c24f1a9d-692c-47aa-9046-db444b9f0c8e}"
		}
	}
}
```

### Testen

1. Starten Sie PowerShell 7 über das Windows-Menü: `Start > Windows Powershell > Windows Powershell`

2. Wechseln Sie mit folgendem Befehl in unser DaVinci-Verzeichnis:

    ```
    cd c:\davinci
    ```

3. Tippen Sie folgenden PowerShell-Befehl ein:

    ```
	Start-DaVinciExport iserv davinci.json
	```

Die Daten aus DaVinci werden direkt nach IServ übertragen.	

### Automation

Die Synchronisation zwischen DaVinci und IServ kann automatisiert werden. Eine vollständige Automatisierung gelingt am besten über die Windows-Aufgabenplanung. Die Aufgabenplanung ist Bestandteil von Windows und ermöglicht das Starten von Anwendungen einmalig oder wiederkehrend zu festgelegten Zeitpunkten.

#### Ein Beispiel

Wir wollen, dass der Abgleich zwischen DaVinci und IServ alle 10 Minuten gestartet wird. Ein Upload erfolgt nur dann, wenn es auch Änderungen in DaVinci seit dem letzten Abgleich gegeben hat. Da dieser Prozess im Hintergrund läuft, soll die Ausgabe in einer Textdatei geloggt werden, so dass nachträglich geprüft werden kann, ob die Aktion erfolgreich war oder nicht. Dabei soll jeden Tag eine neue Textdatei angelegt werden. Die Konfirgurationsdatei ist in unserem Beispiel unter `c:\davinci\davinci.json` gespeichert.

Los geht's:

1. Starten Sie die Aufgabenplanung, indem Sie im Suchfeld der Windows-Taskleiste "Aufgabenplanung" eintippen.

2. Klicken Sie in der Aufgabenplanung in der rechten Aktionsleiste auf `Aufgabe erstellen`. Es öffnet sich ein Dialogfenster.

    [![Einfache Aufgabe erstellen][12]][12]

3. Tippen Sie auf der Registerkarte `Allgemein` einen Namen für Ihre neue Aufgabe ein und optional eine Beschreibung. 

    [![Name und Beschreibung][13]][13]

4. Wechseln Sie auf die Registerkarte `Trigger` und klicken Sie auf `Neu`. Jetzt müssen Sie definieren, wie oft der Abgleich ausgeführt werden soll. Wählen Sie `Täglich` aus und tragen Sie unter `Wiederhole jede` 10 Minuten ein. Bestätigen Sie mit OK.

    [![Tägliche Wiederholung][14]][14]

5. Wechseln Sie nun auf die Registerkarte `Aktionen` und klicken Sie auf `Neu`. Jetzt müssen Sie definieren, was denn nun geschehen soll. Belassen Sie die Auswahl bei `Programm starten` und tragen Sie in die drei Eingabefelder folgende Angaben ein:

    Feld                  | Eingabe
    --------------------- | -------
    Programm/Skript       | `pwsh.exe`
    Argumente hinzufügen  | `-command "& {Start-DaVinciExport iserv .\davinci.json *> .\logs\log-iserv-$(Get-Date -f yyyy-MM-dd).txt}"`
    Starten in (optional) | `c:\davinci` Bitte prüfen Sie, ob das Verzeichnis "davinci" an der Stelle angelegt wurde und ggfs. passen Sie bitte den Pfad an. Bitte im davinci-Verzeichnis ein neues Verzeichnis "logs" erstellen!

	
    Das Ganze sieht dann so aus. Klicke Sie anschließend wieder auf `OK`.

    [![Aktion][15]][15]
	
7. Alles sieht gut aus, Sie können mit `OK` abschließend bestätigen.

Die Aufgabenplanung erstellt jetzt die gewünschte Aufgabe. 

Ein Sache ist aber noch wichtig. Standardmäßig wird Ihre Aufgabe nur dann ausgeführt, wenn Sie an Ihrem Computer aktiv angemeldet sind. Das ist aber nicht immer erwünscht. Möchte man die Aufgabe beispielsweise auf einem Windows-Server erstellen, dann soll diese ja auch dann ausgeführt werden, wenn kein Server-Administrator am Server angemeldet ist (Das ist ja der Standardfall). In diesem Fall müssen Sie die Konfiguration Ihrer Aufgabe anpassen:

1. Wählen Sie eine neue Aufgabe in der Windows-Aufgabenplanung aus und klicken Sie rechts unter `Ausgewähltes Element` auf `Eigenschaften`. Es öffnet sich ein Dialogfenster.

    [![Eigenschaften][16]][16]

2. Wählen Sie unter `Sicherheitsoptionen` die Option `Unabhängig von der Benutzeranmeldung ausführen` aus und bestätigen Sie mit `OK`.

    [![Unabhängig von der Benutzeranmeldung][17]][17]

3. Sie werden jetzt aufgefordert, sich mit einem passenden Windows-Benutzerkonto zu authentifizieren. In der Regel sollte Ihr eigenes Windows-Benutzerkonto ausreichen.

    [![Authentifizierung][18]][18]

Das Ergebnis: 

Wir haben eine Aufgabe erstellt, die das PowerShell-Cmdlet zum Übertragen der Daten von DaVinci nach IServ alle 10 Minuten startet. Ein Upload erfolgt nur dann, wenn es auch Änderungen in DaVinci seit dem letzten Abgleich gegeben hat. Die Ausgabe wird in eine Textdatei geloggt, so dass Sie stets kontrollieren können, ob der letzte Übertrag erfolgreich war oder nicht. 

[12]: /assets/images/datenaustausch/iserv/automation-01.png "Einfache Aufgabe erstellen"
[13]: /assets/images/datenaustausch/iserv/automation-02.png "Name und Beschreibung"
[14]: /assets/images/datenaustausch/iserv/automation-04.png "Tägliche Wiederholung"
[15]: /assets/images/datenaustausch/iserv/automation-05.png "Programm starten"
[16]: /assets/images/datenaustausch/iserv/automation-06.png "Eigenschaften"
[17]: /assets/images/datenaustausch/iserv/automation-07.png "Unabhängig von der Benutzeranmeldung"
[18]: /assets/images/datenaustausch/iserv/automation-08.png "Authentifizierung"
