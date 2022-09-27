# Benutzerverwaltung

Um den Zugriff auf DAVINCI-Daten über den DAVINCI INFOSERVER zu regulieren, müssen Sie im DAVINCI SERVER Benutzer anlegen und diesen passende Rechte zuweisen. Die nachfolgend beschriebenen Schritte steuern die Anzeige der Daten für DAVINCI WEBBOX und DAVINCI MOBILE.

Die grundlegende Vorgehensweise sieht wie folgt aus:

1. Benutzernamen in DAVINCI festlegen **=> bitte keine Umlaute verwenden!**
2. Benutzernamen aus DAVINCI exportieren und in den DAVINCI EXPLORER importieren
3. Kennungen erzeugen, ggfs. Benutzerdaten exportieren
4. Benutzergruppen definieren, Benutzer zuordnen
5. Benutzer und Benutzergruppen der Plandatei zuweisen
6. Richtlinien für Benutzer und Benutzergruppen zuweisen
7. **"Webuser" für die Anmeldung des INFOSERVERS am DAVINCI SERVER einrichten**

## Benutzernamen in DAVINCI festlegen

Für die DAVINCI-Plandatei, die der DAVINCI INFOSERVER verwendet, müssen Sie festlegen, welche Art von Benutzern Zugriff auf die Daten per DAVINCI MOBILE oder der DAVINCI WEBBOX haben sollen. In Ihrer Plandatei können grundsätzlich Lehrer, Klassen und Schüler einen Benutzernamen erhalten.

Um beispielsweise in für Lehrer die Benutzernamen einzutragen, müssen Sie wie folgt vorgehen:

* Laden Sie in DAVINCI die Plandatei, die der DAVINCI-INFOSERVER verwendet.

* Gehen Sie in die Ansicht `Stammdaten > Lehrer`.

* Hier können Sie nun in der Spalte  `Benutzername` einen beliebigen Benutzernamen pro Lehrer eingeben.

Die Vergabe der Benutzernamen kann auch alternativ durch DAVINCI automatisch erfolgen.

* Prüfen Sie unter `Plan > DAVINCI Optionen > Bezeichnungen`, ob Ihre gewünschte Bezeichnung bereits ausgewählt wurde.

Bild [![Bezeichnungen][1]][1]

* Markieren Sie anschließend in der Ansicht `Stammdaten > Lehrer` die Lehrer durch Mehrfachmarkierung, die einen neuen Benutzernamen bekommen sollen.

* Wählen Sie dann die rechte Maustaste und dort den Menüpunkt `Benutzernamen vorbesetzen` und bestätigen Sie die Sicherheitsabfrage mit `OK`.

[![Benutzer generieren][2]][2]

* Die zuvor markierten Lehrer erhalten jetzt das Lehrerkürzel als Benutzername.

!!! info "Hinweis"

    Bitte beachten Sie, dass Benutzernamen keine Umlaute enthalten dürfen. Wenn Sie die Kürzel der Lehrer als Benutzer für die Anmeldung an der Webbox verwenden möchten, muss bitte für den Benutzernamen aus "Müller" "Mueller" werden.

Analog zu den Lehrern können Sie in den Stammdaten der Klassen bzw. Schüler auch die Spalte `Benutzername` füllen.

Im Regelfall ist es ausreichend den Lehrern und Klassen Benutzernamen zu vergeben. Ein Vergabe von Benutzerkennungen für Schüler macht nur dann Sinn, wenn in den Klassen der Schüler überwiegend kein Unterricht im Klassenverbund stattfindet. Die ist beispielsweise in der Gymnasialen Oberstufe der Fall. Hier sollte jeder Oberstufenschüler seinen eigene Benutzerkennung erhalten.

## Benutzernamen exportieren

Die in DAVINCI erzeugten Benutzernamen können auch exportiert und im DAVINCI-EXPLORER wieder importiert werden. Den Aufruf zum Export finden Sie unter `Plan > Importieren und Exportieren > DAVINCI-Benutzerdaten exportieren`. Wahlweise können die Benutzerdaten für Klassen, Lehrer und/oder Schüler in eine Textdatei exportiert werden.

## Benutzer importieren oder anlegen

Für jeden in der DAVINCI-Plandatei zuvor definierten Benutzernamen muss nun im DAVINCI-EXPLORER ein entsprechender Benutzer mit Benutzername und Kennung angelegt werden.

