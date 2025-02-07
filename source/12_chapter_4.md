# Konzeption

*todo: Forschungsfrage konkretisieren hier*
<!-- Überblick über die Zielsetzung der Konzeption der Suchfunktion.
Erläuterung der Relevanz der Suchfunktion innerhalb der MyBMW-App.
Beschreibung des strukturellen Aufbaus der Konzeption. -->



## Anforderungsanalyse der Suchfunktion

*todo: sollen hier auch nicht-umgesetzte sachen stehen? wenn ja hier nochmal mehr stukturieren und priorisieren - in must-haves und nice-to-haves?*

Im 'Requirements Engineering', also der Anforderungsanalyse, werden die Bedürfnisse der Benutzer, Auftraggeber und anderen Interessensgruppen analysiert, um eine geeignete Lösung für ein Produkt zu entwickeln. Dabei wird eine Übereinkunft über die Funktionen des Systems, die Systemgrenzen und die Benutzerschnittstellen getroffen. Diese Informationen helfen auch den Entwickler, die Anforderungen besser zu verstehen. [@richterUsabilityUndUX2016]

<!-- Requirements Engineering / Anforderungsanalyse [@richterUsabilityUndUX2016]:
- Erarbeitung und Erhaltung von Übereinkunft der Stakeholder über Funktionen von System
- Vermittelt Entwicklern besseres Verständnis der Anforderungen
- Definition von Systemgrenzen und Benutzerschnittstellen (mit Fokus auf Bedürfnisse und Ziele der Benutzer)
- Anforderungen ('Requirements') sind ein Teil der primären Disziplinen des Software Engineerings
- Bedürnisse von Benutzern, Auftraggeber und weiteren Interessengruppen (Stakeholder) aufzuarbeiten, damit passende Lösung daraus erstellt werden kann
- Aufbauend auf Bedürfnissen: Erarbeitung von Rahmenbedingungne und Qualitätsanfroderungen
- Bei der Mobilen User Experience: Wer ist die anvisierte Zielgruppe und was sind deren Bedürfnisse? In welchem Kontext und in welchen Situationen wird die Anwendung verwendet? Welche Funktionen sind für die Benutzer in diesen Situationen wirklich nutzbringend?  -->

Im Folgenden werden die Anforderungen an die Suchfunktion dargestellt. Dabei wird zwischen funktionalen und nicht-funktionalen Anforderungen unterschieden. Die funktionalen Anforderungen beziehen sich auf Aspekte, die die Funktionalität des Produkts erklären. Nicht-funktionale Anforderungen beziehen sich auf die erforderlichen Qualitätsaspekte und Rahmenbedingungen, d.h. Elemente, die für das Nutzererlebnis eine wichtige Rolle spielen. In der Regel werden die Inhalte u.a. durch Interviews mit Stakeholdern oder Nutzerbefragungen ermittelt. [@richterUsabilityUndUX2016]

<!-- Funktionale und nicht-funktionale Anforderungen [@richterUsabilityUndUX2016]:
- Funktionale Anforderungen: 
    - Aspekte die mit Funktionsangebot von Produkt zusammenhängen
    - z.B. Suchen, Bestellen, Bewerten
- Nicht-funktionale Anforderungen:
    - geforderte Qualitätsaspekte und Rahmenbedingungen
    - z.B. Anforderungen zur Verfügbarkeit, Antwortzeit, Ausfallsicherheit
    - wichtige Rolle für Nutzererlebnis, Auswirkungen auf verwendete Technologien
- Methoden normalerweise: Interviews und Gespräche mit verscheidenen Stakeholdern, Analyse von Altsystemen und Dokumentationen, Interviews mit Nutzern -->

Da es sich bei der Entwicklung der Suchfunktion um eine prototypische Umsetzung handelt, wurde hierfür keine Nutzerbefragung zur Ermittlung der Anforderungen durchgeführt. Vermutliche Nutzerbedürfnisse wurden antizipiert. 

<!-- - Aber - hier nur prototypische umsetzung, groben Anforderungen kamen von Abteilung und so formuliert, dass es für den protoypschen Umfang sinn macht -->


### Systematische Erfassung der Anforderungen

<!--todo: das rein oder raus - Die identifizierte Zielgruppe der Suchfunktion sind alle Nutzer der MyBMW App - insbesondere diejenigen, die Inhalte innerhalb der App suchen und schnell finden wollen. So können diese nach einem Stichwort, z.B. 'Klima', suchen und bekommen dann die Ergebnisse der App-Inhalte angezeigt, in denen dieses Wort vorkommt. -->

