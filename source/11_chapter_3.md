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

Um die Suchfunktion zu starten, kann die Suchleiste entweder durch das Anklicken eines Suchsymbols aufgerufen oder direkt angezeigt werden. Wenn die Suche in einer Anwendung im Vordergrund steht, ist es empfehlenswert, die Suchleiste sofort anzuzeigen. Ist die Suche hingegen optional, kann ein kontextbezogenes Suchsymbol verwendet werden. [@holstECommerceSearchField2014]

<!-- aus Quelle [holstECommerceSearchField2014]: 
- To a large extent users see the prominence of the search field as an indicator of how strongly the site “recommends” search as a way to find products, versus the alternative of navigating categories via the site menus. If search is relatively crucial, such as in an eCommerce app (studies show that shoppers who start by searching tend to convert better), a search bar is the right choice. If search is more optional, you can tone down its emphasis by substituting a clickable contextual search icon
- During our usability testing the subjects adopted search as their primary product finding strategy much more frequently on sites that had a very prominent search field, while the test sites with a muted search field design saw increased category navigation. -->

Ein weiterer Trend, der sich bei den Suchfunktionen abzeichnet, sind Sprachfunktionen. So wurden 2016 20 % der Google-Suchanfragen über die Sprachfunktion getätigt [@GoogleAppVoice2016]. Laut einer Studie im Jahr 2018 tätigen die Handynutzer mit 27% die meisten Suchanfragen mit Sprachfunktion bzw. Sprachbefehlen, gefolgt von Table- oder PC-Nutzern. Es wurde festgestellt, dass jüngere Nutzer öfter Sprachsuche oder Sprachbefehl-Tools verwendet haben. [@VoiceSearch2018]

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

*ToDo: hier klären, wie diese "eigenen" Aufnahmen zitiert werden*
*Todo: hier Bilder einfügen!*

Um einen Überblick über typische Suchfunktionen in mobilen Anwendungen zu erlangen, werden im Folgenden die Suchfunktionen von Apps aus verschiedenen Anwendungsbereichen analysiert. Ziel dieser Analyse ist die Entwicklung eines Verständnis für die Konzepte und Funktionen von In-App-Suchfunktionen.

Die Suchfunktion der 'Einstellungen'-App von Apple für iOS ermöglicht die Suche nach spezifischen Begriffen, die in das am Seitenanfang befindliche Suchfeld eingegeben werden. Hierbei durchsucht die App sämtliche Inhalte der Einstellungen. In der Version der Softwarestufe iOS 17 werden während der Eingabe Suchergebnisse angezeigt, ohne dass eine explizite Bestätigung der Eingabe durch den Nutzer erforderlich ist. Die Suche generiert eine Liste mit treffenden Ergebnissen, wobei der Titel des zugehörigen Feldes innerhalb der App, ein zugehöriges Symbol und teilweise der Pfad angegeben werden. Durch Anklicken eines Ergebnisses wird die entsprechende Seite geöffnet bzw. der gesamte Pfad, wobei das zugehörige Feld kurzzeitig grau hervorgehoben wird. Navigiert man zurück, gelangt man wenn im Pfad vorhanden auf eine Oberseite, bevor man wieder auf das Suchfenster zurückkommt. [@EinstellungenAppIPhone2024]

Ab iOS 18 werden vor der Eingabe in das Suchfeld Such-Vorschläge durch große Symbole und Text angezeigt und darunter der Verlauf der aufgerufenen Suchergebnisse. [@EinstellungenAppIPhone2025]

Die 'Einstellungen'-App von Android kann ebenfalls nach Begriffen durchsucht werden. Nach Anklicken des Such-Icons wird die Such-Seite geöffnet, in der vergangene Suchen und allgemeine Suchvorschläge aufgelistet sind. Den Vorschläge geht ein Rauten-Symbol vor, wodurch nach Themen und nicht nach konkreten Begriffen gesucht werden kann, wie etwa "beliebt". Während der Eingabe in das Suchfeld werden dann anstelle dessen die Suchergebnisse für die aktuelle Eingabe angezeigt. Diese sind in beliebte und restliche Ergebnisse aufgeteilt, die jeweils in ihre zugehörigen Kategorien gruppiert sind. Durch Anklicken eines Ergebnisses wird die entsprechende Seite innerhalb der 'Einstellungen'-App geöffnet. Durch Betätigen der 'Zurück'-Taste des Handys, gelangt man in die Suchfunktion. Durch Betätigung des 'Zurück'-Button in der Leiste oben, geht man dem der Seite zugehörigen Pfad entlang zurück. [@EinstellungenAppAndroid]

