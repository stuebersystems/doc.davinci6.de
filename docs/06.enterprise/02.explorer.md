# Der DAVINCI EXPLORER

## Allgemein

Der DAVINCI EXPLORER ist das Verwaltungswerkzeug für den DAVINCI SERVER. Mit Hilfe des DAVINCI EXPLORERS können die Hauptverantwortlichen neue gemeinsam zu bearbeitende Stundenpläne anlegen und verwalten, wie auch neue Benutzer zum Zweck der arbeitsteiligen Planung und des Informationsaustausches anlegen und ihnen mit Hilfe der Benutzerrechteverwaltung einen fein abgestimmten Zugriff auf die verschiedenen Zuständigkeitsbereiche der Stundenplanung einräumen.

Der DAVINCI EXPLORER wird zusammen mit der Installation von DAVINCI auf Ihren Computer kopiert. Eine explizite Installation ist also nicht nötig.

## Start

Da der DAVINCI EXPLORER nur in Verbindung mit dem DAVINCI SERVER funktioniert, ist die Installation und Konfiguration des DAVINCI SERVERS die Voraussetzung für den erfolgreichen Programmstart. Zusätzlich muss auf dem PC, auf dem der DAVINCI EXPLORER ausgeführt wird, bereits eine Verbindung zum genutzten DAVINCI SERVER eingerichtet sein.

Unter Windows XP / Vista / 7

* Klicken Sie auf das Windows-Startmenü und dann auf `Programme > STÜBER SYSTEMS > daVinci-Explorer 6`, um den DAVINCI-EXPLORER zu starten.

Unter Windows 8:

* Öffnen Sie die Windows-App-Ansicht und klicken Sie dann auf `STÜBER SYSTEMS > daVinci-Explorer 6`, um den DAVINCI EXPLORER zu starten.

Unter Windows 10:

* Klicken Sie auf das Windows-Startmenü und dann auf `Alle Apps > STÜBER SYSTEMS > daVinci-Explorer 6`, um den DAVINCI EXPLORER zu starten.

Beim Programmstart erscheint zunächst das Anmeldefenster „Mit DAVINCI Server verbinden“.

![Benutzeranmeldung beim Start des DAVINCI-EXPLORERS](/assets/images/server10.png)

Um sich am DAVINCI-EXPLORER anmelden zu können, ist ein Benutzerkonto mit entsprechenden Zugriffsrechten notwendig. Bei einer Erstinstallation ist nur das standardmäßige Administratorkonto aktiv, das die Anmeldung mit dem Benutzernamen „admin“ und einem leeren Passwortfeld erlaubt.

Um sich beim Programmstart für die Verwaltung des Mehrbenutzerbetriebs am DAVINCI EXPLORER anzumelden, führen Sie bitte folgende Schritte aus:

* Wählen im Feld `Server` bitte den Namen ihres DAVINCI-SERVERS aus, den Sie beim Einrichten der Server-Verbindung vergeben haben.

* Tragen Sie in das Feld `Benutzername` den Namen des Benutzers ein, mit dem Sie auf den DAVINCI-SERVER zugreifen möchten.

* Tragen Sie in das Feld `Kennwort` das Kennwort des Benutzerkontos ein, mit dem Sie sich anmelden möchten.

* Falls Sie sich häufig mit dem gleichen Benutzerkonto anmelden, können Sie den Punkt `Benutzername speichern` markieren, so dass der angegebene Benutzername bei der nächsten Anmeldung bereits eingetragen ist.

* Bestätigen Sie bitte mit `OK`.

Sie sind jetzt mit dem DAVINCI-EXPLORER am DAVINCI-SERVER angemeldet und können auf die Verwaltung  
der Benutzer, Mandanten und Plandateien zugreifen.

!!! info "Hinweis"

    Das standardmäßige Administratorkonto mit dem Benutzernamen „admin“ kann nicht gelöscht werden und ist bei jeder Neuinstallation vorhanden. Es verfügt wie jeder Benutzer, dem Sie die Administratorrolle zuordnen, über volle Zugriffsrechte auf alle Bereiche der Stundenplanung. Daher sollten Sie dieses, sobald Sie neue Benutzer angelegt haben, die entweder selbst Administratorrechte haben oder zumindest das Recht auf die Benutzerverwaltung des DAVINCI EXPLORERS zuzugreifen, umgehend deaktivieren oder mit einem Passwort vor unbefugtem Zugriff schützen. Wie das geht erfahren Sie im Abschnitt über die Benutzerverwaltung.

## Server-Verbindungen verwalten

Alle Funktionen zur Verwaltung der lokal eingerichteten Serververbindungen und der jeweils aktuellen Verbindung mit dem beim Programmstart ausgewählten DAVINCI SERVER sind auf der Registerkarte „Server“ oben links im Haupt-Programmfenster des DAVINCI EXPLORERS zusammengefasst.

![Serververbindungen verwalten](/assets/images/server12.png)

* Mit Server verbinden: Sind Sie aktuell mit keinem DAVINCI SERVER verbunden, können Sie sich mit Hilfe dieses des Menüpunkts mit einem DAVINCI SERVER verbinden: Es wird der Dialog „Mit DAVINCI Server verbinden“ angezeigt, dessen Bedienung im Abschnitt Programmstart näher beschrieben ist. Sie können als Abkürzung alternativ auch auf das identische Symbol oben links in der Titelzeile des Haupt-Programmfensters klicken, das die gleiche Funktion hat.

* Vom Server trennen: Sind Sie aktuell mit einem DAVINCI SERVER verbunden, können Sie die Verbindung mit Hilfe dieses Menübefehls trennen. Sie können ebenfalls auf das identische Symbol oben links in der Titelzeile klicken, dieses hat die gleiche Funktion.

* Von Server aktualisieren: Der DAVINCI EXPLORER und der DAVINCI SERVER gleichen sich bei jedem abgeschlossenen Arbeitsschritt automatisch miteinander ab. Möchten Sie vor Beginn eines Arbeitsschritts, z. B. wenn Sie länger keinen Arbeitsschritt mehr ausgeführt haben, sichergehen dass Ihnen der aktuelle Stand aller mit dem DAVINCI EXPLORER verwalteten Ressourcen angezeigt wird, können Sie diesen Menüpunkt nutzen. Auch hier können Sie zur Abkürzung alternativ auf das ähnliche Pfeilsymbol links oben in der Titelleiste klicken, das die gleiche Funktion hat.

* Server verwalten: Möchten Sie den an Ihrem lokalen PC verfügbaren Verbindungen zu unterschiedlichen DAVINCI Servern eine neue Verbindung hinzufügen oder eine bestehende Verbindung bearbeiten oder löschen, können Sie diesen Menüpunkt nutzen, um auf den Dialog „DAVINCI Server verwalten“ zuzugreifen. Die Bedienung dieses Dialogs ist im Abschnitt Die Serververbindung der Arbeitsplatz-PCs einrichten näher beschrieben.

* Server-Informationen: Wenn Sie erfahren möchten, mit welchem Server Sie gerade verbunden sind und welche Nutzer außer Ihnen aktuell auf diesen Server zugreifen, können Sie diese Funktion, die den Programmdialog „Informationen zum DAVINCI Server“ anzeigt, nutzen.

![Server-Informationen](/assets/images/server13.png)

* Optionen: Rufen Sie diesen Menüpunkt auf, um im Dialog „Optionen“ die Sprache der Programmdialoge zu ändern.

## Benutzer verwalten

Mit dem DAVINCI EXPLORER verwalten Sie Benutzer und Benutzergruppen auf Ihrem DAVINCI SERVER.

Das Anlegen von einzelnen Benutzerkonten für alle Benutzer des DAVINCI SERVERS dient der individuellen Identifikation Ihrer Benutzer, die Sie dann je nach dem jeweiligen Aufgabenbereich einer oder mehreren Benutzergruppen zuordnen können, genauso wie Sie jederzeit einzelnen Benutzern individuelle Zugriffsrechte zuweisen können, die von den Gruppenrichtlinien abweichen. Durch die individuellen Benutzerkonten und die persönlichen Angaben wissen Ihre Planer bei Auftreten von Konflikten immer, wer gerade mit Ihnen gemeinsam auf die gerade bearbeitete Planressource zugreift.

