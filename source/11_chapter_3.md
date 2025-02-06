# Vorbereitung und Analyse der Ausgangssituation
 <!-- / Explorative Phase -->

Im Vorfeld der eigentlichen Konzeption der Suchfunktion erfolgt zunächst eine umfassende Analyse der Ausgangssituation, um diese zu verstehen. Zunächst werden allgemeine Funktionen und Anforderungen zusammengefasst, die üblicherweise an eine moderne Suchfunktion gestellt werden. Im Anschluss daran werden vergleichbare Suchfunktionen in Automotive-Apps sowie in anderen Anwendungsbereichen analysiert und mit den Anforderungen abgeglichen. Abschließend wird der Ist-Zustand der vorhandenen Daten und Datenquellen betrachtet.

## Allgemeine Funktionen und Anforderungen an eine Suchfunktion

Bei der Entwicklung von Suchfunktionen in mobilen Anwendungen sollten bewährte Verfahren, auch bekannt als 'Best Practices', in die Konzeption einfließen. Oftmals verfügen Suchfunktionen über einen Übergangsbildschirm, der vergangene Suchanfragen, trendige Suchbegriffe oder vordefinierte Kategorien anzeigt. Eine Filtermöglichkeit ist besonders sinnvoll, wenn relevante Daten vorhanden sind.
Bei der Eingabe von Suchbegriffen wird häufig eine Autovervollständigung angeboten, die Vorschläge für mögliche Suchanfragen liefert. Dabei werden häufig auch Schreibfehler toleriert, um die Benutzerfreundlichkeit zu erhöhen. In den Suchergebnissen können die eingegebenen Suchwörter durch eine Markierung hervorgehoben werden, was die Übersichtlichkeit verbessert.
Die Integration von Künstlicher Intelligenz kann in bestimmten Anwendungsfällen von Suchfunktionen von Vorteil sein, beispielsweise zur Schaffung eines personalisierten Einkaufserlebnisses. Letztlich ist es entscheidend, dass die Erwartungen der Nutzer an die Geschwindigkeit der Suchfunktion erfüllt werden, um eine positive Benutzererfahrung zu gewährleisten.[@deeBestPracticesInapp2024]

<!-- Quelle [@deeBestPracticesInapp2024]:Mobile Suche und Discovery - wie UX
- "Less is more", simples Design für kleinen Bildschirm
- man möchte relevante Inhalte (content) geben, der Nutzer nicht überfordert (overwhelm) oder dazu führt, dass Nutzer die Suche weiter verfeinern müssen
- Im 'Search Transition Screen' Recent searches, Trending, Categories, Instant results, Query suggestions bzw. Autocomplete
- Allgemein: Typo Tolerance
- AI teilweise sinnvoll, z.B. bei Suchfunktion für personalisierte Einkaufs-Experience
- best practices: Erwartungen von Nutzern an Schnelligkeit müssen erfüllt werden, Filter wenn sinnvoll, nach Relevanz sortiert, Suchtext in Ergebnissen mit Highlight/Markierung hervorheben -->

Um die Suchfunktion zu starten, kann die Suchleiste entweder durch das Anklicken eines Suchsymbols aufgerufen oder direkt angezeigt werden. Wenn die Suche in einer Anwendung im Vordergrund steht, ist es empfehlenswert, die Suchleiste sofort anzuzeigen. Ist die Suche hingegen optional, kann ein kontextbezogenes Suchsymbol verwendet werden. [holstECommerceSearchField2014]

<!-- aus Quelle [holstECommerceSearchField2014]: 
- To a large extent users see the prominence of the search field as an indicator of how strongly the site “recommends” search as a way to find products, versus the alternative of navigating categories via the site menus. If search is relatively crucial, such as in an eCommerce app (studies show that shoppers who start by searching tend to convert better), a search bar is the right choice. If search is more optional, you can tone down its emphasis by substituting a clickable contextual search icon
- During our usability testing the subjects adopted search as their primary product finding strategy much more frequently on sites that had a very prominent search field, while the test sites with a muted search field design saw increased category navigation. -->

*todo: voice search*

## Recherche und Analyse vergleichbarer Suchfunktionen