<!-- - *Identifizierung der Zielgruppe und deren Bedürfnisse*
    - *Identifizieren Sie die Zielgruppe und deren Erwartungen an die Suchfunktion*
        Zielgruppe:
        - Alle Benutzer der BMW App
        - besonders die, die speziell auf der Suche nach etwas sind: Tutorial, mehr Informationen über bestimmte Funktion, Interesse an bestimmter Funktion (z.B. Navigation oder Klima)
        Erwartungen:
        - Grundsätzlich: Das Finden, wonach gesucht wird
        - Ideal: Beim Suchen Vorschläge
        - nach Suchen: Übersichtliche Darstellung aller möglichen Ergebnisse, beim Drücken auf Ergebnis möchte man direkt zur Information gelangen
        - evtl. Suchverlauf anzeigen
        - allgemein: relevante Suchergebnisse, schnelle Reaktionszeit -->

<!-- - *Analyse der Suchszenarien*
    - Suche nach einem Stichwort, um zu sehen, ob in letzter Zeit Updates dafür waren -> z.B. 'Klima' eingeben und schauen, ob es in den Release Notes vorgekommen ist, evtl. hierfür gleich Filter
    - Schnelles Suchen nach Tutorial/genauerer Anleitung: z.B. 'Navigation' eingeben und auf How-To-Video stoßen, zuvor ist die Filterung nach 'Video' oder 'Tutorial' möglich -->

Die funktionalen Anforderungen sind an die zu entwickelnde Suchfunktion sind wie folgt definiert:

- Die Suchfunktion soll der bestehenden 'Explore'-Seite hinzugefügt werden
- Nach dem Anklicken eines Suchsymbols soll der Benutzer einen einzelnen Suchbegriff in ein vorgegebenes Suchfeld eingeben können
- Vor der Eingabe einer Suchanfrage in die Suchleiste sollen dem Nutzer Vorschläge und frühere Suchanfragen angezeigt werden
- Bei der Eingabe eines Begriffs werden die zur Suche verfügbaren Quellen werden über die Schnittstelle durchsucht und anschließend jene Ergebnisse angezeigt, die den Suchbegriff beinhalten
- Dabei sollen kleine Rechtschreibfehler oder nicht exakte Übereinstimmungen zwischen Suchbegriff und durchsuchten Daten toleriert werden
- Die Resultate der Suche werden dabei in reduzierter Form untereinander angezeigt
- Zu jedem Ergebnis werden ein Titel und Ausschnitte eines längeren Textes dargestellt. Durch Anklicken wird die dazugehörige Seite geöffnet, während beim Verlassen der Seite wieder die Ergebnisse der Suchfunktion angezeigt werden

<!-- Text ohne Stichpunkte:
Die funktionalen Anforderungen sind an die zu entwickelnde Suchfunktion sind wie folgt definiert. Die Suchfunktion soll der bestehenden 'Explore'-Seite hinzugefügt werden. Nach dem Anklicken eines Suchsymbols soll der Benutzer einen einzelnen Suchbegriff in ein vorgegebenes Suchfeld eingeben können. Dabei sollen kleine Rechtschreibfehler oder nicht exakte Übereinstimmungen zwischen Suchbegriff und durchsuchten Daten toleriert werden. Vor der Eingabe einer Suchanfrage in die Suchleiste sollen dem Nutzer Vorschläge und frühere Suchanfragen angezeigt werden. Bei der Eingabe eines Begriffs werden die zur Suche verfügbaren Quellen werden über die Schnittstelle durchsucht und anschließend jene Ergebnisse angezeigt, die den Suchbegriff beinhalten. Die Resultate der Suche werden dabei in reduzierter Form untereinander angezeigt. Zu jedem Ergebnis werden ein Titel und Ausschnitte eines längeren Textes dargestellt. Durch Anklicken wird die dazugehörige Seite geöffnet, während beim Verlassen der Seite wieder die Ergebnisse der Suchfunktion angezeigt werden.  -->

Die nicht-funktionalen Anforderungen umfassen:

- Die Suchfunktion soll eine gute Performance aufweisen, d.h. die Suchergebnisse sollen schnell angezeigt werden
- Die Suchfunktion soll benutzerfreundlich sein. Bei der prototypischen Umsetzung der Suchfunktion im Rahmen dieser Bachelorarbeit steht das UX-Design jedoch nicht im Vordergrund