Benutzergruppen dienen dazu, mehrere Einzelbenutzer mit ähnlichen Aufgaben zusammenzufassen, um diese später als Gruppe zusammengefasst verwalten zu können. Sie können mit Hilfe der Benutzergruppen dann später z. B. allen Mitgliedern einer Gruppe, - die etwa Ihre Stundenplaner, Vertretungsplaner, Mitglieder der Verwaltung usw. umfasst - den Zugriff auf ein Planverzeichnis ermöglichen, anstatt dies für jeden Benutzer einzeln erfassen zu müssen. Um Ihnen die Arbeit zu erleichtern, bringt der DAVINCI-SERVER bei der Erstinstallation schon die Beispielbenutzergruppen „Masterplaner“, „Stundenplaner“, „Vertretungsplaner“ und „Look-Benutzer“ mit.

![Die Liste der Benutzergruppen](/assets/images/server14.png)

## Benutzerkonto hinzufügen

Das Hinzufügen eines Benutzerkontos bedeutet zunächst nur, dass der neue Benutzer zukünftig am DAVINCI-SERVER bekannt ist und nach dem Hinzufügen als aktiv gesetzt ist. Ob und mit welchem Programm der der gerade angelegte Benutzer zukünftig in einem bestimmten Umfang auf bestimmte Pläne zugreifen darf, hängt von den in einem zweiten Schritt getroffenen Einstellungen im Bereich der Richtlinien und der Zuordnung des neuen Benutzers zu Benutzergruppen ab. Der erste Schritt dazu, einem Benutzer Zugriff auf die Planung mit dem DAVINCI-SERVER zu gewähren ist jedoch, zunächst ein Benutzerkonto anzulegen.

![Einen Benutzer hinzufügen](/assets/images/server15.png)

Der Benutzerliste des aktuellen DAVINCI-SERVERS fügen Sie auf folgende Weise einen neuen Benutzer  
hinzu:

1. Wählen Sie im Programmfenster des DAVINCI-EXPLORERS die Registerkarte „Benutzer“ aus und klicken Sie anschließend in der Menüleiste auf Hinzufügen. Es öffnet sich das Dialogfenster „Benutzer hinzufügen“ mit der Registerkarte „Benutzerkonto“.

2. Tragen Sie in das Feld „Benutzername“ bitte den Namen ein, mit dem sich Ihr Benutzer zukünftig mit einem oder mehreren Programmen der DAVINCI Enterprise-Programmfamilie am DAVINCI-SERVER anmelden soll. Dieser Name dient nur der Anmeldung am Server, den vollen Namen Ihrer Benutzer können Sie an anderer Stelle zusätzlich erfassen.

3. Wählen Sie im Feld "Mandant" optional einen Mandanten, wenn das Benutzerkonto nur auf einen Mandanten beschränkt sein soll.

4. Geben Sie den Benutzertyp der Kennung an. Sie können zwischen den Kennnungen für Lehrer, Klassen, Schüler, Administratoren, Mitarbeitern und Gästen unterscheiden.

5. Geben Sie optional eine Bemerkung für das Benutzerkonto an.

6. Wählen Sie ein Kennwort, das Ihr neu angelegter Benutzer zukünftig bei der Anmeldung an den DAVINCI-SERVER eingeben muss und tragen Sie dies in das Feld „Neues Kennwort“ ein. Falls Sie die Schreibweise des Kennwortes überprüfen möchten, können Sie den Punkt „Kennwörter als Klartext anzeigen“ auswählen.

Sie haben jetzt die Angaben gemacht, die zum Anlegen eines neuen Benutzerkontos minimal nötig sind. Sofern Ihr Kennwort mindestens 8 Zeichen lang ist, wird nun am DAVINCI-SERVER ein neuer Benutzer angelegt, sobald Sie mit OK bestätigen.

!!! info "Hinweis"

    Hat das angegebene Kennwort weniger als acht Zeichen, bleibt die Schaltfläche zum Bestätigen der Änderung inaktiv. Bitte wählen Sie also immer Kennwörter von mindestens acht Zeichen Länge.

Zusätzlich zu den bisherigen Angaben, stehen Ihnen optional noch weitere Möglichkeiten zur Einrichtung  
Ihres neuen Benutzers zur Verfügung.

1. Wenn Sie aus bestimmten Gründen kein Kennwort vergeben wollen, können alternativ den Punkt „Ein neues Kennwort definieren“ deaktivieren. Ihr Benutzer kann sich dann nur mit seinem Benutzernamen anmelden, ohne ein Kennwort eingeben zu müssen.

2. Wenn Sie das neu angelegte Benutzerkonto zunächst nicht aktivieren möchten, können Sie den Punkt „Benutzerkonto ist aktiviert“ deaktivieren. Der Benutzer kann sich folge dessen erst wieder am DAVINCI-SERVER anmelden, sobald ein Benutzer mit Zugriff auf die Benutzerverwaltung sein Benutzerkonto durch Wiederauswählen dieses Punktes reaktiviert.

3. Wenn Sie den Punkt „Benutzer ist Administrator“ auswählen, hat der Benutzer als Administrator zukünftig vollen Zugriff auf alle Programmbereiche von DAVINCI Enterprise.

4. Wenn Sie den Punkt „Benutzer kann eigenes Kennwort ändern“ auswählen, kann der entsprechende Benutzer in einigen Programmen der DAVINCI Enterprise-Programmfamilie anschließend selbst sein Kennwort ändern.

5. Um zu Informationszwecken persönliche Daten wie Namen und E-Mail-Adresse Ihres Benutzers zu erfassen, können Sie von der Registerkarte „Benutzerkonto“ auf die Registerkarte „Persönliche Daten“ umblättern und die persönlichen Daten Ihres Benutzers in die entsprechenden Felder eintragen.

Sie haben jetzt alle Angaben zum Anlegen eines neuen Benutzers gemacht, sobald Sie mit OK  
bestätigen schließt sich das Dialogfenster „Benutzer hinzufügen“ und der soeben neu angelegte  
Benutzer wird in der Liste „Benutzer“ im Haupt-Programmfenster des DAVINCI Explorers angezeigt.

## Benutzerkonto ändern

Um die für einen Benutzer erfassten Daten zu ändern markieren Sie in der Liste auf der Registerkarte „Benutzer“ zunächst das zu bearbeitende Benutzerkonto durch Anklicken mit der linken Maustaste und wählen anschließend den Menüpunkt Eigenschaften aus dem Menübereich „Benutzer“. Alternativ können Sie auch mit der rechten Maustaste auf den gewünschten Benutzer klicken und den Menüpunkt Eigenschaften aus dem eingeblendeten Kontextmenü wählen. Es öffnet sich das Dialogfenster mit den Eigenschaften des Benutzerkontos, auf dem Sie alle im vorangehenden Abschnitt aufgeführten Eigenschaften hinzufügen oder ändern können.

## Benutzerkonto entfernen

Um das Konto eines Benutzers vollständig vom Server zu entfernen, markieren Sie in der Liste der Benutzerkonten bitte das zu bearbeitende Konto durch Anklicken mit der linken Maustaste und wählen anschließend den Menüpunkt Entfernen aus dem Menübereich „Benutzer“. Sie können alternativ auch mit der rechten Maustaste auf das gewünschte Konto klicken und den Menüpunkt Entfernen aus dem eingeblendeten Kontextmenü wählen.

Sobald Sie die Sicherheitsabfrage mit OK bestätigen wird das ausgewählte Benutzerkonto vollständig vom Server gelöscht.

