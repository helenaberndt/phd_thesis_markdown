# Konzeption

## Anforderungsanalyse der Suchfunktion

### Systematische Erfassung der Anforderungen

- *Identifizierung der Zielgruppe und deren Bedürfnisse*
    - *Identifizieren Sie die Zielgruppe und deren Erwartungen an die Suchfunktion*
        Zielgruppe:
        - Alle Benutzer der BMW App
        - besonders die, die speziell auf der Suche nach etwas sind: Tutorial, mehr Informationen über bestimmte Funktion, Interesse an bestimmter Funktion (z.B. Navigation oder Klima)
        Erwartungen:
        - Grundsätzlich: Das Finden, wonach gesucht wird
        - Ideal: Beim Suchen Vorschläge
        - nach Suchen: Übersichtliche Darstellung aller möglichen Ergebnisse, beim Drücken auf Ergebnis möchte man direkt zur Information gelangen
        - evtl. Suchverlauf anzeigen
        - allgemein: relevante Suchergebnisse, schnelle Reaktionszeit

- *Analyse der Suchszenarien*
    - Suche nach einem Stichwort, um zu sehen, ob in letzter Zeit Updates dafür waren -> z.B. "Klima" eingeben und schauen, ob es in den Release Notes vorgekommen ist, evtl. hierfür gleich Filter
    - Schnelles Suchen nach Tutorial/genauerer Anleitung: z.B. "Navigation" eingeben und auf How-To-Video stoßen, zuvor ist die Filterung nach "Video" oder "Tutorial" möglich
    
- *Definition von Qualitätsanforderungen (Usability, Performance, Sicherheit etc.)*

    - *Definieren Sie funktionale und nicht-funktionale Anforderungen an die Suchfunktion (Funktionale Anforderungen: Hierbei handelt es sich um Anforderungen, die in spezifischem Zusammenhang mit dem Projekt stehen. Nicht-funktionale Anforderungen: Alle anderen Anforderungen gibt es auch bei mehreren Projekten, wie etwa das Zeitmanagement oder den Ressourcenverbrauch.)*
        - Funktionale Anforderungen
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

        - Nicht-funktionale Anforderungen
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
        5. Vorschläge

- *Analyse der technischen Rahmenbedingungen*
    - *Untersuchen Sie die technischen Möglichkeiten und Grenzen der Plattform/App*
        - Suchfunktion selber mit Flutter "SearchBar" [@flutterSearchBarClassMaterial] -> Ergebnisse der Query in Liste packen
        - Kann ich bei einem Ergebnis tatsächlich auf die Quelle / den Ort der Daten kommen? Muss ich bzw. wie speichere ich den Ort dieser Information
    - *Prüfen Sie die Verfügbarkeit und Eignung von Bibliotheken/Frameworks für die Suchfunktion*
        - SearchBar von Flutter [@flutterSearchBarClassMaterial]
    - *Identifizieren Sie mögliche Schnittstellen zu anderen Systemkomponenten*

### Konzeptentwurf 

- *Architekturdesign*
    - *Entwerfen Sie die Systemarchitektur der Suchfunktion*
        - mit draw.io !
    - *Legen Sie die Schnittstellen und Datenflüsse zwischen den Komponenten fest*
    - *Wählen Sie geeignete Technologien und Frameworks für die Umsetzung aus*
    - *Integration in das Gesamtkonzept der Anwendung*
- *Interaktionsdesign*
    - *Konzipieren Sie das Nutzererlebnis und die Interaktionsabläufe der Suchfunktion*
    - *Erstellen Sie Wireframes oder Mockups zur Visualisierung des Designs*
    - *Berücksichtigen Sie Aspekte wie Usability, Barrierefreiheit und Responsivität- Konzeption der Suchlogik und Ergebnispräsentation*

## Konzeption der API

### Schnittstellen-Design

- *Festlegung der Endpunkte (Endpoints) der API*
- *Definition der Eingabeparameter und Rückgabewerte für jeden Endpunkt*
- *Festlegung des Datenformats (z.B. JSON, XML)*
- *Spezifikation von HTTP-Methoden (GET, POST, PUT, DELETE)*
- *Dokumentation der API für Entwickler*

### Architektur-Entwurf

- *Aufteilung der Anwendung in logische Komponenten (z.B. Datenzugriff, Geschäftslogik, Präsentation)*
- *Festlegung von Kommunikationswegen und Abhängigkeiten zwischen den Komponenten*
- *Auswahl geeigneter Technologien, Frameworks und Bibliotheken*
- *Entscheidungen zur Skalierbarkeit, Performanz und Ausfallsicherheit*
- *Konzeption von Querschnittsthemen wie Authentifizierung, Logging, Monitoring*

Infos in [@nunkesserAppEntwicklungFuerMobile2023] ab Seite 65