<!-- Informationen zu, Anforderungsmanagement in [@nunkesserAppEntwicklungFuerMobile2023] (Seite 41) -->

Im Folgenden werden zunächst Apps von Automobilherstellern, die als direkte Wettbewerber der MyBMW-App angesehen werden können, näher betrachtet [@WettbewerbsanalyseMethodenUnd2022]. Dabei wird ein besonderer Fokus auf eventuell vorhandene Suchfunktionen gelegt.
Anschließend erfolgt eine allgemeine Analyse von Suchfunktionen in Apps, die einen Überblick über typische Konzepte und Funktionen liefert.

### Suchfunktionen in Automotive Apps

Eine Analyse der von den Automarken Mercedes, Audi, Tesla, Volkswagen und Volvo angebotenen Apps zeigt, dass sie mit der MyBMW App vergleichbar sind. Die Untersuchung der Funktionalitäten der Wettbewerber-Apps ergibt, dass die Grundfunktionen ähnlich sind. Dazu gehören Remote-Funktionen, mit denen das aktuelle Klima eingesehen und gesteuert werden kann, sowie die Möglichkeit, Fahrzeuge über das Handy zu entriegeln und den Fahrzeugstatus abzurufen. Zusätzlich haben Kunden die Möglichkeit, den aktuellen Standort des Autos zu überprüfen und Routen zu planen. Die Analyse der im App Store sichtbaren Funktionen ergab jedoch, dass keine der untersuchten Apps über eine Suchfunktion verfügt, die eine Suche nach Stichwörtern ermöglicht. [@AppStoreMercedesBenz2024],[@AppStoreMyAudi2024],[@AppStoreTesla2024],[@AppStoreVolkswagen2024],[@AppStoreVolvo2024]

*todo: diese quellen sind eigene quellen -> in den anhang?*

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
<!-- Todo: hier Bilder einfügen! -->

------ hier weiter ------

Um einen Überblick über typische Suchfunktionen in Apps zu erhalten, werden im Folgenden die Suchfunktionen von Apps aus verschiedenen Anwendungsbereichen analysiert. Ziel dieser Analyse ist es, ein Verständnis für die Konzepte und Funktionen von In-App-Suchfunktionen zu entwickeln.

Mit der Suchfunktion in der 'Einstellungen'-App von Apple für iOS kann diese nach Suchbegriffen durchsucht werden, indem in das am Seitenanfang befindende Suchfeld Begriffe eingegeben werden. Dabei werden alle Inhalte der App durchsucht. In der Version der Softwarestufe iOS 17 erscheinen während des Tippens Suchergebnisse - die Suche muss als nicht explizit getätigt werden. Untereinander werden passende Ergebnisse angezeigt, wobei der Titel des zugehörigen Feldes innerhalb der App, ein zugehöriges Symbol und teilweise der Pfad angegeben wird. Beim Klicken auf ein Ergebnis wird die entsprechende Seite geöffnet, beziehungsweise der gesamt Pfad, wobei das zugehörige Feld kurzzeitig grau hervorgehoben wird. Navigiert man wieder zurück, kommt man zunächst auf die Oberseite, bevor man dann auf das Suchfenster zurück kommt. [@EinstellungenAppIPhone2024]

Ab iOS 18 werden vor der Eingabe in das Suchfeld Such-Vorschläge angezeigt und darunter der Suchverlauf der betätigten Eingabe. [@EinstellungenAppIPhone2025]

Die 'Einstellungen' App von Android kann ebenfalls durchsucht werden. Nach Klicken auf ein Such-Icon wird eine Seite geöffnet, in der vergangene Suchen und allgemeine Suchvorschläge. Diesen Vorschläge geht ein Rauten-Symbol vor, wodurch nach Themen wie 'beliebt' und keinen konkreten Begriffen gesucht werden kann. Während der Eingabe in das Suchfeld werden dann anstelle dessen die Suchergebnisse angezeigt. Diese sind in beliebte Vorschläge <!-- Top Hits --> und restliche Ergebnisse aufgeteilt, die in die zugehörigen Kategorien gruppiert sind. Drückt man auf ein Ergebnis, öffnet sich die entsprechende Seite. Bei Betätigung der 'Zurück' Taste des Handys, gelangt man in die Suchfunktion, drückt man den 'Zurück' Button, geht man dem der Seite entsprechenden Pfad entlang zurück.  [@EinstellungenAppAndroid]