!!! info "Hinweis"

    Wenn Sie einen Benutzerkonto nur vorübergehend nicht nutzen möchten, können Sie dieses anstelle des vollständigen Entfernens auch temporär deaktivieren. Rufen Sie dazu die Eigenschaften des entsprechenden Benutzerkontos auf wie im vorherigen Abschnitt beschrieben und entfernen Sie den Haken bei „Benutzerkonto ist aktiviert“.

## Mitgliedschaften bearbeiten

Ein Benutzer, der auf dem DAVINCI Server über ein Benutzerkonto verfügt, kann zusätzlich Mitglied einer sog. Benutzergruppe sein. Benutzergruppen dienen zur bequemen Verwaltung von Zugriffsrechten einzelner Benutzer, indem diese in Gruppen zusammengefasst werden. Die Verwaltung der Zugriffsrechte von Benutzergruppen und von Zugriffsrechten allgemein ist in den noch folgenden Abschnitten Die Richtlinien einer Benutzergruppe bearbeiten und Die Zugriffsrechte auf Pläne und Planordner mit DAVINCI Explorer verwalten erklärt. In diesem Abschnitt erfahren Sie zunächst, wie Sie einen Benutzer einer Benutzergruppe hinzufügen oder einen Benutzer aus einer Benutzergruppe entfernen.

Um einen Benutzer zum Mitglied einer Benutzergruppe zu machen oder diesen aus der Mitgliederliste  
einer Benutzergruppe wieder zu entfernen, gehen Sie bitte wie folgt vor:

* Markieren Sie in Liste der Registerkarte „Benutzer“ den Benutzer, dessen Mitgliedschaften Sie bearbeiten möchten, mit der linken Maustaste und klicken Sie anschließend auf den Menüpunkt Mitgliedschaften im Menübereich „Benutzer“. Alternativ können Sie auch mit der rechten Maustaste auf den zu bearbeitenden Benutzer klicken und den Befehl Mitgliedschaften aus dem Kontextmenü wählen: Es öffnet sich der Programmdialog „Mitgliedschaften von Benutzer“, der eine Liste aller Benutzergruppen enthält, in denen der ausgewählte Benutzer Mitglied ist.

![Liste der Mitgliedschaften eines Benutzers](/assets/images/server16.png)

* Falls Sie den Benutzer zu einer Benutzergruppe hinzufügen möchten, klicken Sie bitte auf Hinzufügen: Es öffnet sich der Dialog „Mitgliedschaften hinzufügen“, der eine Liste aller Benutzergruppen anzeigt, in denen der ausgewählte Benutzer noch nicht Mitglied ist. – Markieren Sie hier eine oder mehrere Benutzergruppen und klicken Sie anschließend auf OK, um den Benutzer den markierten Gruppen hinzuzufügen.

![Benutzergruppen zu den Mitgliedschaften hinzufügen](/assets/images/server17.png)

* Falls Sie eine Mitgliedschaft des aktuell ausgewählten Benutzers entfernen möchten, markieren Sie im Dialog „Mitgliedschaften von Benutzer“ dagegen bitte die Benutzergruppe, aus der Sie den Benutzer entfernen möchten, und klicken Sie anschließend auf Entfernen. Sobald Sie die folgende Sicherheitsabfrage mit Ja bestätigt haben, wird der Benutzer aus der entsprechenden Benutzergruppe entfernt.

## Benutzer exportieren

![Listenansicht der vorhandenen Benutzer](/assets/images/server18.png)

Um die für Ihre Benutzer erfassten Angaben zu sichern oder um beim Eingeben einer längeren Liste von Benutzern, die vielleicht schon als Dokument vorliegt, Tipparbeit zu sparen, lassen sich Listen Ihrer Benutzer im- und exportieren. Sowohl der Export als auch der Import geschieht dabei in das bzw. aus dem CSV-Dateiformat, das Sie mit jedem Texteditor aber auch komfortabel mit Tabellenkalkulationssoftware wie Microsoft Excel verwalten können.

Um die Liste Ihrer Benutzer in eine Textdatei im CSV-Dateiformat zu exportieren, führen Sie bitte folgende Schritte aus.

* Klicken Sie auf der Registerkarte „Benutzer“ im Menüband auf die Schaltfläche „Exportieren“.

* Im sich öffnenden Dialog „Benutzer exportieren“ geben Sie bitte einen Pfad zum gewünschten Speicherort der zu erzeugenden CSV-Datei ein bzw. klicken Sie auf Durchsuchen, um den Speicherort und den Dateinamen in einem Dateibrowser anzugeben.

* Wenn Sie die Standardvorgabe für das zur Trennung der einzelnen Datenfelder in der erzeugten CSV-Datei verwendete Trennzeichen von Semikolon in ein anderes Zeichen ändern möchten, können Sie dies zusätzlich im Feld „Verwendetes CSV-Trennzeichen“ tun.

* Bestätigen Sie bitte mit OK, um die Liste Ihrer Benutzer zu exportieren.

!!! info "Hinweis"

     HINWEIS: Beim Export der Benutzer wird das jeweilige Kennwort unverschlüsselt ausgegeben. Somit wäre die Liste eine mögliche Grundlage für den Administrator, um die Benutzer über deren Benutzername und Kennwort zu informieren.

## Benutzer importieren

![Der Import einer Benutzerliste](/assets/images/server19.png)

Sie können jederzeit eine zuvor mit dem DAVINCI-EXPLORER exportierte Liste der Benutzer importieren, indem Sie die dem Export analoge Funktion „Importieren“ nutzen. Möchten Sie dagegen beim neuen Anlegen Ihrer Benutzer eine vorhandene Liste aus einer anderen Anwendung wie Microsoft Excel nutzen, müssten Sie gewährleisten, dass die Reihenfolge der Felder mit der vom DAVINCI Explorer erwarteten Reichenfolge übereinstimmt. Dazu exportieren Sie am besten zunächst die Daten eines im DAVINCI-EXPLORER in der Liste der Benutzer schon vorhandenen Benutzers und formatieren dann die Reihenfolge der Felder Ihrer Liste entsprechend.

### Export der Benutzerdaten

Der einfachste Weg, um Benutzer im DAVINCI-EXPLORER zu erzeugen, ist die Übernahme der Lehrer, Klassen bzw. Schüler aus DAVINCI. Sollen dort sogar schon die Benutzernamen anleget worden sein, können Sie auch diese mit übernehmen.

* Laden Sie in DAVINCI die entsprechende Plandatei
* In den Stammdaten der Lehrer, Klassen bzw Schüler können Sie über die rechte Maustaste das Kontextmenü aufrufen. Dort wählen Sie `Benutzernamen vorbesetzen`, um für alle Einträge, die noch keine Benutzernamen, diesen automatisch erzeugen zu lassen.
* Um jetzt den Export der Benutzerdaten durchzuführen wählen Sie `Plan > Importieren und Exportieren > DAVINCI Benutzerdaten exportieren`.

![Export der DAVINCI Benutzerdaten auswählen](/assets/images/server-benutzer-export1.png)

* Markieren Sie, ob Sie Benutzerdaten von Lehrern, Klassen und/oder Schülern exportieren wollen. Geben Sie Pfad und Namen der zu exportierenden Datei an   und klicken Sie dann auf `Weiter`, um den Export zu starten.

![Welche DAVINCI Benutzerdaten werden exportiert](/assets/images/server-benutzer-export2.png)

### Import durchführen

Um eine Liste von Benutzern aus einer CSV-Datei in den DAVINCI Explorer zu importieren gehen Sie bitte folgendermaßen vor:

* Klicken Sie auf der Registerkarte „Benutzer“ auf Importieren.

* Im sich öffnenden Dialogfenster „Benutzer importieren“ tragen Sie bitte den Dateipfad zur entsprechenden CSV-Datei ein, oder nutzen Sie die Schaltfläche Durchsuchen, um die gewünschte CSV-Datei in einem Dateibrowser auszuwählen.

* Wenn Sie die Standardvorgabe zur Trennung der einzelnen Datenfelder verwendete Trennzeichen von Semikolon in ein anderes Zeichen ändern möchten, passen Sie das gewünschte Trennzeichen bitte im Feld „Verwendetes CSV-Trennzeichen“ Ihren Vorgaben an.