<!-- Text ohne Stichpunkte:
Als nicht-funktionale Anforderung soll die Suchfunktion eine gute Performance aufweisen, d.h. die Suchergebnisse sollen schnell angezeigt werden. Außerdem soll die Suchfunktion benutzerfreundlich sein. Bei der prototypischen Umsetzung der Suchfunktion im Rahmen dieser Bachelorarbeit steht das UX-Design jedoch nicht im Vordergrund. -->

<!-- - *Definition von Qualitätsanforderungen (Usability, Performance, Sicherheit etc.)*

    - *Definieren Sie funktionale und nicht-funktionale Anforderungen an die Suchfunktion (Funktionale Anforderungen: Hierbei handelt es sich um Anforderungen, die in spezifischem Zusammenhang mit dem Projekt stehen. Nicht-funktionale Anforderungen: Alle anderen Anforderungen gibt es auch bei mehreren Projekten, wie etwa das Zeitmanagement oder den Ressourcenverbrauch.)* -->

<!--
Funktionale Anforderungen
1. Freie Textsuche:
    - Die Nutzer können frei Suchbegriffe in ein Suchfeld eingeben, um nach Inhalten zu suchen.
    - Die Suche soll alle durchsuchbaren Bereiche (Explore-Page mit Tutorials und Artikeln, Release Notes, MyHighlights) abdecken.
    - Die Suche soll mit AND- oder OR-Verknüpfung mehrere Suchbegriffe unterstützen.
2. Suchergebnisse:
    - Die Suchergebnisse sollen untereinander angezeigt werden.
    - Dabei soll die Quelle bzw. Kategorie erkennbar sein
    - Durch Drücken auf das Ergebnis soll zum Ort der Daten innerhalb der App navigiert werden
3. Filterung der Suche:
    - Die Suchergebnisse können nach Kategorien wie Tutorials, Artikel, Release Notes usw. gefiltert werden. (evtl.)
4. Suchverlauf:
    - Vor Eingabe des Suchbegriffes soll der Verlauf der letzen Suchanfragen angezeigt werden
5. Suchvorschläge (noch nicht sicher):
    - Während der Eingabe werden Suchvorschläge angezeigt, um die Suche zu erleichtern.
    - Falsch geschriebene Suchbegriffe werden erkannt und Verbesserungsvorschläge angezeigt.

Nicht-funktionale Anforderungen
    1. Usability:
        - Die Suchfunktion soll intuitiv und einfach zu bedienen sein.
        - Die Darstellung der Suchergebnisse muss übersichtlich und verständlich sein.
        - Das Design der Suchfunktion soll konsistent mit dem restlichen App-Design sein.
    2. Performance:
        Die Suchfunktion muss eine schnelle Reaktionszeit auf Nutzereingaben aufweisen.
        Die Anzeige von Suchvorschlägen und Suchergebnissen soll zeitnah erfolgen.
        Die Suchfunktion muss auch bei hoher Nutzerlast zuverlässig und performant arbeiten.

- *Priorisieren Sie die Anforderungen nach Wichtigkeit und Umsetzungsaufwand *  
    1. Freie Textsuche
    2. Suchergebnisse
    3. Filterung
    4. Verlauf
    5. Vorschläge -->

Neben der Analyse der Anforderungen an die Suchfunktion, werden auch die technischen Rahmenbedingungen analysiert. So sollen die technischen Möglichkeiten und Grenzen untersucht, geeignete Bibliotheken gefunden und Schnittstellen geprüft werden. 
Die Suchfunktion soll in die bestehende App-Umgebung der MyBMW-App integriert werden. Da die MyBMW-App mit Flutter entwickelt wurde, basiert die grundlegende technische Infrastruktur der Suchfunktion auf der Programmiersprache Dart.

Flutter stellt u.a. die Klasse 'SearchDelegate' zur Verfügung, die eine Suchseite erzeugt, die u.a. Vorschläge und Ergebnisse anzeigt und im Code Zugriff auf das aktuelle Suchwort, also 'query' ermöglicht [@SearchDelegateClassMaterial]. Diese Klasse vereint die genannten Anforderungen. Die Klasse 'SearchBar' stellt zum Vergleich nur das Eingabefeld für die Suchbegriffe zur Verfügung [@flutterSearchBarClassMaterial].

