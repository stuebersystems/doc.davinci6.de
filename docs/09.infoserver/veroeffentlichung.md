# Welche Vertretungsinformationen werden für DaVinci Look oder die WebBox publiziert

Nicht alle in DaVinci erkennbaren Plan- oder Vertretungsinformationen werden in Look oder der WebBox sichtbar. Letztlich sollen beispielsweise bezogen auf Vertretungsplaneinträge die Betroffenen über die abschließende Regelung informiert werden - nicht über den Zwischenstand.
Nachstehend finden Sie verschiedene Szenarien und das jeweilige Ergebnis der Publikationsmodule.

!!! info "Hinweis"

    1. Alle Beispiele für die WebBox werden mit der Rechtegruppe `Masterplaner` betrachtet, Abweichendes wird gesondert angemerkt.
    2. Wir gehen nachfolgend nicht auf unveröffentlichte Informationen ein. Es ist in allen Beispielen entweder der Punkt "Änderungen freigeben" (Plan > Eigenschaften > Datenschutz) NICHT aktiviert oder die Änderungen wurden gezielt freigegeben.

!!! danger "Achtung"

    In der DaVinci WebBox oder DaVinci App werden Veranstaltungen oder Änderungen an diesen Veranstaltungen gezeigt. Eine Veranstaltung besteht mindestens aus einem **Fach**, einem **Lehrer** und einer **Klasse**. 
    
    **Veranstaltungen ohne Fach, Lehrer oder ohne Klasse können nicht gezeigt werden.** Legen Sie sich für diese Situationen ggfs. Platzhalter in den Stammdaten an.

## Verschiedene Zeitrahmen in DaVinci

Problem:

Sie arbeiten mit individuellen Zeitrahmen für die Kollegen und für die Klassen. In der WebBox/App kann aber rein logisch nur ein Zeitrahmen gezeigt werden, dafür wird der `Hauptzeitrahmen` genutzt. Liegt eine Veranstaltung außerhalb dieses Zeitrahmes oder minimal innerhalb des Zeitrahmens wird sie nicht oder nur schwer erkennbar dargestellt.

Hintergrund:

Wir stellen die Veranstaltungen in der Höhe anteilig der Dauer dar.

Beispiel:

Sie haben im Standardzeitrahmen eine Position von 9:00 bis 9:45 definiert, die nächste Position geht von 10:00 bis 10:45 Uhr, dazwischen liegt eine viertel Stunde Pause, laut `Hauptzeitrahmen`. Im Klassenzeitrahmen haben Sie etwas anderes definiert, hier kann auch eine Veranstaltung von 09:45 bis 10:00 Uhr gehen, diese Veranstaltung kann innerhalb des `Hauptzeitrahmens` in der Webbbox/App nicht dargestellt werden.
Dauert die Veranstaltung von 9:45 bis 10:00 Uhr ist der darstellbare Zeitraum (5 min) so winzig, dass die Inhalte nur schwer lesbar sein werden.

Was können Sie tun:

In diesem Fall müssten allen Kollegen/Klassen individuelle Zeitrahmen (ein Positionsraster mit Pausenzeiten) zugewiesen werden. Der `Hauptzeitrahmen` wird dann so abgeändert, dass alle Zeiten abgedeckt sind, also keine Pausenzeiten (= Lücken) entstehen. Damit können dann alle Veranstaltungen der WebBox/App gezeigt werden.

## Sperrung und Sperrungsbemerkung

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |sichtbar
Look (Klassenplan)|sichtbar
WebBox Planansicht (Lehrerplan)| nicht sichtbar
WebBox Planansicht (Klassenplan)|nicht sichtbar
WebBox Vertretungsliste| nicht sichtbar

## Offene Lehrerfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |sichtbar
Look (Klassenplan)| sichtbar
WebBox Planansicht (Lehrerplan)| sichtbar, außer mit Klassen- oder Schülerrechten
WebBox Planansicht (Klassenplan) |sichtbar, außer mit Klassen- oder Schülerrechten
WebBox Vertretungsliste| nicht sichtbar

