# Tipps zum Einrichten Ihres Netzwerks

Die Installation und Konfiguration des DaVinci INFOSERVERS in Ihrem lokalen Netzwerk ist relativ einfach und wird in dieser Dokumentation ausführlich beschrieben. Interessant wird es, wenn Sie Ihren Web-Server und den dort installierten DaVinci InfoServer auch über das Internet verfügbar machen wollen. Hierbei müssen Sie sich oder Ihrem Administrator folgende Fragen stellen:

1. Besitzt mein Web-Server eine öffentliche IP-Adresse bzw. kann er auf irgendeine andere Art und Weise von außen adressiert werden?

2. Kann ich auf meinen Web-Server mit Hilfe eines leicht zu merkenden DNS-Namens (z.B. `http://www.meineschule.de/davinciis.dll?`) zugreifen?

3. Ist die Netzwerkkommunikation zwischen Web-Server und Client (z.B. Web-Browser, DaVinci Mobile etc.) effektiv geschützt?

Die Beantwortung dieser Fragen hängt stark von Ihrem konkreten Netzwerk, der bereits eingesetzten Hardware und natürlich organisatorischen Vorgaben ab. Wir können daher im Folgenden nur generelle Hinweise geben. Im Zweifelsfall wenden Sie sich an unser Support Team, damit wir zusammen mit Ihnen nach passenden Lösungen suchen können.

## Eine öffentliche IP-Adresse für meinen Web-Server

In IP-Netzwerken (das Netzwerk an Ihrer Bildungseinrichtung ist ein IP-Netzwerk) unterscheidet man zwischen privaten und öffentliche IP-Adressen.

Private IP-Adressen sind Adressen aus einem fest-definierten Adressraum (z.B. 172.16.0.0 bis 172.31.255.255) und haben die Eigenschaft, dass Sie im Internet nicht geroutet werden. D.h. ein Computer mit der IP-Adresse 172.16.0.0 kann im Internet nicht (direkt) adressiert werden. Das ist auch der Grund, warum Sie in Ihrem lokalen Netzwerk private IP-Adressen nach Herzenslust vergeben können, ohne das Sie sich groß Gedanken über eventuelle Adresskonflikte im Internet machen müssen.

Öffentliche IP-Adressen haben dagegen die Eigenschaft, dass sie einen Computer im Internet eindeutig identifizieren. Da der Adressraum für öffentliche IP-Adressen begrenzt ist, werden diese von einer zentralen Stelle namens IANA (Internet Assigned Numbers Authority) vergeben. Und das ist wiederum der Grund, warum Sie IP-Adressen von Ihrem Internetprovider zugewiesen bekommen und nicht einfach selber aussuchen können.

Im besten Fall haben Sie also eine oder mehrere öffentliche IP-Adressen zugewiesen bekommen und mindestens eine dieser Adressen ist noch nicht in Gebrauch. Dann können Sie ganz einfach Ihrem Server-Computer diese IP-Adresse zuweisen und schon ist dieser im Internet verfügbar.

In der Praxis sieht dies jedoch meistens etwas anders aus. Sie besitzen genau eine öffentliche IP-Adresse, die ist aber schon in Gebrauch für Ihr Gateway, das alle Computer des Netzwerks an das  Internet anbindet. In diesem Fall haben Sie zwei Möglichkeiten:

1. Sie installieren Ihren Web-Server auf dem Gateway-Computer. Das ist nicht verkehrt, aber im Sinne einer Teilung der Aufgaben nicht empfehlenswert (Ihr Gateway hat in der Regel schon genug zu tun).

2. Richten Sie Ihr Gateway so ein, dass er eingehende HTTP-Anfragen für einen von Ihnen vorgegebenen DNS-Namen (z.B. `davinci.meineschule.de`) an Ihren internen Web-Servers (z.B. 172.10.10.10) weiterleitet. Dazu benötigen Sie natürlich einen DNS-Namen. Was das ist und wie Sie so einen Namen bekommen, erklärt der nächste Abschnitt.

Natürlich sind dies nicht alle Möglichkeiten. Sie könnten beispielsweise Ihren Web-Server als Cloud-Lösung betreiben. Das bedeutet allerdings in der Regel zusätzliche Kosten.