Die Datenquellen für die Suchfunktion sind die bereits erwähnten 'String Files'-, Kontext- und Lokale-Daten. 

Um letztere Daten aus der JSON-Datei lesen zu können, müssen diese zunächst in ein für Dart lesbares Format gebracht werden. Dies kann mit dem Dart-Package 'json_serializable' realisiert werden. Damit können Daten zwischen dem JSON-Format und der gewünschten und durch den Code definierten Struktur konvertiert werden. [@Json_serializableDartPackage]

In allen Quellen werden für die Suchfunktion unterschiedliche Strings nach Übereinstimmungen durchsucht. Um kleine Abweichungen zwischen Such- und Vergleichswort zu tolerieren, kann das Dart Package 'Fuzzy' verwendet werden. Mit diesem wird ein für einen String-Vergleich ein sogenannter Fuzzy-Score erzeugt, der angibt, wie groß die Übereinstimmung ist. [@FuzzyDartPackage]

<!-- - alles in sprache dart, weil App in flutter
- hier: search delegate
- Datenquellen: verschiedene lokale Quellen - anbindung aus quelle von app, lokaler jsondatei -> jsonSerialzable, durchsuchung der übersetzungs-files
- verschiedene suchfunktionen - was sinnvoll hier
- integration in bestehende systeme -> suchfunktion wird zu seite hinzugefügt -->
<!-- - *Analyse der technischen Rahmenbedingungen*
    - *Untersuchen Sie die technischen Möglichkeiten und Grenzen der Plattform/App*
        - Suchfunktion selber mit Flutter 'SearchBar' [@flutterSearchBarClassMaterial] -> Ergebnisse der Query in Liste packen
        - Kann ich bei einem Ergebnis tatsächlich auf die Quelle / den Ort der Daten kommen? Muss ich bzw. wie speichere ich den Ort dieser Information
        - Rechschreibung: Fuzzy
        - Suchalgorithmen: Abgleich - nur reine Textsuche
    - *Prüfen Sie die Verfügbarkeit und Eignung von Bibliotheken/Frameworks für die Suchfunktion*
        - SearchBar von Flutter [@flutterSearchBarClassMaterial]
        - SearchDeligate
    - *Identifizieren Sie mögliche Schnittstellen zu anderen Systemkomponenten*
        - für eingabe mit Json: JsonSerializable -->

### Konzeptentwurf 

Auf Basis der systematischen Erfassung der Anforderungen an die Suchfunktion wird nun das Konzept für die Suchfunktion konkretisiert. Die Konzeption und der Aufbau der API, an die die Suchanfragen gestellt wird und die die verschiedenen Quellen zusammenführt, werden im nächsten Kapitel behandelt. Daher wird an dieser Stelle nicht näher darauf eingegangen. Grob betrachtet schickt die Suchfunktion ein Suchbegriff an die API und bekommt von dieser dann die Ergebnisse für die Anfrage zurück. (Siehe Abbildung \ref{fig:suchfunktion_api}) 

