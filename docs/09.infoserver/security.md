# DaVinci-InfoServer und DaVinci-WebBox absichern

Um Ihren DaVinci-InfoServer bzw. Ihre DaVinci-WebBox besser gegen unerlaubte Zugriffe abzusichern, sollten Sie folgende Empfehlungen beachten:

1. [Aktualisieren Sie regelmäßig DaVinci](https://doc.davinci6.stueber.de/09.infoserver/update/) insbesondere auch DaVinci Server + DaVinci InfoServer), DaVinci WebBox und DaVinci Mobile.

2. Nutzen Sie https als Übertragungsprotokoll.

3. Richten Sie mit Hilfe des DaVinci Explorer einen ausgewiesenen [DaVinci-Benutzer (Webuser)](https://doc.davinci6.stueber.de/09.infoserver/user-management/#benutzer-webuser-fur-den-infoserver-einrichten) ein, über dessen Rechte definiert wird, was ohne Anmeldung in der DaVinci WebBox sichtbar ist. Dieser Benutzer wird in der Konfiguration des DaVinci InfoServer als Standardnutzer hinterlegt meldet sich später auch im Hintergrund am DaVinci Server an, um die von Ihnen gestatteten Daten abzuholen. Bei einem Aufruf der DaVinci-WebBox muss daher kein Benutzername oder Kennwort mehr angegeben werden.

4. Diesem Benutzer dürfen natürlich **keine** Administrationsrechte zugewiesen werden, sondern nur Richtlinien im Zusammenhang mit DaVinci InfoServer.

5. (Optional): Da dieser Benutzer eine öffentliche Funktion hat, ist das Kennwort nicht relevant. Es empfiehlt sich ein Kennwort wie z.B. “nopassword” zu wählen, um dies zu unterstreichen.

Zusätzliche Hinweise für DaVinci-WebBox:

1. Konfigurieren Sie Ihren IIS, indem Sie für Ihre DaVinci-WebBox Seite die folgenden zusätzlichen HTTP-Antwortheader hinzufügen:

* X-XSS-Protection: 1; mode=block
* X-Content-Type-Options: nosniff
* X-Frame-Options: SAMEORIGIN

2. Nutzen Sie den Aufrufparameter requestMethod=POST, um Login-Parameter im Payload zu übertragen.