<!-- App 'Einstellungen' von Apple für iPhone [@EinstellungenApp2024]
- Suche nach Stichwörtern möglich, alle Ergebnisse aufgelistet, bei Auswahl davon "springt" man in den richtigen Ort (+Pfad) in der App  -->
Die App 'Instagram' bietet für den Einstellungen-Bereich der App eine Suchfunktion an, mit der die Inhalte dieses Bereiches durchsucht werden können. Bei der Eingabe von Suchbegriffen werden die Suchergebnisse in verschiedenen Gruppen untereinander bereits während des Tippens, ohne explizite Bestätigung, angezeigt. Diese Gruppierung entspricht der Kategorisierung, die in den Einstellungen verwendet wird. Beim Anklicken eines Ergebnisses wir direkt die entsprechende Unterseite geöffnet. Es sei jedoch angemerkt, dass nicht alle in den Einstellungen dargestellten Inhalte durch die Suche auffindbar sind. [@InstagramEinstellungen2025]

<!-- App 'Instagram', Einstellungen [@InstagramEinstellungen]
- Instagram-Einstellungen: Liste von Einstellungsmöglichkeiten, Suchbegriffe von dieser Liste eingeben und die werden angezeigt, nichts "dahinter" -->

<!-- Chrome, Einstellungen [@ChromeEinstellungen2024]
- Bei Eingabe von Keyword: Ergebnisse in Kategorien unterteilt + Anzeige, wie viele Ergebnisse pro Suchergebis sind. Nicht mobil!!-->

Die untersuchten Apps setzen viele der zuvor erhobenen Anforderungen um. Häufig gibt es einen Übergangsbildschirm, der Vorschläge und vergangene Suchanfragen anzeigt. Während des Tippens werden jedoch oft nur die Ergebnisse für den aktuellen Stand des Suchbegriffs angezeigt, ohne dass Vorschläge für eine automatische Vervollständigung angeboten werden. Zudem wurden die Suchergebnisse auf den Seiten nur teilweise explizit hervorgehoben. Es besteht auch keine Konsistenz darin, ob die Suchfunktion über eine Suchleiste oder ein Suchsymbol aufgerufen wird. Insgesamt zeigen sich sowohl Übereinstimmungen als auch Unterschiede in den Implementierungen der Suchfunktionen.

## Ist-Analyse der vorhandenen Daten und Datenquellen

Um eine umfassende Suche durch verschiedene Bereiche der App zu ermöglichen, werden die Daten aus verschiedenen Quellen angebunden.

Die Texte, die in der MyBMW-App verwendet werden, beispielsweise in Buttons, Menüpunkten oder anderen Anzeigekomponenten, sind in sogenannten 'String Files' gespeichert. Diese Dateien ermöglichen es, die Anwendung in verschiedenen Sprachen darzustellen, indem die Texte in der jeweiligen Sprache aus der entsprechenden Datei geladen werden.
Jeder Text ist mit einer eindeutigen ID versehen, die es ermöglicht, die Texte den verschiedenen Diensten innerhalb der App zuzuordnen. Jeder Dienst hat dabei einen zugehörigen Pfad, der dann auf die entsprechende Seite des Dienstes führt.
Im Rahmen der Implementierung der Suchfunktion sollen exemplarisch zwei Dienste der MyBMW-App an die Suchfunktion angebunden werden. Diese Daten werden im Weiteren als 'String-File'-Daten bezeichnet.

Zusätzlich wird eine dynamische Quelle integriert, die über die App bereitgestellt und über den 'Context' geladen werden kann. Diese Quelle umfasst die Artikel, die auf der Explore-Seite der MyBMW-App dargestellt werden, und bietet somit aktuelle Inhalte für die Suche. Diese Daten werden als Kontext-Daten bezeichnet.

Darüber hinaus werden lokale Daten in Form einer JSON-Datei in die Suche integriert. In dieser prototypischen Umsetzung enthält die JSON-Datei Datensätze zu 'My Highlights', die besondere Änderungen bei RSU für die Kunden hervorheben. Diese Daten werden als Lokale-Daten referenziert.

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
