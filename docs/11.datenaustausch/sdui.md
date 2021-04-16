# Datenaustausch mit Sdui

Sdui bietet Schulen eine DSGVO-konforme Lösung in der digitalen Kommunikation und Organisation mit Lehrern, Schülern und Eltern an. DAVINCI kann Stundenplandaten mit Sdui abgleichen. Diese werden dann in der Sdui-App angezeigt. Die Übertragung kann manuell oder automatisiert erfolgen.

Der Workflow sieht grob wie folgt aus:

+ Die **DAVINCI CONSOLE** liest Daten direkt aus einer DAVINCI-Datei oder von einem DAVINCI-Server und überträgt diese in Ihre Sdui-Instanz

+ Mit dem **PowerShell-Modul PSDaVinci** können Sie den Workflow mit einem einzigen Befehl ausführen.

## Voraussetzungen

Es werden PowerShell 7, das PowerShell-Modul PSDaVinci und natürlich eine Installation von DAVINCI benötigt.

### PowerShell 7

Die Systemvoraussetzungen für eine erfolgreiche Ausführung der PowerShell-Skripte ist **PowerShell 7**. [PowerShell 7][1] ist nicht Teil des Betriebssystems und muss separat installiert werden. 

1. Öffnen Sie die [Download-Webseite für PowerShell 7 auf GitHub][2] in Ihrem Web-Browser.

2. Laden Sie das passende Installationpaket herunter. In der Regel wird dies das MSI-Paket für Windows 64bit sein (z.B. PowerShell-7.1.3-win-x64.msi).

    [![PowerShell-Setup (Windows x64)][3]][3]
	
3. Starten Sie das MSI-Paket auf Deinem Computer und folgen Sie den Anweisungen.

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
[3]: /assets/images/datenaustausch/sdui/requirements-04.png "PowerShell-Setup (Windows x64)"
[4]: /assets/images/datenaustausch/sdui/requirements-02.png "PowerShell als Administrator ausführen"
[5]: /assets/images/datenaustausch/sdui/requirements-03.png "Ausführungsrichtlinie anpassen"
[6]: https://blog.stueber.de/posts/powershell7-unter-windows-10/

### PSDaVinci

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
[8]: /assets/images/datenaustausch/sdui/requirements-05.png "PowerShell ausführen"
[9]: https://www.powershellgallery.com/
[10]: /assets/images/datenaustausch/sdui/requirements-06.png "Untrusted repository"
[11]: https://github.com/stuebersystems/psdavinci

## Konfiguration

### Konfiguration

1. Legen Sie im Windows-Explorer ein neues Verzeichnis `c:\davinci` an (das Verzeichnis kann natürlich auch anders heißen).

3. Starten Sie PowerShell 7 über das Windows-Menü: `Start > Windows Powershell > Windows Powershell`

4. Wechseln Sie mit folgendem Befehl in das soeben angelegte Verzeichnis mit:

    ```
    cd c:\davinci
    ```

5. Tippen Sie nun folgenden PowerShell-Befehl ein:

    ```
	Initialize-DaVinciExport sdui davinci.json
	```
	
    Es wird jetzt eine Konfigurationsdatei `davinci.json` angelegt, die als Vorlage für die weitere Konfiguration dient.

## Konfigurieren
 
Die gesamte Konfiguration des Imports befindet sich in der Textdatei `davinci.json`. Öffnen Sie diese Datei in einem Texteditor und überschreiben die gewünschten Eigenschaften.

Die folgende Eigenschaft *muss* angepasst werden. Sie konfiguriert den individuellen Zugang zu Sdui:

Eigenschaft                         | Bedeutung                      
----------------------------------- | -------------------------------
`daVinci.SduiExport.SduiPIN`        |  Admin-PIN aus Sdui

Die Admin-PIN für Sdui finden Sie in Sdui unter `Administration > Stundenplan > Synchronisation`.

Die folgenden Eigenschaften *müssen* beim Abgleich von **einer lokalen DAVINCI-Datei** überschrieben werden:

Eigenschaft                         | Bedeutung
----------------------------------- | ---------
`daVinci.SduiExport.SourceProvider` | Wert = `File`
`daVinci.SduiExport.SourceFileName` | Vollständiger Dateiname der DAVINCI-Datei

Die folgenden Eigenschaften *müssen* beim Abgleich von **einer DAVINCI-Datei, die auf einem DAVINCI-Server gehostet wird** auf alle Fälle überschrieben werden:

Eigenschaft                         | Bedeutung
----------------------------------- | ---------
`daVinci.SduiExport.SourceProvider` | Wert = `Server`
`daVinci.SduiExport.ServerName`     | Servername des DAVINCI-Servers im lokalen Netzwerk.
`daVinci.SduiExport.ServerPort`     | Portnummer des DAVINCI-Servers im lokalen Netzwerk.<br/>(Standard ist 8100)
`daVinci.SduiExport.ServerUserName` | Ein DAVINCI-Benutzername.
`daVinci.SduiExport.ServerPassword` | Ein DAVINCI-Benutzerkennwort.
`daVinci.SduiExport.ServerFileID`   | Die GUID der DAVINCI-Datei auf dem DAVINCI-Server.