* Bestätigen Sie Ihre Angaben mit OK, um die in der angegebenen CSV-Datei enthaltenen Daten in die Liste der Benutzer zu importieren.

!!! info "Hinweis"

    Sollten Sie zuvor die DAVINCI-Benutzerdaten exportiert haben, so können Sie hier die aus DAVINCI erzeugt Datei für den Import verwenden. Die in das CSV-Format exportierte Liste Ihrer Benutzer kann Ihnen Tipparbeit beim Übertragen und Neuanlegen von Benutzern sparen. Sie enthält jedoch nicht sämtliche für diese Benutzer getroffenen Einstellungen wie Zugriffsrechte, Gruppenmitgliedschaften etc. Wenn Sie sämtliche Benutzereinstellungen, die Sie für Ihren DAVINCI-SERVER konfiguriert haben, sichern möchten, schließen Sie bitte die Datei „DAVINCI.users“, die sich im Arbeitsverzeichnis des DAVINCI SERVERS befindet, in Ihr Backup mit ein. Diese Datei enthält alle für Ihren Server getroffenen Benutzereinstellungen.

### Kennwörter erzeugen

Wenn Sie nach dem Import der Benutzerdaten für die Benutzer noch keine die Kennwörter haben, so können Sie neben der manuellen Eingabe des Kennworts pro Benutzer auch Kennwörter automatisch erzeugen lassen. Wenn Sie der Menüleiste "Start" die Schaltfläche `Kennwörter erzeugen` wählen, werden für alle Benutzer ohne Kennwort automatisch Kennwörter erzeugt.

## Benutzergruppen verwalten

![Die Liste der Benutzergruppen](/assets/images/server14.png)

Das Anlegen und Verwalten von Benutzergruppen dient bei der Arbeit mit DAVINCI-ENTERPRISE dazu, Richtlinien und Zugriffrechte auf bestimmte Pläne und Planbereiche für Personengruppen festzulegen. Statt für jeden Benutzer jeweils einzeln bestimmte Richtlinien und Rechte festzulegen, können Sie die entsprechenden Benutzer einer Benutzergruppe zuordnen, für die Sie die für die Gruppe geltenden Regelungen somit nur einmal zu treffen brauchen. Die für die Benutzergruppe getroffenen Regelungen  
gelten dann für alle Benutzer, die als Mitglieder der entsprechenden Benutzergruppe eingetragen werden. Wie Sie an den bei der Erstinstallation bereits voreingetragenen Beispielbenutzergruppen für Stundenplaner, Vertretungsplaner usw. erkennen können, ist ein typischer Anwendungsfall für Benutzergruppen die Zuteilung von Zugriffsrechten entsprechend dem Aufgabenbereich bei der Planung. Wie Sie in der Praxis sinnvoll mit den verschiedenen sich ergebenden Möglichkeiten arbeiten, Richtlinien für einzelne Benutzer, Benutzergruppen, Pläne und Planordner festzulegen, ist ein einem separaten Abschnitt erklärt. Der folgende Abschnitt beschreibt dagegen, wie Sie Benutzergruppen anlegen, bearbeiten und löschen können.

### neue Benutzergruppe

Wenn Sie der Liste der Benutzergruppen eine neue Gruppe hinzufügen wollen, führen Sie bitte folgende Schritte aus:

* Wählen Sie im Programmfenster des DAVINCI Explorers die Registerkarte „Benutzergruppen“ und klicken Sie in der Menüleiste auf den Menüpunkt Hinzufügen: Es öffnet sich der Dialog „Benutzer hinzufügen.

![Eine neue Benutzergruppe hinzufügen](/assets/images/server20.png)

* Tragen Sie in das Feld „Gruppenname“ den gewünschten Namen Ihrer neu anzulegenden Benutzergruppe ein.

* Tragen Sie optional in das Feld „Beschreibung“ eine zusätzliche Beschreibung ein, die in der Liste der Benutzergruppen im Haupt-Programmfenster mit angezeigt werden soll.

* Wenn Sie die neu angelegte Benutzergruppe zunächst nicht aktivieren möchten, können Sie den Haken bei „Gruppenkonto ist aktiviert“ entfernen.

* Bestätigen Sie mit OK, um die Benutzergruppe anzulegen.

### Benutzergruppe ändern

Wenn Sie die Bezeichnung einer Benutzergruppe ändern wollen oder eine Benutzergruppe de- bzw. reaktivieren wollen, gehen sie bitte wie folgt vor:

* Markieren Sie die entsprechende Benutzergruppe in der Listendarstellung der Registerkarte „Benutzergruppen“ bitte mit einem Klick auf die linke Maustaste und wählen Sie den Menüpunkt Eigenschaften aus dem Menübereich „Benutzergruppe“. Alternativ können Sie den Menüpunkt Eigenschaften auch aus dem Kontextmenü aufrufen, indem Sie mit der rechten Maustaste auf die entsprechende Benutzergruppe klicken: Es öffnet sich das Dialogfenster „Eigenschaften von Benutzergruppe“.

* Nehmen Sie die gewünschten Änderungen in den Feldern „Gruppenname“, „Beschreibung“ und „Gruppenkonto ist aktiviert“ vor.

* Bestätigen Sie Ihre Änderungen mit OK, um diese zu übernehmen.

!!! info "Hinweis"

    Das Deaktivieren einer Benutzergruppe wirkt sich ausschließlich auf die mit der Mitgliedschaft in dieser Benutzergruppe verbundenen Rechte aus. Ein Benutzer, der Mitglied in einer deaktivierten Benutzergruppe hat, hat die genau jene Rechte, die er hätte, wenn seine Mitgliedschaft in dieser Gruppe entfernt wäre. Sie können diese Funktion nutzen, um bestimmte Rechte nur vorübergehend zu gewähren oder zu entziehen.

### Benutzergruppe entfernen

Eine Benutzergruppe lässt sich folgendermaßen vom Server entfernen:

* Markieren Sie die entsprechende Benutzergruppe in der Listendarstellung der Registerkarte „Benutzergruppen“ bitte mit einem Klick auf die linke Maustaste und wählen Sie den Menüpunkt Entfernen aus dem Menübereich „Benutzergruppe“. Alternativ können Sie den Menüpunkt Entfernen auch aus dem Kontextmenü aufrufen, indem Sie mit der rechten Maustaste auf die entsprechende Benutzergruppe klicken.

* Bestätigen Sie die folgende Sicherheitsabfrage mit OK, um die gewählte Benutzergruppe dauerhaft zu löschen.

### neue Mitglieder

Um einer Benutzergruppe einzelne Mitglieder hinzuzufügen, gehen Sie bitte wie folgt vor:

* Markieren Sie im Haupt-Programmfenster in der Liste der Registerkarte „Benutzergruppen“ die Benutzergruppe, der Sie neue Mitglieder hinzufügen wollen.

* Wählen Sie aus der Menügruppe „Benutzergruppe“ den Menüpunkt Mitglieder: Es öffnet sich der Programmdialog „Mitglieder von Benutzergruppe“, der eine Liste aller Benutzer anzeigt, die aktuell Mitglied der ausgewählten Benutzergruppe sind.

![Die Mitgliederliste einer Benutzergruppe](/assets/images/server21.png)

* Klicken Sie auf die Schaltfläche Hinzufügen: Es öffnet sich der Dialog „Mitglieder hinzufügen“, der alle Benutzer anzeigt, die aktuell nicht Mitglied der ausgewählten Benutzergruppe sind.

![Einer Benutzergruppe Mitglieder hinzufügen](/assets/images/server22.png)

* Wählen Sie aus der Liste einen oder mehrere Benutzer, die Sie der Benutzergruppe hinzufügen möchten und bestätigen Sie mit OK.

* Die ausgewählten Benutzer sind jetzt Mitglieder der entsprechenden Benutzergruppe.

### Mitglieder entfernen

