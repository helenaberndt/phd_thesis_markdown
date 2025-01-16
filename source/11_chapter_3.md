# Vorbereitung und Analyse
 <!-- / Explorative Phase -->

## Recherche und Analyse vergleichbarer Suchfunktionen

<!-- Informationen zu, Anforderungsmanagement in [@nunkesserAppEntwicklungFuerMobile2023] (Seite 41) -->

Um einen Vergleichswert zwischen bereits bestehenden Suchfunktionen in vergleichbaren Apps wurden Apps aus der Automobilbranche und Apps aus anderen Bereichen mit Suchfunktion evaluiert.

### Suchfunktionen in Automotive Apps

Die Automarken Mercedes, Audi, Tesla, Volkswagen und Volvo stellen Ihren Kunden Apps zur Verfügung, die mit der MyBMW App vergleichbar sind. So können bei den Wettbewerber-Apps gleiche Grundfunktionalitäten ausgeführt werden: über Remote-Funktionen kann das aktuelle Klima eingesehen und gesteuert, Fahrzeuge können über das Handy entriegelt oder der Fahrzeugstatus abgerufen werden. Außerdem können Kunden den aktuellen Standort des Autos einsehen und Routen planen. Nach Sichtung der über den App Store sichtbaren Funktionen konnte für keines der App-Beispiele eine Suchfunktion ausgemacht werden, die Inhalte der Apps nach Stichwörtern durchsuchen kann. [@AppStoreMercedesBenz2024],[@AppStoreMyAudi2024],[@AppStoreTesla2024],[@AppStoreVolkswagen2024],[@AppStoreVolvo2024]

<!-- Info: das sind Wettbewerber

Quellen: [@AppStoreMercedesBenz2024],[@AppStoreMyAudi2024],[@AppStoreTesla2024],[@AppStoreVolkswagen2024],[@AppStoreVolvo2024]

- Betrachtete Automobilhersteller-Apps: myAudi, Volvo Cars, MercedesMe, Volkswagen, Tesla
- alle haben ähnliche Funktionen wie My BMW App:
    - Remote Funktionen: Klima einsehen und steuern, Fahrzeug entriegeln etc.
    - Fahrzeugstatus abrufen: Reifendruck, Reichweite etc.
    - Routen planen, Standort einsehen
    - aber: keine der Apps hat Funktion, mit der die App nach Stichwörtern durchsucht werden kann -->

### Suchfunktionen in Apps anderer Bereiche

<!-- ToDo: hier klären, wie diese "eigenen" Aufnahmen zitiert werden -->

Bei Apps, die keine Ähnlichkeit zur MyBMW-App aufzeigen, sind teilweise Suchfunktionen für den Nutzer verfügbar.

So kann die 'Einstellungen'-App von Apple für iOS nach Suchbegriffen durchsucht werden, indem in das am Seitenanfang befindende Suchfeld Begriffe eingegeben werden können. Dabei werden alle Inhalte der App durchsucht. In der Version der Softwarestufe iOS 17 erscheinen während des Tippens Suchergebnisse - die Suche muss als nicht explizit getätigt werden. Untereinander werden passende Ergebnisse angezeigt, wobei der Titel des zugehörigen Feldes innerhalb der App, ein zugehöriges Symbol und teilweise der Pfad angegeben wird. Beim Klicken auf ein Ergebnis wird die entsprechende Seite geöffnet, beziehungsweise der gesamt Pfad, wobei das zugehörige Feld kurzzeitig grau hervorgehoben wird. Navigiert man wieder zurück, kommt man zunächst auf die Oberseite, bevor man dann auf das Suchfenster zurück kommt.   [@EinstellungenApp2024]
Ab iOS 18 werden vor der Eingabe in das Suchfeld Such-Vorschläge angezeigt und darunter der Suchverlauf der betätigten Eingabe. [EinstellungenAppIPhone2025]

Die 'Einstellungen' App von Android kann ebenfalls durchsucht werden. Nach Klicken auf ein Such-Icon wird eine Seite geöffnet, in der vergangene Suchen und allgemeine Suchvorschläge. Diesen Vorschläge geht ein Rauten-Symbol vor, wodurch nach Themen wie 'beliebt' und keinen konkreten Begriffen gesucht werden kann. Während der Eingabe in das Suchfeld werden dann anstelle dessen die Suchergebnisse angezeigt. Diese sind in beliebte Vorschläge <!-- Top Hits --> und restliche Ergebnisse aufgeteilt, die in die zugehörigen Kategorien gruppiert sind. Drückt man auf ein Ergebnis, öffnet sich die entsprechende Seite. Bei Betätigung der 'Zurück' Taste des Handys, gelangt man in die Suchfunktion, drückt man den 'Zurück' Button, geht man dem der Seite entsprechenden Pfad entlang zurück.  [EinstellungenAppAndroid]

<!-- App 'Einstellungen' von Apple für iPhone [@EinstellungenApp2024]
- Suche nach Stichwörtern möglich, alle Ergebnisse aufgelistet, bei Auswahl davon "springt" man in den richtigen Ort (+Pfad) in der App  -->
Die App 'Instagram' bietet für den Einstellungen-Bereich eine Suchfunktion an, mit der die Inhalte dieses Bereiches durchsucht werden können. Bei der Eingabe von Suchbegriffen werden die Suchergebnisse in verschiedenen Gruppen untereinander angezeigt. Diese Gruppierung entspricht der Kategorisierung, die in den Einstellungen verwendet wird. Beim Klicken auf ein Ergebnis wir direkt die entsprechende Unterseite geöffnet. Es fällt auf, dass nicht alle in den Einstellungen gezeigten Inhalte ebenfalls durch die Suche auffindbar sind. [@InstagramEinstellungen]

<!-- App 'Instagram', Einstellungen [@InstagramEinstellungen]
- Instagram-Einstellungen: Liste von Einstellungsmöglichkeiten, Suchbegriffe von dieser Liste eingeben und die werden angezeigt, nichts "dahinter" -->


<!-- Chrome, Einstellungen [@ChromeEinstellungen2024]
- Bei Eingabe von Keyword: Ergebnisse in Kategorien unterteilt + Anzeige, wie viele Ergebnisse pro Suchergebis sind. Nicht mobil!!-->



## Ist-Analyse der vorhandenen Daten und Datenquellen

Explore Tab:
<!-- aktueller: Könnte ich hernehmen und erweitern, wo die Daten herkommen (Theresa gefragt)
- neuer: gibt es noch nicht. ich könnte ihn mir "nachbasteln" und eigene Daten (z.B. in JSON) selber erzeugen -->
- Ich nehme die aktuellen Daten her

Nach Gespräch mit Jonas:
- erst mal in der aktuellen Explore Seite einbauen
- wenn das nicht geht -> selber bauen

- fehlt: Informationen über Daten innerhalb von Explore Seite

My Highlights:
- aktuell nur ein einziges File immer lokal vorhanden, Link zu Format: https://atc.bmwgroup.net/confluence/display/INFOTAIN/My+Highlights+Service+-+Back-End+Data+Model -> JSON 

Release Notes:
- gerade im Umbau -> erst mal lassen, sollen aber das gleiche Format wie My Highlights bekommen