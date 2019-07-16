# DAVINCI-INFOSERVER und DAVINCI-WEBBOX absichern

Um Ihren DAVINCI-INFOSERVER bzw. Ihre DAVINCI-WEBBOX besser gegen unerlaubte Zugriffe abzusichern, sollten Sie folgende Empfehlungen beachten:

1. [Aktualisieren Sie regelmäßig DAVINCI](/09.infoserver/update-internet-publication/infoserver-und-webbox-aktualisieren.md) (insbesondere auch DAVINCI SERVER + DAVINCI INFOSERVER), DAVINCI WEBBOX und DAVINCI MOBILE.

2. Nutzen Sie https als Übertragungsprotokoll.

3. Richten Sie mit Hilfe des DAVINCI EXPLORER einen ausgewiesenen [DAVINCI-Benutzer (Webuser)](/09.infoserver/user-management.md#benutzer-webuser-für-den-infoserver-einrichten) ein, über dessen Rechte definiert wird, was ohne Anmeldung in der DAVINCI WEBBOX sichtbar ist. Dieser Benutzer wird in der Konfiguration des DAVINCI INFOSERVER als Standardnutzer hinterlegt meldet sich später auch im Hintergrund am DAVINCI SERVER an, um die von Ihnen gestatteten Daten abzuholen. Bei einem Aufruf der DAVINCI-WEBBOX muss daher kein Benutzername oder Kennwort mehr angegeben werden.

4. Diesem Benutzer dürfen natürlich **keine** Administrationsrechte zugewiesen werden, sondern nur Richtlinien im Zusammenhang mit DAVINCI INFOSERVER.

5. (Optional): Da dieser Benutzer eine öffentliche Funktion hat, ist das Kennwort nicht relevant. Es empfiehlt sich ein Kennwort wie z.B. “nopassword” zu wählen, um dies zu unterstreichen.

Zusätzliche Hinweise für DAVINCI-WEBBOX:

1. Konfigurieren Sie Ihren IIS, indem Sie für Ihre DAVINCI-WEBBOX Seite die folgenden zusätzlichen HTTP-Antwortheader hinzufügen:

* X-XSS-Protection: 1; mode=block
* X-Content-Type-Options: nosniff
* X-Frame-Options: SAMEORIGIN

2. Nutzen Sie den Aufrufparameter requestMethod=POST, um Login-Parameter im Payload zu übertragen.