Führen Sie bitte folgende Schritte aus, um Benutzer aus einer Benutzergruppe zu entfernen:

* Markieren Sie die Benutzergruppe, deren Mitgliederliste Sie bearbeiten möchten.

* Wählen Sie aus der Menügruppe „Benutzergruppe“ den Menüpunkt Mitglieder: Es öffnet sich der Programmdialog „Mitglieder von Benutzergruppe“, der eine Liste aller Benutzer anzeigt, die aktuell Mitglied der ausgewählten Benutzergruppe sind.

* Markieren Sie in der Liste einen oder mehrere Benutzer, die Sie aus der Mitgliederliste der ausgewählten Benutzergruppe entfernen möchten und klicken Sie auf die Schaltfläche Entfernen.

* Bestätigen Sie die folgende Sicherheitsabfrage mit OK.

Der bzw. die ausgewählten Benutzer sind jetzt aus der entsprechenden Benutzergruppe entfernt  
worden.

## Plandateien verwalten

Indem Sie im Programmfenster die Registerkarte „Plandateien“ auswählen, erreichen Sie die Ansicht zur Verwaltung Ihrer Pläne. Sie können diese in beliebig vielen Ordnern und Unterordnern organisieren und in einem zweiten Schritt mit Hilfe von Benutzererrichtlinien festlegen, ob die entsprechenden Ordner und Pläne allen oder nur bestimmten am DAVINCI Server angemeldeten Benutzern zur Verfügung stehen sollen.

![Die Registerkarte für Plandateien](/assets/images/server23.png)

In der Programmansicht des DAVINCI EXPLORERS, die zur Verwaltung Ihrer Plandateien dient, befindet sich auf der linken Seite der Bereich „Planordner“, in dem die Ordnerstruktur, die Sie auf dem Server angelegt haben, um Ihre Plandateien zu organisieren, in einer Baumansicht angezeigt wird. Bei der  
Ersteinrichtung wird hier nur das Wurzelverzeichnis „Arbeitsbereich“ angezeigt, in dem Sie beliebig viele eigene Ordner und Unterordner anlegen können. Auf der rechten Seite befindet sich der Bereich „Plandateien“. In diesem werden alle im links ausgewählten Ordner enthaltenen Pläne aufgelistet, wie Sie es auch vom Windows-Explorer kennen, wenn Sie sich den Inhalt eines Dateiordners anzeigen lassen. Planordner dienen nicht nur dazu, Ihre Pläne sinnvoll und übersichtlich zu gruppieren, Sie können auch bestimmten Nutzern oder Nutzergruppen besondere Rechte nur für einzelne Ordner  oder Unterordner zuweisen. Wie Sie Benutzern und Benutzergruppen Zugriffsrechte auf bestimmte Pläne und Planordnern gewähren erfahren Sie im folgenden Abschnitt. Dieser Abschnitt beschreibt, wie Sie Planordner und neue Pläne anlegen können sowie Plandateien auf den Server laden oder vom Server auf ihr lokales System herunterladen können.

### Planordner hinzufügen

Um auf dem DAVINCI SERVER einen neuen Planordner anzulegen, tun Sie bitte Folgendes:

* Markieren Sie im linken Bereich „Planordner“ den Arbeitsbereich oder den Ordner, in dem der neue Ordner als Unterordner angelegt werden soll, mit der linken Maustaste und wählen Sie aus dem Menübereich „Planordner“ den Menüpunkt Hinzufügen. Alternativ können Sie auch mit der rechten Maustaste ein Element in der Baumansicht anklicken und den Befehl Hinzufü- gen aus dem Kontextmenü wählen: Es öffnet sich der Programmdialog „Planordner hinzufügen“.

![Einen neuen Planordner hinzufügen](/assets/images/server24.png)

* Tragen Sie im Feld „Ordnername“ den gewünschten Ordnernamen ein.

* Aktivieren oder deaktivieren Sie die Auswahl des Punktes „Planordner ist aktiviert“, um zu entscheiden, ob Ihr Ordner und die enthaltenen Plandateien für den Zugriff bereitstehen sollen.

* Bestätigen Sie Ihre Auswahl mit OK, um den Dialog zu schließen und den Planordner anzulegen.

### Planordner bearbeiten

Führen Sie bitte die folgenden Schritte aus, wenn Sie den Namen eines Planordners nachträglich  
ändern möchten oder einen Ordner nachträglich aktivieren oder deaktivieren wollen:

* Markieren Sie im Bereich „Planordner“ der Registerkarte „Plandateien“ den Ordner, an dem Sie Änderungen vornehmen möchten mit der linken Maustaste und wählen Sie aus dem Menübereich „Planordner“ den Menüpunkt Eigenschaften. Alternativ können Sie auch mit der rechten Maustaste auf einen Ordner klicken und den Befehl Eigenschaften aus dem Kontextmenü wählen: Es öffnet sich der Programmdialog „Eigenschaften von Planordner“.

![Die Eigenschaften eines Planordners](/assets/images/server25.png)

* Nehmen Sie die gewünschten Änderungen in den Feldern „Ordnername und „Planordner ist aktiviert“ vor.

* Bestätigen Sie Ihre Änderungen mit OK, um diese zu übernehmen.

### Planordner entfernen

Einen Planordner wird folgendermaßen vom Server entfernt:

* Markieren Sie im Bereich „Planordner“ den Ordner, den Sie löschen möchten mit der linken Maustaste und wählen Sie aus dem Menübereich „Planordner“ den Menüpunkt Entfernen. Alternativ können Sie auch mit der rechten Maustaste auf einen Ordner klicken und den Befehl Entfernen aus dem Kontextmenü wählen.

* Bestätigen Sie die folgende Sicherheitsabfrage mit OK, um den gewählten Planordner dauerhaft zu entfernen.

!!! info "Hinweis"

    Löschen Sie einen Planordner, der Plandateien enthält, werden alle zum Zeitpunkt des Löschens noch im Ordner enthaltenen Plandateien mit gelöscht! Wenn Sie einen Ordner nur vorübergehend für den Zugriff sperren wollen, können Sie diesen temporär deaktivieren, wie im Abschnitt Einen Planordner bearbeiten beschrieben.

## Plan

### Plan hinzufügen

Um auf dem DAVINCI-SERVER eine neue Plandatei anzulegen, gehen Sie folgendermaßen vor:

* Markieren Sie im linken Bereich „Planordner“ den Arbeitsbereich oder den Ordner, in dem Sie die neue Plandatei anlegen wollen und wählen Sie aus dem Menübereich „Plandatei“ den Menüpunkt `Hinzufügen`. Alternativ können Sie, nachdem Sie einen Planordner markiert haben, auch mit der rechten Maustaste in den rechten Bereich „Plandateien“ klicken und den Befehl Hinzufügen aus dem Kontextmenü wählen: Es öffnet sich der Programmdialog „Plandatei hinzufügen“.

![Eine Plandatei hinzufügen](/assets/images/server26.png)

* Tragen Sie in das Feld „Dateiname“ den gewünschten Namen des neuen Plans ein.

* Fügen Sie falls gewünscht im Feld eine Beschreibung hinzu, die in der Liste der Plandateien zusätzlich mit angezeigt werden soll.

* Aktivieren oder deaktivieren Sie die Auswahl des Punktes „Plandatei ist aktiviert“, um zu entscheiden, ob der neu angelegte Plan für den Zugriff bereitstehen soll.

* Bestätigen Sie Ihre Auswahl mit OK, um den Dialog zu schließen und die Plandatei anzulegen. Die neu angelegte Plandatei steht jetzt auf dem DAVINCI Server zu Zugriff mit den Programmen der DAVINCI Enterprise-Programmfamilie bereit. Die Client-Programme zeigen die neu angelegte Datei als vollständig leeren Plan an. Möchten Sie Ihren Benutzern dagegen einen Plan bereitstellen, der schon bestimmte Basis-Informationen enthält, müssen Sie diesen Basisplan auf den Server laden. Dies ist im Abschnitt „Eine lokale Plandatei auf den Server laden“ erklärt.