<!-- App 'Einstellungen' von Apple für iPhone [@EinstellungenApp2024]
- Suche nach Stichwörtern möglich, alle Ergebnisse aufgelistet, bei Auswahl davon "springt" man in den richtigen Ort (+Pfad) in der App  -->
Die App 'Instagram' bietet für den Einstellungen-Bereich eine Suchfunktion an, mit der die Inhalte dieses Bereiches durchsucht werden können. Bei der Eingabe von Suchbegriffen werden die Suchergebnisse in verschiedenen Gruppen untereinander angezeigt. Diese Gruppierung entspricht der Kategorisierung, die in den Einstellungen verwendet wird. Beim Klicken auf ein Ergebnis wir direkt die entsprechende Unterseite geöffnet. Es fällt auf, dass nicht alle in den Einstellungen gezeigten Inhalte ebenfalls durch die Suche auffindbar sind. [@InstagramEinstellungen2025]

<!-- App 'Instagram', Einstellungen [@InstagramEinstellungen]
- Instagram-Einstellungen: Liste von Einstellungsmöglichkeiten, Suchbegriffe von dieser Liste eingeben und die werden angezeigt, nichts "dahinter" -->


<!-- Chrome, Einstellungen [@ChromeEinstellungen2024]
- Bei Eingabe von Keyword: Ergebnisse in Kategorien unterteilt + Anzeige, wie viele Ergebnisse pro Suchergebis sind. Nicht mobil!!-->



## Ist-Analyse der vorhandenen Daten und Datenquellen

Die Daten, die an die Suchfunktion angebunden werden sollen, stammen aus unterschiedlichen Quellen, um eine möglichst umfassende Suche zu ermöglichen.

Texte, die in der MyBMW-App verwendet werden, beispielsweise in Buttons, Menüpunkten oder anderen Anzeigekomponenten, sind in sogenannten 'String Files' gespeichert. Diese Dateien dienen dazu, die Anwendung in verschiedenen Sprachen darstellen zu können. Dafür werden die Texte in der jeweiligen Sprache aus der entsprechenden Datei geladen.
Jeder dieser Texte ist mit einer eindeutigen ID versehen. Über diese IDs können die Texte den verschiedenen Diensten innerhalb der App zugeordnet werden.
Im Rahmen der Implementierung der Suchfunktion sollen exemplarisch zwei dieser Dienste an die Suchfunktion angebunden werden.

Darüber hinaus soll eine dynamische Quelle an die Suche eingebunden werden, die über die App bereitgestellt und über den 'Context' geladen werden kann. Die Artikel die in der 'Explore'-Seite dargestellt werden, sind dafür passend.

Außerdem sollen noch lokale Daten in Form einer JSON-Datei in die Suche integriert werden. In dieser prototypischen Umsetzung enthält diese JSON-Datei Daten für die 'My Highlights', die besondere Änderungen bei Remote Software Upgrade für die Kunden hervorheben.

<!-- Explore Tab:
aktueller: Könnte ich hernehmen und erweitern, wo die Daten herkommen (Theresa gefragt)
- neuer: gibt es noch nicht. ich könnte ihn mir "nachbasteln" und eigene Daten (z.B. in JSON) selber erzeugen
- Ich nehme die aktuellen Daten her

Nach Gespräch mit Jonas:
- erst mal in der aktuellen Explore Seite einbauen
- wenn das nicht geht -> selber bauen

- fehlt: Informationen über Daten innerhalb von Explore Seite

My Highlights:
- aktuell nur ein einziges File immer lokal vorhanden, Link zu Format: https://atc.bmwgroup.net/confluence/display/INFOTAIN/My+Highlights+Service+-+Back-End+Data+Model -> JSON 

Release Notes:
- gerade im Umbau -> erst mal lassen, sollen aber das gleiche Format wie My Highlights bekommen
 -->