![Quelle: eigenes Diagramm, 2025](source/figures/Suchfunktion_API.drawio.png){#fig:suchfunktion_api width=50%}

Der Ablauf der Suchfunktion aus Benutzersicht soll wie folgt ablaufen. Durch Anklicken des Lupensymbols auf der 'Explore'-Seite, öffnet sich die Seite der Suchfunktion. Über die Leiste Leiste am oberen Rand dieser Seite können folgende Funktionen ausgeführt werden: Es besteht die Möglichkeit zurück zur vorherigen Seite zu navigieren, einen Suchbegriff einzugeben oder den bisher eingegebenen zu löschen. Unterhalb der Leiste befinden sich Suchvorschläge, die von der Funktionsseite gegeben werden und die zuletzt durchgeführten Suchanfragen. Dabei muss entschieden werden, ob diese Funktionen durch Symbole dargestellt oder mit Text angeschrieben werden. Auch muss entschieden werden, ob die Suchvorschläge dynamisch oder statisch sind.

Eine Suchanfrage wird durchgeführt, indem ein Suchbegriff in das Suchfeld eingegeben und dann mit der Eingabetaste bestätigt wird. Während des Tippens wird die Seite mit Suchverlauf und den Vorschlägen weiter angezeigt. Der Suchbegriff wird an die API geschickt, die diese Anfrage bearbeitet. Anschließend werden die durch die API gefundenen Ergebnisse nach Relevanz sortiert aufgelistet. Diese können je nach Quelle und damit Inhalt unterschiedlich aufgebaut sein. 

Bei den Ergebnissen aus den 'String Files' müssen einige Punkte bedacht werden. So muss geklärt werden, ob nur die Datei für die aktuelle Sprache, in der die App gerade ist, oder alle vorhandenen Sprachen, und damit alle Files durchsucht werden. Denn Nutzer könnten beispielsweise mit einer deutschen App-Einstellung nach einem englischen Begriff suchen und dafür ein Ergebnis erwarten. Andererseits könnte besonders durch die Toleranz von Rechtschreibfehlern Begriffe aus anderen Sprachen, die ähnlich sind, als Treffer angesehen werden können. Zudem muss geklärt werden, wie die Ergebnisse aus den 'String Files' dargestellt werden. Da alle Ergebnisse eines Dienstes auf die gleiche Seite verweisen, ist zu festzusetzen, ob Ergebnisse pro Dienst gruppiert oder einzeln angezeigt werden.

Wird ein Ergebnis angeklickt, öffnet sich die entsprechende Seite der App. Navigiert man zurück, gelangt man wieder auf die Ergebnisseite. (Siehe Abbildung \ref{fig:wireframe_1}) Dieser Aufbau ähnelt der Struktur, die von der Klasse 'SearchDelegate' von Flutter vorgeschlagen wird, in der Platz für Suchvorschläge und -ergebnisse vorgesehen ist [@SearchDelegateClassMaterial]. 

![Quelle: eigene Zeichnung, 2025](source/figures/Wireframes_ba_1.png){#fig:wireframe_1 width=100%}

Der Suchbegriff wird durch Ausführen der Suche an die API übergeben, die nach der Verarbeitung die passenden Ergebnisse aus den verschiedenen Quellen zurückgibt. Diese werden dann untereinander aufgelistet, wobei die verschiedenen Ergebnisse deutlich voneinander unterschieden werden. Die eigentliche Suchfunktion liegt also in der API, die im folgenden Kapitel konzipiert wird.

<!-- - *Architekturdesign*
    - *Entwerfen Sie die Systemarchitektur der Suchfunktion*
        - mit draw.io !
    - *Legen Sie die Schnittstellen und Datenflüsse zwischen den Komponenten fest*
    - *Wählen Sie geeignete Technologien und Frameworks für die Umsetzung aus*
    - *Integration in das Gesamtkonzept der Anwendung*
- *Interaktionsdesign*
    - *Konzipieren Sie das Nutzererlebnis und die Interaktionsabläufe der Suchfunktion*
    - *Erstellen Sie Wireframes oder Mockups zur Visualisierung des Designs*
    - *Berücksichtigen Sie Aspekte wie Usability, Barrierefreiheit und Responsivität- Konzeption der Suchlogik und Ergebnispräsentation* -->

## Konzeption der API

Nachdem im vorherigen Kapitel das Bedienkonzept erarbeitet worden ist, soll nun die bisher nicht näher betrachtete API konzipiert werden. Die hier zu entwickelnde API wird als Schnittstelle in das existierende App-Umfeld hinzugefügt.

### Schnittstellen-Design

Der Zugriff auf die API erfolgt über einen lokalen Aufruf innerhalb der Suchfunktion. Bei Bestätigung der Eingabe in das Suchfeld wird der Suchbegriff an die Schnittstelle übergeben. Als Rückgabewert werden dann die Ergebnisse der Suche erwartet.

Um die Daten auslesen zu können, muss die API auf verschiedene Datenquellen zugreifen. Für die prototypische Umsetzung sind die, wie bereits schon mehrfach angeführt, die 'String-Files'-, Kontext- und Lokale-Daten. Die detaillierte Betrachtung des Zugriffs auf diese Daten erfolgt im Kapitel zur Implementierung.

### Architektur-Entwurf

- *Aufteilung der Anwendung in logische Komponenten (z.B. Datenzugriff, Geschäftslogik, Präsentation)*
- *Festlegung von Kommunikationswegen und Abhängigkeiten zwischen den Komponenten*
- *Auswahl geeigneter Technologien, Frameworks und Bibliotheken*
- *Entscheidungen zur Skalierbarkeit, Performanz und Ausfallsicherheit*
- *Konzeption von Querschnittsthemen wie Authentifizierung, Logging, Monitoring*

Infos in [@nunkesserAppEntwicklungFuerMobile2023] ab Seite 65

