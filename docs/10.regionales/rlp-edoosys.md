# Datenabgleich zwischen DaVinci und edoo.sys

DaVinci verfügt über eine eigene Schnittstelle zu edoo.sys RLP. Für einen erfolgreichen Datenaustausch zwischen DaVinci und edoo.sys sind einige wesentliche Schritte zu beachten.

Unter [https://svp-rlp.topdesk.net](https://svp-rlp.topdesk.net) finden Sie im Bereich ``VIDEOS ZU EDOO.SYS RLP`` ein Video, dass die Übernahme des Stundenplans aus DaVinci in die Matrix von edoo.sys beschreibt. Hierzu wird der Prozess vom Export der Stammdaten aus edoo.sys bis zum Import der Daten aus DaVinci gezeigt.

Alternativ können Sie dieses Video auch [hier](https://my.hidrive.com/share/lf7uza7klt) öffnen.

Sie können die Daten generell über einen Datenimport aus dem [Schuldatentransferformat](https://doc.sdtf.stueber.de/) einlesen. Diese Spezifikation enthält die Beschreibung des Schuldatentransferformats.

Dieses Format dient zum Datenaustausch zwischen Schulverwaltungs- und Stundenplanprogrammen, die dieses Format unterstützen. Die Informationen in dieser Datei benötigen Sie, wenn Sie z.B. selbst Daten aus DaVinci in Fremdprogramme, z.B. Datenbanken, einlesen möchten. Ferner dient dieses Format als Standard für Softwareentwickler, die ihre Schulverwaltungsdaten in andere Programme, die das Schuldatentransferformat unterstützen, exportieren bzw. von dort importieren möchten.

!!! info "Hinweis"

    Der [Datensatz P1](https://doc.sdtf.stueber.de/davinci-zeilentypen/#zeilentyp-p1) enthält die Schülerdaten. Wenn aus edoo.sys in dieser Form exportiert wird, können auch die Kurswahldaten der Schüler aus edoo.sys in DaVinci eingelesen werden. 
    Der Artikel ["Fachwahlen werden nicht übernommen (gymnasiale Oberstufe)"](https://svp-rlp.topdesk.net/tas/public/ssp/content/detail/knowledgeitem?unid=de7eb635a52740b98cee8e6f0be10b30) beschreibt, wie Schulen in DaVinci vorgehen müssen, um die Fachwahlen aus edoo.sys im Kursplan zu zeigen.


