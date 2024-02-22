# Welche Vertretungsinformationen werden für DAVINCI LOOK oder die WEBBOX publiziert

Nicht alle in DAVINCI erkennbaren Plan- oder Vertretungsinformationen werden in LOOK oder der WEBBOX sichtbar. Letztlich sollen beispielsweise bezogen auf Vertretungsplaneinträge die Betroffenen über die abschließende Regelung informiert werden - nicht über den Zwischenstand.
Nachstehend finden Sie verschiedene Szenarien und das jeweilige Ergebnis der Publikationsmodule.

!!! info "Hinweis"

    1. Alle Beispiele für die WEBBOX werden mit der Rechtegruppe `Masterplaner` betrachtet, Abweichendes wird gesondert angemerkt.
    2. Wir gehen nachfolgend nicht auf unveröffentlichte Informationen ein. Es ist in allen Beispielen entweder der Punkt "Änderungen freigeben" (Plan > Eigenschaften > Datenschutz) NICHT aktiviert oder die Änderungen wurden gezielt freigegeben.

!!! danger "Achtung"

    In der DAVINCI WEBBOX oder DAVINCI APP werden Veranstaltungen oder Änderungen an diesen Veranstaltungen gezeigt. Eine Veranstaltung besteht mindestens aus einem **Fach**, einem **Lehrer** und einer **Klasse**. 
    
    **Veranstaltungen ohne Fach, Lehrer oder ohne Klasse können nicht gezeigt werden.** Legen Sie sich für diese Situationen ggfs. Platzhalter in den Stammdaten an.

## Verschiedene Zeitrahmen in DAVINCI

Problem:

Sie arbeiten mit individuellen Zeitrahmen für die Kollegen und für die Klassen. In der WEBBOX/App kann aber rein logisch nur ein Zeitrahmen gezeigt werden, dafür wird der `Hauptzeitrahmen` genutzt. Liegt eine Veranstaltung außerhalb dieses Zeitrahmes oder minimal innerhalb des Zeitrahmens wird sie nicht oder nur schwer erkennbar dargestellt.

Hintergrund:

Wir stellen die Veranstaltungen in der Höhe anteilig der Dauer dar.

Beispiel:

Sie haben im Standardzeitrahmen eine Position von 9:00 bis 9:45 definiert, die nächste Position geht von 10:00 bis 10:45 Uhr, dazwischen liegt eine viertel Stunde Pause, laut `Hauptzeitrahmen`. Im Klassenzeitrahmen haben Sie etwas anderes definiert, hier kann auch eine Veranstaltung von 09:45 bis 10:00 Uhr gehen, diese Veranstaltung kann innerhalb des `Hauptzeitrahmens` in der Webbbox/App nicht dargestellt werden.
Dauert die Veranstaltung von 9:45 bis 10:00 Uhr ist der darstellbare Zeitraum (5 min) so winzig, dass die Inhalte nur schwer lesbar sein werden.

Was können Sie tun:

In diesem Fall müssten allen Kollegen/Klassen individuelle Zeitrahmen (ein Positionsraster mit Pausenzeiten) zugewiesen werden. Der `Hauptzeitrahmen` wird dann so abgeändert, dass alle Zeiten abgedeckt sind, also keine Pausenzeiten (= Lücken) entstehen. Damit können dann alle Veranstaltungen der WEBBOX/App gezeigt werden.

## Sperrung und Sperrungsbemerkung

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |sichtbar
LOOK (Klassenplan)|sichtbar
WEBBOX Planansicht (Lehrerplan)| nicht sichtbar
WEBBOX Planansicht (Klassenplan)|nicht sichtbar
WEBBOX Vertretungsliste| nicht sichtbar

## Offene Lehrerfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |sichtbar
LOOK (Klassenplan)| sichtbar
WEBBOX Planansicht (Lehrerplan)| sichtbar, außer mit Klassen- oder Schülerrechten
WEBBOX Planansicht (Klassenplan) |sichtbar, außer mit Klassen- oder Schülerrechten
WEBBOX Vertretungsliste| nicht sichtbar

## Offene Lehrerfehlzeit (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |nicht sichtbar
LOOK (Klassenplan)| nicht sichtbar
WEBBOX Planansicht (Lehrerplan) |nicht sichtbar
WEBBOX Planansicht (Klassenplan)| nicht sichtbar
WEBBOX Vertretungsliste| nicht sichtbar