### Plan bearbeiten

So können Sie den Namen einer Plandatei nachträglich ändern oder diese nachträglich aktivieren oder deaktivieren:

* Wählen Sie im linken Bereich „Planordner“ den Arbeitsbereich oder den Ordner, in dem sich die zu bearbeitende Plandatei befindet und markieren Sie im linken Bereich „Plandateien“ die Datei, die Sie bearbeiten wollen. Wählen Sie anschließend aus dem Menübereich „Plandatei“ den Menüpunkt Eigenschaften. Ebenso können Sie mit der rechten Maustaste auf ein Element im Bereich „Plandateien“ klicken und den Befehl Eigenschaften aus dem Kontextmenü wählen: Es öffnet sich der Programmdialog „Plandatei hinzufügen“.

![Die Eigenschaften einer Plandatei bearbeiten](/assets/images/server27.png)

* Nehmen Sie die gewünschten Änderungen in den Feldern „Dateiname“, „Beschreibung“ und „Plandatei ist aktiviert“ vor.

* Bestätigen Sie Ihre Änderungen mit OK, um diese zu übernehmen.

### Plan entfernen

Um eine Plandatei vom Server zu entfernen gehen Sie bitte wie folgt vor:

* Wählen Sie auf der Registerkarte „Plandateien“ im rechten Bereich die Datei, die Sie löschen möchten, mit der linken Maustaste und wählen Sie aus dem Menübereich „Plandatei“ den Menüpunkt Entfernen. Alternativ können Sie auch mit der rechten Maustaste auf eine Plandatei klicken und den Befehl Entfernen aus dem Kontextmenü wählen.

* Bestätigen Sie die folgende Sicherheitsabfrage mit OK, um die gewählte Plandatei dauerhaft zu löschen.

### Plan hochladen

Mittels der Funktion „Plan hinzufügen“ neu angelegte Pläne werden als vollständig leere Pläne  
dargestellt. Wenn Sie dagegen Ihren Mitplanern einen bereits als lokale Datei existierenden Plan zur  
Verfügung stellen wollen, gehen Sie bitte wie folgt vor:

* Erstellen Sie, wie im Abschnitt „Eine Plandatei hinzufügen“ erklärt, mittels der Funktion Hinzufügen einen neuen Plan und tragen Sie den gewünschten Namen und die gewünschte Beschreibung ein.

* Markieren Sie den angelegten Plan auf der Registerkarte „Plandateien“ in der Liste der Pläne mit der linken Maustaste und klicken Sie im Menübereich „Plandatei“ auf den Menübefehl Hochladen. Sie können den Menübefehl Hochladen alternativ auch aus dem Kontextmenü des ausgewählten Plans aufrufen.

* Wählen Sie im nun angezeigten Dateibrowser „Lokale DAVINCI Plandatei auswählen“ die lokale Datei, die Sie auf dem Server bereitstellen möchten, und klicken Sie auf Öffnen.

* Bestätigen Sie die folgende Erfolgsmeldung mit OK.

Eine Kopie Ihrer lokalen Datei steht nun unter dem beim Hinzufügen angegebenen Namen auf dem  
Server für den Zugriff über DAVINCI Enterprise bereit.

### Plan herunterladen

Wenn Sie einen auf dem DAVINCI-SERVER gespeicherten Plan auf Ihrem lokalen PC als DAVINCI Datei speichern möchten, führen Sie bitte folgende Arbeitsschritte aus:

* Markieren Sie in der Programmansicht der Registerkarte „Plandateien“ den Plan, den Sie vom Server herunterladen möchten.

* Wählen Sie aus dem Menübereich „Plandatei“ den Menüpunkt Herunterladen. Sie können den Befehl Herunterladen ebenfalls aus dem Kontextmenü des ausgewählten Plans aufrufen.

vWählen Sie im sich öffnenden Dateibrowser „DAVINCI Plandatei lokal speichern unter“ einen Speicherort und tragen Sie den gewünschten Dateinamen ein, unter dem Sie die Datei lokal speichern möchten und bestätigen Sie mit Speichern.

* Bestätigen Sie die folgende Erfolgsmeldung mit OK.

Eine Kopie des auf dem Server gespeicherten Plans wurde unter dem angegebenen Dateinamen lokal  
gespeichert.

## Zugriffrechte

Die Verwaltung von Benutzer- bzw. Benutzergruppenrechten mit dem DAVINCI-EXPLORER dient dazu, Benutzern oder Benutzergruppen bestimmte Rechte für die Arbeit mit bestimmten Plänen zu gewähren oder zu entziehen. Alle Festlegungen gelten dabei immer für einen bestimmten Ordner im Teilfenster „Planordner“ der Programmansicht „Plandateien“ oder – dies ist der einfachste Fall, der zugleich bei der Erstinstallation für die Standardbenutzergruppen vorgegeben ist – für den gesamten Wurzelordner „Arbeitsbereich“ und damit für alle Plandateien auf dem Server.

Die Festlegung der Zugriffrechte für Benutzer geschieht dabei immer in drei Schritten:

* Es wird ein bestimmtes Element des Arbeitsbereichs gewählt, für das die Benutzerrechte bearbeitet werden sollen. Dies kann der Arbeitsbereich insgesamt sein, ein Ordner oder eine einzelne Plandatei.

* Im Richtlinien-Dialog des gewählten Elements wird ausgewählt, ob die zu bearbeitenden Richtlinien für einen bestimmten Benutzer oder für eine bestimmte Benutzergruppe gelten sollten. Das geschieht entweder durch das Auswählen eines Benutzers oder einer Benutzergruppe aus einer Liste, oder das Hinzufügen eines Benutzers oder einer Benutzergruppe zu einer Liste.

* Ist somit in Schritt 1. und Schritt 2. der Bereich des Arbeitsbereiches und der Personenkreis festgelegt worden, werden die einzelnen Richtlinien bearbeitet.

Diese drei prinzipiellen Schritte werden in den folgenden Abschnitten noch einmal konkret anhand von  
Beispielen und den entsprechenden Programmfunktionen erklärt.

## Arbeit mit Benutzergruppen

Zur Erinnerung: Im Abschnitt Benutzergruppen mit dem DAVINCI Explorer verwalten haben Sie  
erfahren, wie Sie die einzelnen Benutzer bestimmter Personenkreise mit ähnlichen Aufgaben in  
Benutzergruppen wie z. B. Stundenplaner, Vertretungsplaner, Schulleitung oder Sekretariat zusammenfassen  
können. Bei der Erstinstallation bringt DAVINCI Enterprise schon einige BeispielBenutzergruppen  
für „Masterplaner“, „Stundenplaner“, „Vertretungsplaner“ und „Look-Benutzer“ mit.  
Die Festlegung von Richtlinien für Einzelbenutzer oder Benutzergruppen unterscheidet sich nicht  
prinzipiell. Eine Festlegung für eine Benutzergruppe wirkt sich einfach so aus, als wäre die Festlegung  
für alle Mitglieder der Benutzergruppe einzeln getroffen worden.

## Arbeit mit Planordnern