Es empfiehlt sich einen seperaten DAVINCI-Benutzer für diese Funktion anzulegen, er muss lediglich das Recht haben, sich an DAVINCI anmelden zu können.

Alle anderen Eigenschaften sind schon vorkonfiguriert, können aber natürlich jederzeit überschrieben werden.

!!! warning "Hinweise"

	* Der Backslash (= umgedrehter Schrägstrich) in Dateipfaden muss in einer JSON-Datei stets gedoppelt werden, also **\\\\** statt **\\**. 
	
	* Einige Zeilen in der json Datei sind mit einem "-" versehen. Diese Zeilen sind auskommentiert. Je nachdem, ob Du nun mit einer lokalen DAVINCI Datei oder mit einer Datei auf dem DAVINCI Server arbeitest, musst Du die "-" entsprechend setzen oder löschen. Bitte schauen dazu auch die nachfolgenden Beispiele an, dort sind für beide Beispiele die benötigten Zeilen enthalten und das "-" ist jeweils entfernt.

### Beispiel für eine lokale DAVINCI Datei

Das Ergebnis für den Abgleich mit einer **lokalen DAVINCI-Datei** könnte wie folgt aussehen:

```json
{
	"daVinci": {
		"SduiExport": {
			"SduiPIN": "abc-def-ghi",
			"SourceProvider": "File",
			"SourceFileName": "davinci\\beispiel.daVinci",
		}
	}
}
```

### Beispiel für eine DAVINCI-Serverdatei

Das Ergebnis für den Abgleich mit **einer DAVINCI-Datei, die auf einem DAVINCI-Server gehostet wird**, könnte wie folgt aussehen:

```json
{
	"daVinci": {
		"SduiExport": {
			"SduiPIN": "abc-def-ghi",
			"SourceProvider": "Server",
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

## Testen

1. Starten Sie PowerShell 7 über das Windows-Menü: `Start > Windows Powershell > Windows Powershell`

2. Wechseln Sie mit folgendem Befehl in unser DAVINCI-Verzeichnis:

    ```
    cd c:\davinci
    ```

3. Tippen Sie folgenden PowerShell-Befehl ein:

    ```
	Start-DaVinciExport sdui davinci.json
	```

Die Daten aus DAVINCI werden direkt nach Sdui übertragen.	
	
## Automation

Die Synchronisation zwischen DAVINCI und Sdui kann automatisiert werden. Eine vollständige Automatisierung gelingt am besten über die Windows-Aufgabenplanung. Die Aufgabenplanung ist Bestandteil von Windows und ermöglicht das Starten von Anwendungen einmalig oder wiederkehrend zu festgelegten Zeitpunkten.

### Ein Beispiel

Wir wollen, dass der Abgleich zwischen DAVINCI und Sdui alle 10 Minuten gestartet wird. Ein Upload erfolgt nur dann, wenn es auch Änderungen in DAVINCI seit dem letzten Abgleich gegeben hat. Da dieser Prozess im Hintergrund läuft, soll die Ausgabe in einer Textdatei geloggt werden, so dass nachträglich geprüft werden kann, ob die Aktion erfolgreich war oder nicht. Dabei soll jeden Tag eine neue Textdatei angelegt werden. Die Konfirgurationsdatei ist in unserem Beispiel unter `c:\davinci\davinci.json` gespeichert.

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
    Argumente hinzufügen  | `-command "& {Start-DaVinciExport sdui .\davinci.json *> .\logs\log-sdui-$(Get-Date -f yyyy-MM-dd).txt}"`
    Starten in (optional) | `c:\davinci`

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

Wir haben eine Aufgabe erstellt, die das PowerShell-Cmdlet zum Übertragen der Daten von DAVINCI nach Sdui alle 10 Minuten startet. Ein Upload erfolgt nur dann, wenn es auch Änderungen in DAVINCI seit dem letzten Abgleich gegeben hat. Die Ausgabe wird in eine Textdatei geloggt, so dass Sie stets konrtollieren können, ob der letzte Übertrag erfolgreich war oder nicht. 

[12]: /assets/images/datenaustausch/iserv/automation-01.png "Einfache Aufgabe erstellen"
[13]: /assets/images/datenaustausch/iserv/automation-02.png "Name und Beschreibung"
[14]: /assets/images/datenaustausch/iserv/automation-04.png "Tägliche Wiederholung"
[15]: /assets/images/datenaustausch/iserv/automation-05.png "Programm starten"
[16]: /assets/images/datenaustausch/iserv/automation-06.png "Eigenschaften"
[17]: /assets/images/datenaustausch/iserv/automation-07.png "Unabhängig von der Benutzeranmeldung"
[18]: /assets/images/datenaustausch/iserv/automation-08.png "Authentifizierung"