## Fehlgründe

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |optional sichtbar (`DAVINCI > Plan > Eigenschaften > Datenschutz`)
LOOK (Klassenplan)| optional sichtbar (`DAVINCI > Plan > Eigenschaften > Datenschutz`)
WEBBOX Planansicht (Lehrerplan) |nicht sichtbar
WEBBOX Planansicht (Klassenplan)| nicht sichtbar
WEBBOX Vertretungsliste| nicht sichtbar

## Klassenfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |sichtbar
LOOK (Klassenplan) |sichtbar
WEBBOX Planansicht (Lehrerplan) |sichtbar
WEBBOX Planansicht (Klassenplan)|sichtbar
WEBBOX Vertretungsliste |sichtbar

## Klassenfehlzeit (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |nicht sichtbar
LOOK (Klassenplan)| nicht sichtbar
WEBBOX Planansicht (Lehrerplan) |nicht sichtbar
WEBBOX Planansicht (Klassenplan)| nicht sichtbar
WEBBOX Vertretungsliste |nicht sichtbar

## Zusatzunterricht (öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |sichtbar
LOOK (Klassenplan)|sichtbar
WEBBOX Planansicht (Lehrerplan) |sichtbar
WEBBOX Planansicht (Klassenplan) |sichtbar
WEBBOX Vertretungsliste |sichtbar

## Zusatzunterricht (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK |nicht sichtbar
WEBBOX Planansicht|nicht sichtbar
WEBBOX Vertretungsliste |nicht sichtbar

## Mitteilung

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) | sichtbar
LOOK (Klassenplan)|sichtbar
WEBBOX Planansicht (Lehrerplan)|sichtbar
WEBBOX Planansicht (Klassenplan)|sichtbar
WEBBOX Übersicht aller Klassen|nur Mitteilungen sichtbar, <br/>die nicht für **alle** Klassen/Lehrer erfasst wurde
WEBBOX Vertretungsliste|sichtbar

## Bemerkungen der Veranstaltung

Erfassbar unter `Stundenplan > Veranstaltungsliste > Rechtsklick auf eine Veranstaltung > Veranstaltung bearbeiten > Veranstaltung > Bemerkung`.

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) | sichtbar
LOOK (Klassenplan)|sichtbar
WEBBOX Planansicht (Lehrerplan)|nicht sichtbar
WEBBOX Planansicht (Klassenplan)|nicht sichtbar
WEBBOX Übersicht aller Klassen|nicht sichtbar
WEBBOX Vertretungsliste|nicht sichtbar

## Offene Raumfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |sichtbar
LOOK (Klassenplan)|sichtbar
WEBBOX |sichtbar, wenn eine Veranstaltung betroffen ist
WEBBOX Vertretungsliste|nicht sichtbar

## Offene Raumfehlzeit (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan)| nicht sichtbar
LOOK (Klassenplan) |nicht  sichtbar
WEBBOX |nicht sichtbar
WEBBOX Vertretungsliste|nicht sichtbar

## Vertretene Lehrerfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan) |sichtbar
LOOK (Klassenplan)|sichtbar
WEBBOX Planansicht (Lehrerplan)|sichtbar
WEBBOX Planansicht (Klassenplan)|sichtbar
WEBBOX Vertretungsliste|sichtbar

## Vertretene Lehreraufsicht (öffentlich)

Stelle|Sichtbarkeit
--|--
LOOK (Lehrerplan)| sichtbar
WEBBOX Planansicht (Lehrerplan)| sichtbar
WEBBOX Vertretungsliste| sichtbar

## Raumbuchung (über DAVINCI LOOK)

Stelle|Sichtbarkeit
--|--
LOOK |sichtbar
WEBBOX Planansicht|nicht sichtbar
WEBBOX Vertretungsliste |nicht sichtbar

## Aufsichten

Stelle|Sichtbarkeit
--|--
LOOK |sichtbar
WEBBOX Planansicht|sichtbar
Mobile App| sichtbar

## Aufsichten Vertretungen

Stelle|Sichtbarkeit
--|--
LOOK |sichtbar
WEBBOX Planansicht|sichtbar
WEBBOX Vertretungsliste |sichtbar
Mobile App| sichtbar
Mobile App Vertretungsliste| sichtbar
