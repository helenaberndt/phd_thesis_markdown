# Vorbereitung und Analyse / Explorative Phase

## Recherche und Analyse ähnlicher Suchfunktionen

Informationen zu, Anforderungsmanagement in [@nunkesserAppEntwicklungFuerMobile2023] (Seite 41)

### Analyse des Suchfunktions-Angebots innerhalb Automobil-Apps der Wettbewerber

Quellen: [@AppStoreMercedesBenz2024],[@AppStoreMyAudi2024],[@AppStoreTesla2024],[@AppStoreVolkswagen2024],[@AppStoreVolvo2024]

- Betrachtete Automobilhersteller-Apps: myAudi, Volvo Cars, MercedesMe, Volkswagen, Tesla
- alle haben ähnliche Funktionen wie My BMW App:
    - Remote Funktionen: Klima einsehen und steuern, Fahrzeug entriegeln etc.
    - Fahrzeugstatus abrufen: Reifendruck, Reichweite etc.
    - Routen planen, Standort einsehen
    - aber: keine der Apps hat Funktion, mit der die App nach Stichwörtern durchsucht werden kann

### Analyse des Suchfunktions-Angebots innerhalb Apps anderer Branchen

Beispiele: 

App 'Einstellungen' von Apple für iPhone [@EinstellungenApp2024]
- Suche nach Stichwörtern möglich, alle Ergebnisse aufgelistet, bei Auswahl davon "springt" man in den richtigen Ort (+Pfad) in der App 

App 'Instagram', Einstellungen [@InstagramEinstellungen]
- Instagram-Einstellungen: Liste von Einstellungsmöglichkeiten, Suchbegriffe von dieser Liste eingeben und die werden angezeigt, nichts "dahinter"

Chrome, Einstellungen [@ChromeEinstellungen2024]
- Bei Eingabe von Keyword: Ergebnisse in Kategorien unterteilt + Anzeige, wie viele Ergebnisse pro Suchergebis sind

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