Im Abschnitt Plandateien mit dem DAVINCI Explorer verwalten haben Sie erfahren, wie Sie Ihrem rbeitsbereich neue Planordner und Plandateien hinzufügen können. Am Anfang dieses Abschnitts urde bereits erwähnt, dass der erste Schritt zur Arbeit mit Zugriffsrechten immer in der Auswahl eines lanordners oder einer Plandatei besteht, für den oder die die zu treffenden Festlegungen gelten sollen. Ist Ihr „Arbeitsbereich“ in mehrere Ordner und Unterordner gegliedert, ergeben sich auf Grund der hierarchischen Ordnerstruktur des Arbeitsbereiches entsprechend der Baumansicht im linken nterfenster „Planordner“ der Registerkarte „Plandateien“ zusätzliche Möglichkeiten bzw. Besonderheiten ei der Verwaltung der Zugriffsrechte auf Pläne und Planordner. So übertragen sich alle in Rchtlinien, die für ein Element des „Arbeitsbereichs“ getroffen wurden, auf alle in der Baumansicht des Arbeitsbereichs“ untergeordneten Elemente, d. h. eine Festlegung, die Sie für den Wurzelordner "rbeitsbereich“ treffen gilt ausnahmslos für alle Ordner und Unterordner und alle darin befindlichen Plandateien. Würden Sie im Rahmen der folgenden Abbildung dagegen statt für den Arbeitsbereich als Ganzes eine Festlegung für den „Ordner 1“ treffen, würden die im Dialog „Richtlinien von Ordner 1 bearbeiten“ definierten Richtlinien für alle im „Ordner 1“ enthaltenen Unterordner und Plandateien gelten, nicht jedoch für die im „Ordner 2“ enthaltenen Pläne und Unterordner.

![Registerkarte mit Plandateien](/assets/images/server28.jpg)

Die zweite Besonderheit im Rahmen von Ordnerhierarchien stellt die Möglichkeit dar, Benutzerrichtlinien zu staffeln. Nehmen wir an, in der obigen Abbildung ist, wie dies bei der Erstinstallation standardmäßig der Fall ist, dem gesamten Arbeitsbereich die Benutzergruppe „Stundenplaner“ zugeordnet. Diese hat standardmäßig das Recht, Pläne zu öffnen und zu bearbeiten. Nimmt man jetzt an, der „Ordner 2“ enthielte die Pläne des letzten Jahres, die von den Stundenplanern nur noch zur Ansicht genutzt, aber nicht mehr bearbeitet werden sollen, so kann die Benutzergruppe „Stundenplaner“ dem „Ordner 2“ zugewiesen werden, obwohl die Benutzergruppe Stundenplaner ja schon dem „Arbeitsbereich“ zugeordnet ist. Auf diese Weise können dann für die Benutzergruppe „Stundenplaner“ im Richtliniendialog von „Ordner 2“ nur die Besonderheiten für diesen Ordner erfasst werden. Es wird also ausschließlich die Richtlinie zum Bearbeiten von Plandateien auf „Nicht erlaubt“ gesetzt, ansonsten gelten weiter die allgemeinen Festlegungen für den übergeordneten Wurzelordner „Arbeitsbereich“.

!!! info "Hinweis"

    Mit Hilfe der Richtlinienverwaltung lassen sich nach den oben genannten Prinzipien umfangreiche und fein abgestufte Arbeitsszenarien verwalten. Gerade bei der Verwaltung zahlreicher Nutzer ist die Möglichkeit Richtlinien zu staffeln ein mächtiges und arbeitssparendes Werkzeug. Umgekehrt können die komplexen Kombinationsmöglichkeiten, die sich ergeben, aber auch verwirrend wirken. Daher empfiehlt es sich bei der Einarbeitung in DAVINCI Enterprise, sich bei der Festlegung von neuen Richtlinien zunächst auf das Wurzelverzeichnis „Arbeitsbereich“ zu beschränken, wie dies bei einer Erstinstallation auch bei den vorgegebenen Benutzergruppen der Fall ist. So gelten alle Festlegungen immer für sämtliche Plandateien auf dem Server und es ist einfach, den Überblick zu behalten.

## Richtlinien

### "Richtlinien" für Planordner

Um für einen Planordner oder eine Plandatei den Dialog zur Festlegung der Benutzer- oder Benutzergruppenrichtlinien aufzurufen, gehen Sie bitte folgendermaßen vor:

* Wählen Sie auf der Registerkarte „Plandateien“ im linken Teilfenster „Planordner“ den Ordner, für den Sie die Benutzerrichtlinien neu festlegen oder verändern wollen, durch einen Klick mit der linken Maustaste aus.

* Wählen Sie im Menübereich „Planordner“ den Menüpunkt „Richtlinien“. Alternativ können Sie auch mit der rechten Maustaste auf den gewünschten Planordner klicken und den Menüpunkt „Richtlinien“ aus dem eingeblendeten Kontextmenü wählen. Es öffnet sich der Dialog „Richtlinien“ des gewählten Ordners

Die getroffenen Einstellungen gelten beim Bearbeiten der Richtlinien für einen Planordner für alle im  
gewählten Ordner und ggf. Unterordnern des gewählten Ordners enthaltenen Pläne.

### "Richtlinien" für Plandateien

Um für eine bestimmte Plandatei den Dialog zur Festlegung der Benutzer- bzw. Benutzergruppenrichtlinien aufzurufen, gehen Sie bitte wie folgt vor:

* Wählen Sie auf der Registerkarte „Plandateien“ im linken Teilfenster „Planordner“ den Ordner, der die Plandatei enthält, deren Benutzerrichtlinien Sie neu festlegen oder bearbeiten wollen.

* Wählen Sie im linken Teilfenster „Plandateien“ die Plandatei, deren Richtlinien Sie bearbeiten wollen.

* Wählen Sie im Menübereich „Plandatei“ den Menüpunkt „Richtlinien“.

* Es öffnet sich der Dialog „Richtlinien“ der gewählten Plandatei.

Die Einstelllungen, die Sie im Dialog „Richtlinien“ einer Plandatei treffen, gelten anschließend nur für  
diese einzelne Plandatei.

### Dialogfenster Richtlinien

Das Dialogfenster „Richtlinien“, das in der Programmansicht „Plandateien“ für den Wurzelordner „Arbeitsbereich“, jeden Planordner innerhalb des Arbeitsbereichs und auch für jede einzelne Plandatei separat aufgerufen werden kann, ist in die beiden Ansichten „Benutzer“ und „Benutzergruppen“ unterteilt. Auf der linken Seite des Dialogs befindet sich ein Teilfenster mit einer Liste der Benutzer bzw. Benutzergruppen, rechts daneben befindet sich Ansicht mit einer Listendarstellung der Richtlinien, die für den links ausgewählten Benutzer oder die links ausgewählte Benutzergruppe gelten.

![Richtlinien](/assets/images/server29.jpg)

### Richtlinien bearbeiten

Um die Zugriffsrechte eines Benutzers oder einer Benutzergruppe für einen bestimmten Teil des  
Arbeitsbereichs zu bearbeiten, gehen Sie bitte wie folgt vor:

* Öffnen Sie wie das Dialogfenster `Richtlinien` für das Element des Arbeitsbereichs, für das Sie die entsprechenden Richtlinien bearbeiten wollen.

* Wählen Sie die Registerkarte `Benutzer` oder `Benutzergruppen`, je nachdem, ob Sie die Richtlinien für einen einzelnen Benutzer oder eine Benutzergruppe bearbeiten möchten.

* Wählen Sie aus der Liste der Benutzer oder Benutzergruppen den Benutzer oder die Benutzergruppe, für die Sie Richtlinien bearbeiten oder neu festlegen möchten. Ist der gewünschte Benutzer oder die gewünschte Benutzergruppe noch nicht in der Liste vorhanden, klicken Sie auf die Schaltfläche `Hinzufügen` und führen Sie zusätzlich folgende Schritte aus:

  * Wählen Sie im Dialog `Benutzergruppen hinzufügen` bzw. `Benutzer hinzufügen` die Benutzergruppen oder die Benutzer, die Sie der Liste hinzufügen möchten.

  * Bestätigen Sie Ihre Auswahl mit `OK`. Die hinzugefügten Benutzer oder Benutzergruppen sind jetzt im Dialogfenster `Richtlinien` verfügbar.

![Hinzufügen von Benutzergruppen](/assets/images/server30.jpg)

* Wählen Sie im Dialogfenster `Richtlinien` im rechten Teilfenster die Richtlinie, die Sie bearbeiten möchten und klicken Sie auf die Schaltfläche `Bearbeiten`.

