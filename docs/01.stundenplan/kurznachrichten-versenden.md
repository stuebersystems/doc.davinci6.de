# Kurznachrichten versenden

!!! info "Hinweis"

    Die Nutzung der in diesem Kapitel beschriebenen Funktionalität setzt eine Lizenz des Moduls DaVinci LiveMessage voraus. 
    Für den SMS Versand wird zusätzlich ein SMS-Paket benötigt.

Sie können in DaVinci jederzeit Kurznachrichten an Lehrer und Schüler senden. Diese Funktionalität können Sie z.B. verwenden, um Ihre Kollegen schnell über Vertretungsplanänderungen zu informieren.

!!! info "Hinweis"

    Zuvor müssen Sie bei den betreffenden Lehrern bzw. Schülern die E-Mail-Adressen bzw. die Mobiltelefonnummern eingegeben haben. Diese Angaben tragen Sie in der Ansicht ``Stammdaten > Lehrer`` bzw. ``Stammdaten > Schüler`` in den Spalten „E-Mail“ bzw. „Mobil“ ein.

### Einstellung in DaVinci Optionen Email

Öffnen Sie über `Extras > Optionen` Ihre DaVinci Optionen.

![Einstellung in DaVinci Optionen Email](/assets/images/stundenplan/sp124.png)

Eingabefeld | Eingabe wie folgt:
--|--
Server | Name des Mailclients
Port| Port des Mailclients
Absender E-Mail Adresse| Geben Sie hier die absendende Mailadresse an
Benutzername| Benutzername des Mailkontos
Passwort| Passwort des Mailkontos
SSL-verschlüsselte Verbindung| wenn ja bitte anhaken
SSL-Modus | geben Sie an ob der Modus Explizit oder Implizit ist

### Einstellung in DaVinci Optionen Mitteilungen

Öffnen Sie über `Extras > Optionen` Ihre DaVinci Optionen.

![Einstellungen für Änderungs- und Notfallmitteilungen](/assets/images/stundenplan/sp123.png)

Änderungsmitteilungen | Eingaben
--|--
E-Mail Betreff | Geben Sie hier den Text für den E-Mail Betreff ein, der für Änderungsmitteilungen gelten soll.
SMS-Präfix | Geben Sie hier den Präfix für SMS Mitteilungen ein, der für Änderungsmitteilungen gelten soll.

Notfallmitteilungen | Eingaben
--|--
E-Mail Betreff | Geben Sie hier den E-Mailbetreff Text ein-
Mitteilungstext | Geben Sie hier Mitteilungstext für Notfallmitteilungen ein. 

Über die Schaltfläche `Notfallmitteilung senden` können Sie die Mitteilung auch hier direkt versenden und ggf. den Betreff und den Mitteilungstext verändern.

![Notfallmitteilung senden](/assets/images/stundenplan/notfall.png)

### Einstellung in DaVinci Optionen SMS Nachrichten

Öffnen Sie über `Extras > Optionen` Ihre DaVinci Optionen.

![Einstellungen für die SMS Verbindungsdetails](/assets/images/stundenplan/sp122.png)

Mit dem Erwerb eine SMS Paketes erhalten sie die Informationen für die Absenderkennung, Benutzername und Passwort von uns. Die Standard-Ländervorwahl ist je nach Land einzutragen, standardmäßig für Deutschland ist dies die 49.

Sie erhalten bei der Bestellung Credits für den SMS-Versand. Die Credits pro SMS sind pro Provider unterschiedlich, meistens sind es 2 Credits = 2,000. Wählen Sie `Publizieren > SMS Protokoll`  um den aktuellen Status der noch zur Verfügung stehenden Credits anzuzeigen.

## Mitteilung senden

![Aufruf "Gruppen benachrichtigen"](/assets/images/MitteilungSenden02.png)

Geöffnet wird nun das **Mitteilung senden**-Fenster:

![Geben Sie hier die Kurznachricht als Mitteilung für bestimmte Empfängergruppen ein.](/assets/images/MitteilungSenden01.png)

Um bestimmte Gruppen mit einer Kurznachricht mittels E-Mail und/oder SMS zu informieren, müssen Sie wie folgt vorgehen:

1. Wählen Sie im Menüband ``Publizieren > Gruppen benachrichtigen``. 
2. Geben Sie unter **Betreff** und **Nachricht** den gewünschten Text der Kurznachricht ein. 
3. Soll die Kurznachricht per SMS und/oder E-Mail versendet werden, so markieren Sie das Kontrollkästchen ``SMS senden`` bzw. ``E-Mail senden``.
4. Wählen Sie unter ``Empfänger filtern`` die gewünschte Empfängergruppe aus. 
5. Klicken Sie auf die Schaltfläche ``Senden``, um die Kurznachricht zu versenden.

## Notfallmitteilung senden

![Aufruf "Notfall senden"](/assets/images/NotfallSenden01.png)

Geöffnet wird nun das **Notfallmitteilung senden**-Fenster:

![Geben Sie hier die Notfallmitteilung ein](/assets/images/NotfallSenden02.png)

In Notfällen, z.B. einem Feueralarm, können Sie mit einem einzigen Dialogfenster alle Schüler, Personen und Lehrer der Schule schnell informieren. Dazu gehen Sie wie folgt vor:

1. Wählen Sie im Menü ``Publizieren > Notfall senden``.
2. Geben Sie unter **Betreff** und **Nachricht** den gewünschten Text der Kurznachricht ein. 
3. Soll die Kurznachricht per SMS und/oder E-Mail versendet werden, so markieren Sie das Kontrollkästchen ``SMS senden`` bzw. ``E-Mail senden``.
4. Markieren Sie das Kontrollkästschen ``Nicht den Schülern senden``, wenn die Nachricht nicht an die Schüler gesendet werden soll.
5. Klicken Sie auf die Schaltfläche ``Senden``, um die Kurznachricht zu versenden.

## SMS Protokoll

![Protokoll aller versendeten SMS](/assets/images/sms.protokoll.png)

Erfolgt das Versenden der Kurznachricht der SMS, so werden alle gesendeten SMS mit dem jeweiligen Empfänger, der Kurznachricht, den Status der Versendung und dem Absende-Datum in einem Protokoll festgehalten. Das SMS Protokoll rufen Sie über ``Publizieren > SMS Protokoll`` auf.

![Aufruf "SMS Protokoll"](/assets/images/sms.protokoll01.png)

Zusätzlich zur Übersicht der versendeten SMS sehen Sie im Dialogfenster ``SMS Protokoll`` auch Ihren aktuellen Status der verfügbaren Kreditpunkte für die Versendung von SMS Nachrichten aufgrund Ihres erworbenen SMS-Pakets.

!!! info "Hinweis"

    Im Gegensatz zu E-Mail-Kurznachrichten sind SMS-Kurznachrichten nicht kostenfrei. Das Versenden von SMS erfordert ein sog. SMS-Paket, das als Teil der LiveMessage Lizenz erworben werden kann. Mit einem SMS-Paket erwerben Sie ein Budget von sog. Kreditpunkten, das Sie durch das Versenden von SMS aufbrauchen. Wenn Ihr Budget aufgebraucht ist, müssen Sie ein weiteres SMS-Paket erwerben, um weitere SMS versenden zu können.

!!! info "Hinweis"

    Die erworbenen Credits verfallen, wenn innerhalb eines Jahres ab Kauf des SMS-Paket keine SMS verschickt worden sind!