Sollten Sie keine Möglichkeit finden, DaVinci direkt ans Internet zu binden, können Sie trotzdem noch DaVinci-Pläne als statische HTML-Seiten exportieren und diese auf einen separaten Web-Server hochladen.

## Ein schöner DNS-Name für meinen Web-Server

Eine URL wie diese

```
http://216.58.213.35
```

kann sich niemand merken. Daher existiert in Netzwerken ein Standarddienst namens DNS (Domain Name System). Dieser bildet IP-Adressen auf sogenannte Domänennamen ab. Und das erlaubt es Ihnen, statt der Zahlenkombination von eben eine aussagekräftige URL einzutragen

```
http://www.google.de
```

Das gleiche gilt nun für Ihren DaVinci InfoServer. Um Ihre IP-Adresse über einen DNS-Namen abzufragen,  müssen Sie einen derartigen Namen definieren. In der Regel besitzen Sie bereits eine Domäne (z.B. meineschule.de) für Ihre Bildungseinrichtung. Diese sollten Sie nutzen. Richten Sie eine sogenannte Unterdomäne ein (z.B. davinci.meineschule.de) und konfigurieren Sie diese so, dass Sie auf die IP-Adresse Ihres DaVinci INFOSERVERS bzw. Web-Servers abgebildet wird. Dies funktioniert in der Regel über ein Web-Interface bei Ihrem Domänen-Provider und ist schnell gemacht.

## Die Netzwerkkommunikation effektiv sichern

Das grundlegende Sicherheitsproblem beim Kommunizieren zweier Computer über ein öffentliches Netzwerk wie z.B. das Internet ist, dass ein Fremder mit technischem Knowhow die Netzwerkkommunikation abfangen und mitlesen kann. Dies ist gemeinhin als Man-in-the-Middle-Attacke bekannt.

Die Lösung dieses Problems ist nicht, den "Mann in der Mitte" davon abzuhalten, die Netzwerkkommunikation abzugreifen, sondern vielmehr die Daten so zu verschlüsseln, dass sie keinen unmittelbaren Informationsgehalt mehr haben. In diesem Zusammenhang hat sich im Internet ein Standard namens SSL etabliert.

SSL (Secure Sockets Layer) ist eine asynchrone Verschlüsselungstechnik zum sicheren Übertragen von Inhalten. Eine SSL-geschützte Verbindung zu einem Web-Server erkennen Sie in der Regel daran, dass die URL mit einem `https` und nicht mehr mit einem `http` anfängt. Zusätzlich zeigt Ihr Web-Browser bei einer mit SSL geschützten Webseite ein kleines Vorhängeschloss neben der URL an. Ist dies der Fall, kann niemand mehr die Kommunikation zwischen Ihnen und dem entfernten Web-Server einsehen. Beispielsweise arbeiten nahezu alle Online-Banking-Portale mit SSL.

Was liegt also näher, als auch Ihre Webseiten mit SSL zu schützen.

Sie benötigen dazu lediglich ein SSL-Zertifikat. Dies müssen Sie bei einem Dienstleister im Internet erwerben. Die Kosten variieren stark und hängen unter anderem von der Laufzeit des Zertifikats ab. Mit ein bisschen Glück bekommen Sie derartige Zertifikate mit einer Laufzeit von einem Jahr schon ab 5 Euro. Googlen Sie einfach mal nach "SSL Zertifikat kaufen" und Sie bekommen zahlreiche Angebote als Suchergebnis angezeigt.

Sobald Sie das SSL-Zertifikat erworben haben, müssen Sie dieses auf Ihrem Web-Server installieren. Zudem müssen Sie Ihren Web-Server noch so konfigurieren, dass er zukünftig auf `https` und nicht mehr auf `http` reagiert. Dazu folgen Sie einfach den Anweisungen des SSL-Dienstleisters. Die meisten von ihnen stellen ausführliche Anleitungen sowohl für IIS als auch für Apache im Internet zur Verfügung.

!!! info "Hinweis"

    Neben der Neztzwerkkommunikation müssen Sie natürlich auch Ihren Web-Server als solches sichern. D.h. Sie sollten auf alle Fälle eine aktuelle Virenschutzsoftware sowie eine Firewall installieren. Schalten Sie zudem auf Ihrem Web-Server alle Dienste (z.B. FTP) ab, die Sie nicht benötigen. Das erhöht zusätzlich die Sicherheit.