## Offene Lehrerfehlzeit (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |nicht sichtbar
Look (Klassenplan)| nicht sichtbar
WebBox Planansicht (Lehrerplan) |nicht sichtbar
WebBox Planansicht (Klassenplan)| nicht sichtbar
WebBox Vertretungsliste| nicht sichtbar

## Fehlgründe

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |optional sichtbar (`DaVinci > Plan > Eigenschaften > Datenschutz`)
Look (Klassenplan)| optional sichtbar (`DaVinci > Plan > Eigenschaften > Datenschutz`)
WebBox Planansicht (Lehrerplan) |nicht sichtbar
WebBox Planansicht (Klassenplan)| nicht sichtbar
WebBox Vertretungsliste| nicht sichtbar

## Klassenfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |sichtbar
Look (Klassenplan) |sichtbar
WebBox Planansicht (Lehrerplan) |sichtbar
WebBox Planansicht (Klassenplan)|sichtbar
WebBox Vertretungsliste |sichtbar

## Klassenfehlzeit (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |nicht sichtbar
Look (Klassenplan)| nicht sichtbar
WebBox Planansicht (Lehrerplan) |nicht sichtbar
WebBox Planansicht (Klassenplan)| nicht sichtbar
WebBox Vertretungsliste |nicht sichtbar

## Zusatzunterricht (öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |sichtbar
Look (Klassenplan)|sichtbar
WebBox Planansicht (Lehrerplan) |sichtbar
WebBox Planansicht (Klassenplan) |sichtbar
WebBox Vertretungsliste |sichtbar

## Zusatzunterricht (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
Look |nicht sichtbar
WebBox Planansicht|nicht sichtbar
WebBox Vertretungsliste |nicht sichtbar

## Mitteilung

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) | sichtbar
Look (Klassenplan)|sichtbar
WebBox Planansicht (Lehrerplan)|sichtbar
WebBox Planansicht (Klassenplan)|sichtbar
WebBox Übersicht aller Klassen|nur Mitteilungen sichtbar, <br/>die nicht für **alle** Klassen/Lehrer erfasst wurde
WebBox Vertretungsliste|sichtbar

## Bemerkungen der Veranstaltung

Erfassbar unter `Stundenplan > Veranstaltungsliste > Rechtsklick auf eine Veranstaltung > Veranstaltung bearbeiten > Veranstaltung > Bemerkung`.

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) | sichtbar
Look (Klassenplan)|sichtbar
WebBox Planansicht (Lehrerplan)|nicht sichtbar
WebBox Planansicht (Klassenplan)|nicht sichtbar
WebBox Übersicht aller Klassen|nicht sichtbar
WebBox Vertretungsliste|nicht sichtbar

## Offene Raumfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |sichtbar
Look (Klassenplan)|sichtbar
WebBox |sichtbar, wenn eine Veranstaltung betroffen ist
WebBox Vertretungsliste|nicht sichtbar

## Offene Raumfehlzeit (nicht öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan)| nicht sichtbar
Look (Klassenplan) |nicht  sichtbar
WebBox |nicht sichtbar
WebBox Vertretungsliste|nicht sichtbar

## Vertretene Lehrerfehlzeit (öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan) |sichtbar
Look (Klassenplan)|sichtbar
WebBox Planansicht (Lehrerplan)|sichtbar
WebBox Planansicht (Klassenplan)|sichtbar
WebBox Vertretungsliste|sichtbar

## Vertretene Lehreraufsicht (öffentlich)

Stelle|Sichtbarkeit
--|--
Look (Lehrerplan)| sichtbar
WebBox Planansicht (Lehrerplan)| sichtbar
WebBox Vertretungsliste| sichtbar

## Raumbuchung (über DaVinci Look)

Stelle|Sichtbarkeit
--|--
Look |sichtbar
WebBox Planansicht|nicht sichtbar
WebBox Vertretungsliste |nicht sichtbar

## Aufsichten

Stelle|Sichtbarkeit
--|--
Look |sichtbar
WebBox Planansicht|sichtbar
Mobile App| sichtbar

## Aufsichten Vertretungen

Stelle|Sichtbarkeit
--|--
Look |sichtbar
WebBox Planansicht|sichtbar
WebBox Vertretungsliste |sichtbar
Mobile App| sichtbar
Mobile App Vertretungsliste| sichtbar