* Wählen Sie im sich öffnenden Dialogfenster `Richtlinie bearbeiten` aus der Auswahlliste `Wert` den für die im Feld `Richtlinie` angegebenen Wert. Es stehen folgende Werte zur Auswahl:

  * `Übergeordnete Richtlinie verwenden` – Die für ein in der Ordnerhierarchie des Arbeitsbereiches getroffene Festlegung wird für die unter „Richtlinie“ angezeigte Richtlinie nicht verändert.

  * `Nicht erlaubt` – Die im Feld „Richtlinie“ angezeigte Aktion ist im ausgewählten Bereich für den ausgewählten Benutzer bzw. die ausgewählte Benutzergruppe nicht erlaubt.

  * `Nicht erlaubt` – Die angezeigte Aktion ist im ausgewählten Bereich für den ausgewählten Benutzer bzw. die ausgewählte Benutzergruppe erlaubt

![Bearbeiten einer Richtlinie](/assets/images/server31.jpg)

* Bestätigen Sie Ihre Auswahl im Dialogfenster `Richtlinie bearbeiten` mit `OK`.

* Passen Sie ggf. weitere Richtlinien Ihren Wünschen an. Wenn Sie mit Ihrer Arbeit fertig sind, können Sie das Dialogfenster schließen.

### Ein Beispiel

Die Masterplanerin unserer DAVINCI-Schule heißt Frau Freitag, die mit den beiden Stundenplanern Herrn Bolzano und Herrn Gauss mit Hilfe des DAVINCI-SERVERS gemeinsam an der Erstellung der Stundenpläne arbeitet. Um allen drei die nötigen Zugriffsrechte dafür einzurichten ruft Frau Freitag die Registerkarte `Benutzer` auf und legt zunächst die drei Benutzer „Freitag“, „Gauss“ und „Bolzano“ an. Anschließend öffnet sie die Mitgliedschaften ihres eigenen Benutzerkontos und fügt die Benutzergruppe „Masterplaner“ hinzu. Dann ruft sie auf der Registerkarte `Benutzergruppen` die Mitgliederliste der Benutzergruppe "Stundenplaner" auf und fügt die Benutzer "Bolzano" und "Gauss" hinzu. Zuletzt geht Sie auf die Registerkarte `Plandateien` und ruft die Richtlinien des Arbeitsbereiches auf. Hier sind die Benutzergruppen „Masterplaner“ und „Stundenplaner“ bereits standardmäßig vorhanden. Das Ergebnis ist, dass Frau Freitag auf alle Planordner und Pläne auf dem Arbeitsbereich mit den Rechten eines Masterplaners zugreifen kann. Herr Bolzano und Herr Gauss können ebenfalls auf alle Ordner und Pläne auf dem Arbeitsbereich zugreifen, jedoch mit den Rechten der Benutzergruppe „Stundenplaner“. Um ganz sicher zu gehen, erstellt Frau Freitag einen neuen Plan, den Sie „Neuer Plan“ nennt, und fügt in den Richtlinien des Plans „Neuer Plan“ Herrn Bolzano als Benutzer hinzu. Tatsächlich werden für Herrn Bolzano die Zugriffsrechte nach den Richtlinien der Benutzergruppe „Stundenplaner“ angezeigt, weil Frau Freitag die Benutzergruppe „Stundenplaner“ mit Ihren entsprechenden Richtlinien ja dem Arbeitsbereich hinzugefügt hat.

![Ein Beispiel für Gruppenrichtlinien](/assets/images/server32.png)

Da Herr Bolzano sich anhand eines Beispielplans gern mit der Arbeit im Modul Vertretungsplan vertraut machen möchte, räumt Frau Freitag ihm in den Richtlinien von „Neuer Plan“ die entsprechenden Rechte ein. Der Zugriff auf die Vertretungsplanung ist Herr Bolzano also nur bei diesem Plan möglich.

## Mandanten verwalten

Im DAVINCI-EXPLORER können Sie Mandanten auf der gleichnamigen Registerkarte einzurichten. Ein Mandant ist in der Regel eine Schule. Ein DAVINCI-SERVER verwaltet dann mehrere Mandanten. Für Mandanten gilt:

* Jeder Benutzer und jede Benutzergruppe kann einem Mandant zuordnen werden

* Ein Benutzer, der einem Mandant zugordnet wurde, kann als Sub-Administrator fungieren, indem Sie bei ihm die Option „Benutzer ist Administrator“ markieren.

Die Aufgaben des Super-Administrators (keinem Mandant zugeordnet) und des Sub-Administrators (der einem Mandanten zugeordnet ist) ergeben sich aus folgender Tabelle:

| Super-Administrator (mandantenunabhängig) | Sub-Administrator (für einen Mandanten) |
| --- | --- |
| Hinzufügen und Löschen von Mandanten | Hinzufügen und Löschen von weiteren SubAdministratoren für den Mandanten |
| Hinzufügen und Löschen von Sub-Administratoren | Hinzufügen und Löschen von Planunterordnern für den Mandanten |
| Hinzufügen und Löschen von Planordnern für jeden Mandanten | Hinzufügen und Löschen von Benutzern für den Mandanten |

### Mandanten einrichten

![Einen Mandanten hinzufügen](/assets/images/server35.png)

Als Administrator (nicht als Sub-Administrator) können Sie auf der Registerkarte „Mandanten“ über Hinzufügen neue Mandanten einrichten. Ein Mandant muss einen über alle Mandanten eindeutigen Namen haben und eine optionale Beschreibung. Es liegt daher nahe, für Schulen die Schulnummer als eindeutigen Namen zu verwenden.

![Registerkarte Mandanten. Sie ist nicht sichtbar für Sub-Administratoren](/assets/images/server36.png)

### Benutzer und Benutzergruppen

![Registerkarte mit Benutzern](/assets/images/server11.png)

Sowohl der Super-Administrator wie auch der Sub-Administrator kann über Hinzufügen die weiteren Benutzer einrichten, der Sub-Administrator ausschließlich die für seinen Mandanten. Der Name einer Benutzergruppe muss über alle Mandanten eindeutig sein. So macht es z.B. Sinn, den Benutzergruppennamen immer mit der vorangestellten Schulnummer beginnen zu lassen.

![Registerkarte mit Benutzergruppen](/assets/images/server37.png)

## Planordner für Mandanten anlegen

![Planordner für jeden Mandanten](/assets/images/server38.png)

Auf der Registerkarte „Plandateien“ legt der Super-Administrator je Mandant einen Ordner unterhalb des Arbeitsbereichs an, indem er dem Ordner einen Namen gibt, z.B. die Schulnummer und ihm einem Mandanten zuweist.

![Benutzergruppen zuweisen und Richtlinien festlegen](/assets/images/server39.png)

Anschließend weist der Administrator oder der Sub-Administrator des Mandanten diesem Ordner die betreffenden Benutzer bzw. Benutzergruppen, die für den Mandanten vorgesehen sind, zu.

## Sub-Administratoren

![Sub-Administrator hinzufügen](/assets/images/server40.png)

Ein Sub-Administrator ist ein Benutzer, dem im Eingabefeld „Mandant“ ein Mandant zugeordnet wurde und der über die Option „Benutzer ist Administrator“ als Sub-Administrator ausgewiesen wurde. Im Gegensatz zu einem Super-Administrator, also einem Benutzer ohne Mandantenzuordnung der als „Administrator“ markiert wurde, kann ein Sub-Administrator nur im Bereich seines Mandanten arbeiten, d.h. er sieht nur folgendes:

| Registerkarte | Sichtbarkeit für Sub-Administrator |
| --- | --- |
| Benutzer | Nur Benutzer seines Mandanten |
| Benutzergruppen | Alle Benutzergruppen aller Mandanten |
| Plandateien | Nur die Planordner seines Mandanten |
| Mandanten | Nicht sichtbar |

Ein Sub-Administrator kann weitere Sub-Administratoren sowie weitere Benutzer oder Benutzergruppen - allerdings ausschließlich für seinen Mandanten - anlegen. Der einem Mandanten zugeordnete Benutzer kann nur den Ordner seines Mandanten (seiner Schule) sehen.
