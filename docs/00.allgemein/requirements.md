# Systemvoraussetzungen

## DAVINCI

| DAVINCI| Kompatibilität|
| -- | -- |
| **Betriebssystem 32-Bit** | Windows 8/10 |
| **Betriebssystem 64-Bit** | Windows 8/10 und Windows Server 2008 R2/2012/2016/2019/2022|
| **Hardware** | DAVINCI benötigt keine besonderen Hardware-Anforderungen |
| **Bildschirmauflösung** | Die Bildschirmauflösung sollte 1024 x 768 Bildpunkte nicht unterschreiten |

## DAVINCI INFOSERVER

| DAVINCI INFOSERVER | Kompatibilität |
| -- | -- |
| **Betriebssysteme** | Windows Server 2008 R2/2012/2016/2019/2022|
| **Webserver** | Windows InternetInformationServer 7/7.5/8/8.5/10 und Apache 32-Bit|

## DAVINCI MOBILE APP

| DAVINCI MOBILE APP| Kompatibilität|
| -- | -- |
| **Betriebssystem der Android-Mobilgeräte** | mindestens Android 4.4.3 ( mit WebView Chromium Engine Version 33) |
| **Betriebssystem der IOS-Mobilgeräte**| mindestens IOS 9.0|

### Wartezeit

Die Dauer, die benötigt wird um Daten auf der App anzuzeigen, kann man berechnen.

Ein Beispiel:
Für eine Datei mit rund 100 Klassen, 100 Lehrern, 850 Veranstaltungen und 1200 Terminen ergibt sich ein zu übertragenes Datenvolumen von rund 1,1 MB.

Diese Menge ist bei der ersten Anfrage der App zu übertragen und auch in dem Fall, dass es eine Änderung (zum Beispiel eine neue Vertretung) gibt. Fragt die App erneut an, es gibt aber keine Änderung, gibt es auch nichts zu übertragen.

Je schneller die Verbindung (von der App zum Internet/lokales Netzwerk und zwischen der Schule und dem Internet/lokales Netzwerk) ist, desto weniger Zeit wird für die Übertragung benötigt.

Beispiel 1:

Lokales Netzwerk über WLan
Der Server braucht circa 1 bis 2 Sekunden um die Antwort vorzubereiten, das lokale Netzwerk braucht deutlich weniger als 1 Sekunde um die Daten zu übertragen. In rund 3 Sekunden hätte man den Plan auf dem Display, wenn die Anfrage aus dem lokalen Netzwerk kommt.
Werden zahlreiche Anfragen zeitgleich gestellt (z.b.: um 7:30 Uhr, 100 Lehrer...), würde ein Datenvolumen von insgesamt etwa 80 MB zu übertragen sein. Bis für alle Kollegen die Daten auf die Geräte im Schul-WLan (802.11N) übertragen werden, dauert es rund 5 Sekunden.

Beispiel 2:

Schule nutzt eine ADSL Verbindung (Download 16 Mb/s, **Upload 1 Mb/s**); App auf dem Mobilgerät verfügt über 4G (Download 30 Mb/s): man wartet auf die Erstanfrage oder die Antwort nach einer Änderung circa 8s.
Werden von unterwegs per Mobilgerät zahlreiche Anfragen zeitgleich gestellt (z.b.: um 7:40 Uhr, 80 Lehrer...), würde auch ein Datenvolumen von insgesamt etwa 80 MB zu übertragen sein. Bis für alle Kollegen die Daten auf die Geräte übertragen von der Schule (durch ADSL Uplink) werden, dauert es rund 10 Minuten.

!!! danger "Achtung"

    Das Nadelöhr an dieser Stelle ist also die Uploadgeschwindigkeit, hier kann man die Wartezeit deutlich beeinflussen.