Dazu können Sie die aus DAVINCI exportierten Benutzerdaten importieren oder Benutzer manuell anlegen.  
Passworte für die Benutzer können Sie einzeln vergeben oder für mehrere Benutzer automatisch erzeugen lassen. Markieren Sie dazu die Benutzer in der Übersicht und wählen dann in der Menüleiste den Punkt `Kennungen erzeugen` aus.

[![Kennungen erzeugen][3]][3]

Um die automatischen Kennwörter den Nutzern mitzuteilen finden Sie die Option `Exportieren` in der Menüleiste. Es wird eine Textdatei erzeugt, die die persönlichen Zugangsdaten enthält.

[![Kennungen exportieren][4]][4]

Weitere Information hierzu finden Sie in dem Abschnitt [Benutzerverwaltung](https://doc.davinci6.stueber.de/06.enterprise/06.benutzer/) des DAVINCI-EXPLORERS.

!!! info "Hinweis"

    Ein Benutzer im DAVINCI-Explorer vom Typ "Lehrer", "Klasse" bzw. "Schüler" muss immer eine korrespondierende Kennung in der dem DAVINCI-INFOSERVER zugeordneten Plandatei haben, damit diese Benutzer sich korrekt in der DAVINCI-APP anmelden kann.

## Benutzergruppen einrichten

Um nicht für einzelne Benutzer die Rechte zuordnen zu müssen, legen Sie sich Benutzergruppen an, weisen den Benutzergruppen die Benutzergruppen zu, ordnen die Benutzergruppen der Plandatei zu und vergeben dann die Rechte.
Welche Benutzergruppen Sie benötigen, hängt davon ab für welche Gruppen Sie Inhalte publizieren möchten.  Sicher benötigen Sie eine Gruppe für die Lehrer und für die Klassen. Sollen zum Beispiel Oberstufenschüler auch den individuellen Plan sehen können, benötigen Sie eine weitere Benutzergruppe.
Erzeugen Sie im DAVINCi-EXPLORER auf der Unterkarte `Benutzergruppen`über die Schaltfläche `Hinzufügen` neue Benutzergruppen. Mit einem Doppelklick auf die angelegten Benutzergruppen können Sie Benutzer per Mehrfachmarkierung hinzufügen.

!!! warning "Wichtig"

    Bitte achten Sie darauf, dass ein Benutzer möglichst nur in einer Benutzergruppe enthalten sind oder die Benutzergruppen inhaltlich nur Teilbereiche abdecken, um gegensätzliche Rechtezuweisungen zu vermeiden.

## Benutzerrechte und -gruppen der Plandatei zuordnen

Wählen Sie auf der Unterkarte `Plandateien` die Ebene aus, auf die die Benutzer zugreifen sollen und klicken dann auf die Schaltfläche  `Richtlinien` in der Menüleiste. Auf der Unterkarte `Benutzergruppen` fügen Sie Ihre angelegten Benutzergruppen hinzu.
Auf der Unterkarte `Plandateien` wählen Sie anschließend den `Arbeitsbereich` aus, klicken dann auf die Schaltfläche `Richtlinien` Unterkarte `Benutzer` fügen Sie Ihren "Webuser" hinzu,

[![Benutzer zuordnen][5]][5]

!!! info "Hinweis"

    Benutzer und Benutzergruppen kann man wahlweise auf den Ebenen Arbeitsbereich, Verzeichnis oder Plandatei per `Rechtsklick > Richtlinien` zuweisen. Bitte achten Sie darauf die BENUTZER/BENUTZERGRUPPEN NUR AUF EINER EBENE ZU ZUWEISEN, damit die Rechtestruktur eindeutig bleibt. Eine Empfehlung für den Aufbau der Plandateienstruktur und der Vergaben von Rechten finden Sie in der [DAVINCI Knowledge Base](https://doc.kb.stueber.de/) im Artikel ["Plandateienstruktur und Rechtevergabe"](https://doc.kb.stueber.de/explorer/plandateienstruktur.im.explorer.html).

## Richtlinien für DAVINCI INFOSERVER zuordnen

Im DAVINCI-EXPLORER können Sie für die  Benutzergruppen unter den "Richtlinien für DAVINCI INFOSERVER”  bestimmen, welche Rechte der Benutzer für die betreffende Plandatei erhalten soll.

Bild [![Richtlinien Infoserver][6]][6]

|Richtlinie|Optionen|
|--|--|
|**Daten exportieren**|* Nicht erlaubt|
| |* HTML exportieren erlaubt|
| |* XML und HTML exportieren erlaubt|
| |Der DAVINCI-INFOSERVER kann XML-Daten und/oder HTML-Daten vom DAVINCI-SERVER abholen, beides wird für DAVINCI-MOBILE und DAVINCI-WEBBOX nicht mehr benötigt, beide Anwendungen erhalten Daten im Format Json. Sie haben an dieser Stelle die Möglichkeit den alten Output für HTML und XML-Daten zu unterbinden.<br/> **Für den Einsatz der WEBBOX empfehlen wir hier die Auswahl "Nicht erlaubt" zu treffen.**|
|**DAVINCI WEBBOX Logout/Login anzeigen**|* Ja|
| |* Nein|
| |Möchten Sie, dass für die DAVINCI WEBBOX **der Schalter zum Aufruf des Anmeldefenster gezeigt wird**, dann wählen Sie bitte "Ja". Wenn Sie in der DAVINCI WEBBOX Inhalte zeigen möchten, die alle sehen dürfen, können Sie den Schalter zum Aufruf des Anmeldefenster mit der Auswahl "Nein" ausblenden.|
|**DAVINCI WEBBOX/MOBILE Lehrernamen anzeigen**|* Ja|
| |* Nein|
| |Hier können Sie entscheiden, ob der Lehrer in der DAVINCI WEBBOX und der App DAVINCI MOBILE im Stundenplan und **in der Vertretungsliste in der Spalte "Vertreter" mit seinem Namen (Auswahl JA) oder nur mit seinem Kürzel (Auswahl NEIN) angezeigt werden soll**.|

## Stundenpläne anzeigen

Folgende Richtlinien stehen zur Auswahl, die die Menge der angezeigten Daten bestimmen:

| Werte | Bedeutung | Ansichten in DAVINCI-MOBILE (siehe Legende) 
| --- | --- | --- |
| Nicht erlaubt | Kein Zugriff erlaubt | keine |
| Gast | keine Lehrer- /Schülerpläne erlaubt | 2 |
| Gast | Nur Klassen- und Raumpläne | 2, 3, 4, 5, 6 |
| Gast | Vertretungsliste erlaubt <br/>[nur Vertretungsdaten, keine unveränderten Veranstaltungsdaten] | 3 |
| Gast | Vertretungsliste, Raumpläne erlaubt | 3, 2 |
| Gast | Vertretungsliste, Raum-/Klassenpläne erlaubt | 3, 2 |
| Gast | Vertretungsliste, Raum-/Klassen-/Lehrerpläne erlaubt | 1, 2, 3, 4 |
| Schüler | Nur eigener Plan | 1, 3, 4, 6 |
| Klasse | Nur eigener Plan | 1, 3, 4, 6 |
| Lehrer | Nur eigener Plan, alle Klassen und Raumpläne | 1 (Lehrer), 2 (Klassen, Räume), 3, 4, 5, 6 |
| Team | Eigener Plan, Klassen-, Raumpläne des Teams | 1 (Lehrer), 2 (Klassen, Räume), 3 (des Teams), 4 (des Teams), 5 (des Teams), 6 (des Teams) |
| Teammaster | Alle Klassen-, Lehrer-, Raumpläne des Teams | 1, 2 (Lehrer des Teams, Klassen, Räume), 3 (des Teams), 4 (des Teams), 5 (des Teams), 6 (des Teams) |
| Mitarbeiter | Alle Pläne außer Lehrerpläne | 2, 3, 4, 5, 6 |
| Master | Uneingeschränkter Zugriff | alle |

## Legende für die Ansichten in DAVINCI-MOBILE

In Abhängigkeit von den Rechten, die über die Menge der angezeigten Daten bestimmen, die im DAVINCI-EXPLORER eingestellt worden sind, können folgende Übersichten in DAVINCI-MOBILE für Benutzer anzeigt werden:

| Nr. | Ansicht in DAVINCI-MOBILE |
| --- | --- |
| 1 | Eigener Plan |
| 2 | Andere Pläne |
| 3 | Liste der Änderungen/Vertretungen |
| 4 | Kalendereinträge (z.B. Ferien) |
| 5 | Übersichtspläne: Alle Klassen-/Lehrer-Raumpläne heute |
| 6 | Gebäudeplan: Was wird gerade wo unterrichtet? |

!!! warning "Wichtig"

    Die vorstehenden Ansichten sind sichtbar oder unsichtbar, werden aber entsprechend der Richtlinien mit Daten gefüllt. Hat ein Nutzer beispielsweise das Recht "Vertretungsliste erlaubt", sieht er in den jeweiligen Ansichten (Raumplan, Vertretungsliste...) nur die geänderten Daten (keine unveränderten Daten).

## Kollegen und Schulleitung

Der Gesamtplaner sollte die Richtlinie “Master” erhalten. Kollegen sollten Sie die Richtlinie “Lehrer” zuweisen. Damit können sie zwar den eigenen Plan aber keinen anderen sehen.

Sollten Sie mit Abteilungen arbeiten, können Sie die Richtline “Team” verwenden. In diesem Fall sehen die Kollegen den eigenen Plan und alle Klassen- und Raumpläne ihrer Abteilung (ihres Teams). Mit der Richtline “Teammaster” können alle Lehrerpläne des Teams eingesehen werden.

## Schüler und Eltern/Ausbilder

Schüler sind in der Regel nur dann in DAVINCI erfaßt, wenn es sich um Klassen im Kurssystem handelt, d.h. jeder Schüler hat seinen eigenen Stundenplan z.B. in der gymnasialen Oberstufe. Solange dies nicht der Fall ist, sollten Sie für jede Klasse einen Benutzer mit Benutzerkennung und Kennwort im DAVINCI-EXPLORER anlegen. Die Klasse wird damit selbst als “Benutzer” geführt. Jeder Schüler bzw. die Eltern/die Ausbilder der Schüler der Klasse erhalten dann diese Kenndaten und können per DAVINCI-APP den jeweiligen Klassenplan mit Vertretungsinformationen anzeigen.

### Nutzung mehrerer Kennungen

DAVINCI-MOBILE ist in der Lage, mit einer Anfrage an den DAVINCI-INFOSERVER mehrere Kennungen zu nutzen. In den nachfolgenden Fällen sind solche Situationen aus der Praxis beschrieben

## Eltern mit mehr als einem Kind an der Schule

Wenn Eltern mehr als ein Kind an der Schule haben, so ist die DAVINCI-APP in der Lage, diesen Sachverhalt bei der Anmeldung mit den Kenndaten zu berücksichtigen.

1. Fall: Beide Kinder sind in der gleichen Klasse und den Eltern sind nur die Kenndaten der Klasse (Benutzername `5a`/Kennwort `5apwd`) bekannt. In diesem Fall melden sich die Eltern mit Benutzernamen `5a` und dem Kennwort `5apwd` in der DAVINCI-APP an.

2. Fall: Beide Kinder sind in unterschiedlichen Klassen und den Eltern sind nur die Kenndaten der beiden Klassen (Benutzername `5a`/Kennwort `5apwd`) und (Benutzername `8c`/Kennwort `8cpwd`) bekannt. In diesem Fall melden sich die Eltern mit Benutzernamen `5a,8c` und dem Kennwort `5apwd,8cpwd` in der DAVINCI-APP an, um die Klassenpläne und Klassenvertretungen der beiden Kinder zu sehen.

3. Fall: Beide Kinder sind in unterschiedlichen Klassen und den Eltern sind die Kenndaten der beiden Kinder (Benutzername `pet35a`/Kennwort `pet35apwd`) und (Benutzername `ana68c`/Kennwort `ana68cpwd`) bekannt. In diesem Fall melden sich die Eltern mit Benutzernamen `pet35a,ana68c` und dem Kennwort `pet35apwd,ana68cpwd` in der DAVINCI-APP an, um die Schülerpläne und Schülervertretungen der beiden Kinder zu sehen.

### Ausbilder mit mehr als einem Auszubildenden an der Schule

Hier gelten die analogen Regeln, die schon zuvor bei den Kindern der Eltern beschrieben worden sind: Die Eltern entsprechen den Ausbildern und die Kinder den Auszubildenden.

### Lehrer mit Kindern an der Schule

Auch hier gelten vergleichbare Regeln wie bei den Kindern der Eltern. Wenn der Lehrer gleichzeitig seinen Stundenplan und den seines Kindes sehen möchte, müssen auch hier die Benutzernamen und Kennwörter durch Komma konkateniert bei Benutzername und Kennwort in den Einstellungen von DAVINCI-MOBILE eingegeben werden.

## Benutzer "Webuser" für den Infoserver einrichten

Benutzer für Klassen, Lehrer oder Schüler richten Sie ein, damit geklärt ist, was der einzelne Benutzer später nach der Anmeldung an der DAVINCI WEBBOX (PC) oder in DAVINCI MOBILE (Tablet, Smartphone) ansehen kann.

!!! warning "Wichtig"

    Es muss zusätzlich ein Benutzer angelegt werden, über dessen Rechte definiert wird, was ohne Anmeldung in der WEBBOX sichtbar ist. Dieser Benutzer meldet sich später auch im Hintergrund am DAVINCI SERVER an, um die von Ihnen gestatteten Daten abzuholen.  Legen Sie einen Benutzer an, nennen Sie ihn "Webuser", vergeben ein Passwort und weisen Sie ihm bitte **keine** Administratorenrechte zu.

### Webuser anlegen

Den Benutzer "Webuser" legen Sie im DAVINCI EXPLORER auf der Karte Benutzer an und weisen ihm **keine** Administratorenrechte zu.

### Webuser zuordnen

Weisen Sie diesen neuen Benutzer bitte **keiner** Benutzergruppe zu, sondern wechseln Sie auf die Karte `Plandateien`, markieren auf der linken Seite bitte den `Arbeitsbereich`, klicken dann links oben auf `Richtlinien` und fügen den Benutzer auf der Unterkarte `Benutzer` über die Schaltfläche `Hinzufügen` hinzu.

[![Webuser dem Arbeitsbereich zuweisen][7]][7]

mit Berechtigungen versehen und später für die Server-Verbindung zum DAVINCI-SERVER  unter `Start > Systemsteuerung >  DAVINCI Infoserver > Server-Verbindung` verwendet.

## Berechtigungen für den "Webuser"

!!! info "Hinweis"

    Mit diesen Einstellungen legen Sie fest, was genau gezeigt wird, wenn man die Webbox aufruft. Das könnten zum Beispiel nur Raumpläne sein, nur die Vertretungsliste oder eben auch kein Inhalt, sondern nur das Anmeldefenster.

| Richtlinie | Empfehlung |
| --- | --- |
| Daten exportieren | Für den Funktionstest des DAVINCI INFOSERVERS, wählen Sie "XML und HTML exportieren erlaubt".<br/> Möchten Sie nur mit der DAVINCI WEBBOX und DAVINCI MOBILE arbeiten, wählen Sie bitte "Nicht erlaubt". |
| DaVinci-Webbox LogIn/LogOut anzeigen | Möchten Sie, dass kein Zugriff ohne vorherige Anmeldung möglich ist, wählen Sie bitte "Ja". |
|DAVINCI WEBBOX/MOBILE Lehrernamen zeigen|Wählen Sie hier "Nein" aus.
| Stundenpläne anzeigen | Wenn ohne Anmeldung kein Inhalt dargestellt werden soll, wählen Sie bitte "Nicht erlaubt". <br/> Sollte ohne Anmeldung z.B. nur der Vertretungsplan sichtbar sein, wählen Sie "Gast: Vertretungsliste, Raumpläne erlaubt". 

Die sind die empfohlenen Einstellungen für den Webuser.

[![empfohlene Einstellungen für den Webuser][8]][8]

!!! info "Hinweis"

    Wenn Sie für den Webuser unter "Stundenpläne anzeigen" den Wert "Nicht erlaubt" wählen, verwenden Sie bitte den Parameter "account=private" in Ihrer URL, damit nicht die Fehlermeldung "901: Forbidden (error)" gezeigt wird.

```
http://Ihr Server/davinci-timetable.html?account=private
```
Start der WEBBOX ohne den Parameter account=private

[![Beschriftung][9]][9] 

Start der WEBBOX mit dem Parameter account=private

[![Beschriftung][10]][10]

[1]:/assets/images/is/bezeichnungen.png
[2]:/assets/images/is/benutzer_generieren.jpg
[3]:/assets/images/is/Kennungen_erzeugen.jpg
[4]:/assets/images/is/Kennungen_exportieren.jpg
[5]:/assets/images/is/Benutzer_zuordnen.jpg
[6]:/assets/images/is/richtlinien_infoserver.png
[7]:/assets/images/is/webuser.png
[8]:/assets/images/is/wb.empfehlung.png
[9]:/assets/images/is/wb.ohne.parameter.png
[10]:/assets/images/is/wb.mit.parameter.png