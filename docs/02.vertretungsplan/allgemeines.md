# Allgemein

Der Stundenplan unterliegt in der Regel täglich Änderungen, die daher kommen, dass Lehrer fehlen oder Unterricht aufgrund von Klassenfahren oder aus anderen Gründen entfällt. Dies führt zu Änderungen im Stundenplan aufgrund von Vertretungen, über die die betroffenen Lehrer und Klassen schnell informiert werden müssen. Dieser Aufgabe dient die Ansicht `Vertretungsplan` in DAVINCI.

![Vertretungsplan](/assets/images/vertretungsplan/sub-plan1.png)

Sie öffnen die Ansicht `Vertretungsplan`, indem Sie in der linken Navigationsleiste auf `Vertretungsplan` klicken.

## Die Arbeitsumgebung

Der Navigationsbereich `Vertretungsplan` teilt sich in fünf Ansichten, die Sie direkt in der Gruppe `Vertretungsplan` in der Navigationsleiste aufrufen können.

* _Fehlzeiten:_ Hier erfassen Sie die Fehlzeiten der Klassen, Lehrer und Räume.

* _Stundenplan:_ In dieser Ansicht können Sie verschiedene Planänderungen direkt vornehmen, ohne vorher eine Fehlzeit eingetragen zu haben. Hier können Sie z.B. Termine verschieben und vertauschen oder Lehrer und Räume zwischen zwei Terminen vertauschen.

* _Vertretungen:_ Hier erstellen Sie die Vertretungen für die eingetragenen Fehlzeiten.

* _Änderungen:_ Diese Ansicht enthält die Änderungsliste mit den vorgenommenen Planänderungen und den erstellten Vertretungen.

* _Anrechnungen:_ Hier finden Sie eine Liste mit den Anrechnungsstunden der Lehrer. Diese Ansicht dient in der Regel nur der Information,

Wie Sie mit diesen Ansichten arbeiten können, erfahren Sie in den folgenden Kapiteln dieses Handbuchs.

## Vertretungspläne publizieren

DAVINCI stellt Ihnen verschiedene Wege zur Verfügung, Ihre Planänderungen schnell zu publizieren:

* [Webbox](https://doc.davinci6.stueber.de/09.infoserver/allgemeines/#2-davinci-webbox) oder [DAVINCI App](https://doc.davinci6.stueber.de/09.infoserver/allgemeines/#1-davinci-mobile)
* [Per Ausdruck](https://doc.davinci6.stueber.de/02.vertretungsplan/publikation/#drucken)
* [Als HTML-Pläne](https://doc.davinci6.stueber.de/02.vertretungsplan/publikation/#html-vertretungsplane-exportieren)
* [Als Kurznachricht per E-Mail oder SMS](https://doc.davinci6.stueber.de/02.vertretungsplan/publikation/#kurznachrichten-versenden)
* [Über öffentliche Bildschirme (Public Displays) in Ihrer Schule](https://doc.davinci6.stueber.de/05.look/02.ansichten/#die-ansicht-vertretungsplan)

## DAVINCI Planeigenschaften

Öffen Sie die DaVIINVI Planeigenschaften über die `Plan > Eigenschaften`. Auf der Registerkarte `Datenschutz` finden die Eintragungsmgölcihkeiten für den Vertretungsplanbereich:

![Dateieigenschaften](/assets/images/vertretungsplan/Dateieigenschaften.png)

### Änderungen

Setzen Sie den Haken bei "Änderungen freigeben", wenn Sie gezielt entscheiden möchten, ob Änderungen freigegeben werden müssen und damit im Ausdruck, in DAVINCI Look und der Webbox sichtbar sind.

Im unteren Bereich können Sie auswählen, für wieviele Tage maximimal Änderungen in der Webbox angezeoigt werden.

Mit dem Haken bei Mitteilungen für Vertretungslisten nicht publizieren, legen Sie für die Webbox fest, ob die Mittteilungen dort in der Vertretungsliste angezeigt werden oder nicht.

### Fehlgründe

Bitte wählen Sie aus, ob die Lehrer-Fehlgründe in DAVINCI LOOK als "abwesend" oder mit dem Text des Schlüsselverzeichnisses "Lehrerfehlgründe" ausgegeben wird.

Über den Haken "Fehlgrund in Lehrerplan anzeigen" können Sie zusätzlich für DAVINCI festlegen, ob der Lehrerfehlgrund hier im Léhrerplan immer mit angezeigt wird.

### Lehrer-Datenschutz

Bitte wählen Sie aus, ob die Ausdrucke der Lehrer-Veransatltungen und Lehrerzeitkonten aus DAVINCI LOOK heraus möglich ist.

## Schlüsselverzeichnisse

Bei der Erstellung der eigentlichen Vertretung werden bestimmte Schlüsselverzeichnisse verwendet, die individuell gefüllt werden können. So gelangen Sie beispielsweise zu den Schlüsselverzeichnissen für den Vertretungsplan:

* Wählen Sie in der Navigationsleiste die Navigationsgruppe `Vertretungsplan` mit der Ansicht `Fehlzeiten` aus.

* Klicken Sie die Schaltfläche `Schlüsselverzeichnisse` in der Menügruppe `Extras > Verwalten`.

![Schlüsselverzeichnisse](/assets/images/vertretungsplan/sub-plan2.png)

Um eine bestimmtes Schlüsselverzeichnis zu bearbeiten, gehen Sie beispielsweise für das Schlüsselverzeichnis „Lehrerfehlgründe" wie folgt vor:

* Wählen Sie in der Navigationsleiste die Navigationsgruppe `Vertretungsplan` mit der Ansicht `Fehlzeiten` aus.

* Klicken Sie die Schaltfläche `Schlüsselverzeichnisse` in der Menügruppe `Extras > Verwalten`.

* Markieren im Dialogfenster `Schlüsselverzeichnisse` den Eintrag "09 Lehrerfehlgründe". Klicken Sie dann auf `Bearbeiten`.

![Lehrerfehlgründe](/assets/images/vertretungsplan/sub-plan3.png)

Folgende Schlüsselverzeichnisse werden in daVinci-Vertretungsplan verwendet:

| Verzeichnis | Verwendung in daVinci-Vertretungsplan |
| :--- | :--- |
| 06 Klassenfehlgründe | Diese werden beim Eintragen von Fehlzeiten für Klassen verwendet |
| 09 Lehrerfehlgründe | Diese werden beim Eintragen von Fehlzeiten für Lehrer verwendet |
| 15 Raumfehlgründe | Diese werden beim Eintragen von Änderungen für Räume verwendet |
| 27 Vertretungsentfallgründe | Diese werden bei der Festlegung von Vertretungsalternativen genutzt (siehe Abschnitt „Vertretungsalternativen eingeben“) |
| 28 Vertretungslehrerarten | Diese werden bei der Erstellung einer Vertretung verwendet |
| 29 Vertretungsqualitäten | Diese werden bei der Erstellung einer Vertretung verwendet |

## Stammdaten

Auch in den Stammdaten gibt es Eintragungen, die Sie speziell für den Vertretungsplan treffen können.

### Fächer

In den `Stammdaten > Fächer > Vertretung` können folgende Vorgaben gemacht werden:

* **Präsenz**: wird als Art bei der Vertretungserstellung ausgegeben, Stunden fließen nicht in Lehrer-Ist Berechnung ein
* **keine Vertretung** : für diese Fächer werden keine Vertretunsgalternativen benötigt
* **keine Anrechenstunden**: für die Fehlzeit und Vertretung dieser Fächer werden keine Anrechenstunden summiert

### Lehrer

In den `Stammdaten > Lehrer > Lehrerart` kann zur Auswahl bei der Vertretungserstellung eine Lehrerart ausgewählt werden. Grundlage ist das Schlüsselverzeichnis `Lehrerart`.

## Vertretungsoptionen

Über den Aufruf `Extras > Verwalten > Optionen` gelangen Sie in das Dialogfenster der DAVINCI-Optionen. Hier  können Sie spezielle Einstellungen für den Vertretungsplan
vornehmen. 

### Allgemeine Vertretungsplanoptionen

Im Bereich `Vertretungsplan` des Dialogfensters können Sie

* vordefinierte Texte für die Spalten Info, Mitteilung und Bemerkung in der Ansicht `Vertretungen`
erstellen,
* die Behandlung von Doppelstunden bzw. Terminblöcken,
* vorziehbare Vertreter

![Dies ist das Dialogfenster „daVinci-Optionen“ mit dem Bereich `Vertretungsplan`.](/assets/images/vertretungsplan/vp08.png)

**Vordefinierte Infos, Mitteilungen und Bemerkungen**

In den Bereichen `Vordefinierte Infos`, `Vordefinierte Mitteilungen` und `Vordefinierte Bemerkungen` können Sie häufig genutzte Texte definieren, die Sie im Rahmen der Vertretungserstellung in der Ansicht `Vertretungen` in der Fehlzeiten-/Vertretungen-Liste in den Spalten Info, Mitteilung und Bemerkung als vorbelegte Texte auswählen können.

**Doppelstunden und Terminblöcke**

Durch das Markieren des Optionsfelds `Doppelstunden bzw. Terminblöcke in Einzelstunden aufteilen` legen Sie fest, ob Doppelstunden bzw. Terminblöcke in Einzelstunden aufgeteilt werden sollen. In diesem Fall kann für jede Einzelstunden der Doppelstunde bzw. des Terminblocks eine getrennte Vertretung erstellt werden.

Ist das Feld nicht markiert, werden für beide Stunden der Doppelstunde bzw. für alle Termin eines Blocks immer die gleichen Vertretung gewählt.

**Änderungen in der Plananzeige darstellen**

Im Dialogfenster `daVinci-Optionen` können Sie im Bereich `Plananzeige` Einstellungen für Änderungen im Plan in der Gruppe Änderungen vornehmen.

![Dies ist das Dialogfenster `daVinci-Optionen` mit dem Bereich `Plananzeige`.](/assets/images/vertretungsplan/vp09.png)

Sie können im DAVINCI-Vertretungsplan angeben, wie neue Änderungen im Vertretungsplan in den Stundenplänen auf dem Bildschirm und im Ausdruck speziell gekennzeichnet werden.

Definieren Sie zunächst unter `Zeitpunkt`, ab der eine Änderung als `neu` angesehen wird: den Zeitpunkt, ab der eine Änderung im Vertretungsplan als `neu` angesehen wird. Im Aufklappmenü ist dabei die Standardeinstellungen `Letzte Veröffentlichung`. Bei dieser Einstellung werden alle Änderungen als neu betrachtet, die seit der letzten Veröffentlichung der Änderung durch einen Vertretungsplaner hinzugekommen sind.

Alternativ können Sie als Zeitpunkt, ab der eine Änderung als `neu` angesehen wird, auch eine der vordefinierten Zeiteinstellungen wählen, z.B. `vor 1 Stunde`. In welcher textlichen Form diese neuen Änderungen dargestellt werden, entscheidet der Eintrag unter Kennzeichen einer neuen Änderung. Steht hier z.B. der Eintrag „\*“, so wird dieser mit Stundenplanelement angezeigt, wie die nachfolgende Abbildung exemplarisch zeigt.

Eine Besonderheit stellt die Spalte `Vertreter` in der Änderungsliste dar. Diese kann in einigen Fällen anstelle eines Lehrerkürzels auch besondere Bemerkungstexte beinhalten, z.B. bei Aufsichten, Fehlstellen. Der Eintrag unter Kennzeichnung einer Bemerkung in der Spalte `Vertreter` legt fest, welche
textliche Form eine neue Änderung kennzeichnet.

Zur analogen Kennzeichnung einer neuen Änderung im Ausdruck folgen Sie bitte den speziellen Anweisungen zum Druck von tagesaktuellen Stundenplänen (siehe Abschnitt „Tagesaktuell Stundenpläne drucken“).

### Farben

Im Dialogfenster `daVinci-Optionen` können Sie im Bereich `Farben` Farbvorgaben für bestimmte Einstellungen speziell für DAVINCI-Vertretungsplan vornehmen.

![Dies ist das Dialogfenster `daVinci-Optionen` mit dem Bereich `Farben`.](/assets/images/vertretungsplan/vp10.png)

Auf der Registerkarte `Allgemein` können die Farben für `Abwesend`, `Änderung`, `Neue Änderung` und `Unterrichtsfrei` festgelegt werden.
