# Implementierung der API und Suchfunktion

## Implementierung der API

### Vertiefte Hintergründe der API
Quelle [@selvarajMasteringRESTAPIs2024]:

- Client-Server-Architektur: trennt die Verantwortlichkeiten zwischen Client und Server und ermöglicht damit skalierbare, maintainable und effiziente Systeme
    - Client: repräsentiert das user Interface oder die Applikation die mit dem Server interagiert, um Ressourcen anzufragen oder Operationen durchzuführen. Clients können sein: Web Browser, Mobile Apps, Desktop Applikationen, IoT-Geräte, entspricht der presentation layer
    - Server: Hosted die Ressourcen, verarbeitet / führt die Anforderungen (Requests) vom Client durch, speichert und managed die Daten, setzt Security Maßnahmen durch, stellt sicher, dass Requests ausgeführt werden 
    - wichtig: klare Separation zwischen den Aufgaben
    - Statelessness. Kein Client State muss vom Server gespeichert werden, wodurch die Interaktion vereinfacht wird
    - Caching: mächtige Performance-Optimierungs Technik, reduziert redundant Requests und verbessert die System Performance insgesamt
    - Scalability: durch layered architecture, Separation zwischen Client und Server - wenn höherer Demand ist, können mehr Server hinzugeschaltet werden
    - Flexibilität: Server und Client können in unterschiedlichen Sprachen und Frameworks implementiert werden
    - Interoperabilität: ermöglicht Interoperabilität zwischen verschiedenen Clients und Servern, solange alle common Kommunikationsprotokolle verwenden (z.b. HTTPs bei Restful APIs)
    - Sicherheit: besseres Security-Management, der Server kann Sicherheitsmaßnahmen (authentication, authorization, data validation etc.) durchführen
- Stateless Interaction bei RESTful APIs:
    - jeder Request von einem Client muss alle notwendigen Informationen beinhalten, so dass er vom Server verstanden und verarbeitet werden kann. Jeder Request ist also self-contained und independent (abgeschlossen und unabhängig)
    - Server muss also keine Informationen über die vergangenen Anfragen von Clients speichern
    - auch hier wieder: Scalability (Servers speichern nichts zum Client-state und können eine große Anzahl von Requests speichern), Flexibility (Requests können an jeden Server gestellt werden), Fault Tolerance (da jeder Request unabhängig ist, kann man den gleichen Request bei mehreren Servern durchführen, falls einer fehlerhaft ist), Caching (Clients oder proxy Server können Antworten cachen udn damit die Performance verbessern, indem wiederholte Antworten verhindert werden)
    - Vorteile: Simplicity (vereinfacht Design und Development), Scalability, Resilience (Fehler in einem Teil des Systems haben keinen Einfluss auf andere), Compatibility (verbessert Interoperabilität, indem ein breites Spektrum an Clients das Design der API's nutzen, z.B. Browsers, Mobile Apps)
    - Caching: wichtig für Performance, reduziert Network Load, verbessert User Experience; Server kann indicaten, ob der Client Antworten, die er bekommt cachen kann; damit können Antworten/Responses gespeichert werden und sich wiederholende Anfragen für die gleichen Ressourcen können reduziert werden. Gut für Ressourcen, die sich nicht häufig ändern (Statische Inhalte, Bilder, Daten aus einer Datenbank) (Noch mehr Infos, S.10)
    - Uniform Interface Principle:
        - Resource Identification: Resourcen sind der Core von RESTfulAPIs, jede Resource hat eine einzigartige URL, diese ist die Adresse um auf die Resource zuzugreifen und oder auf ihr Operationen durchzuführen
        - Standard HTTP Methoden: GET, POST, PUT, DELETE, welche zu den CRUD Operationen passen. Diese Uniformität vereinfacht die Struktur der API und die Benutzung; dabei werden auch Standard HTTP status Codes verwendet (200 für Erfolg, 404 not found, 500 server error) dadurch ist eine klare und konsistente Art gegeben, um den Client über das Ergebnis des Requests zu informieren
        - Die Nachrichten sollte selbst-erklärend (self-descriptive) sein, so dass der Server kein zusätzliches Wissen benötigt
        - durch UIP: Simplicity, Predictability, Interoperability, Decoupling (Client und Server können unabhängig arbeiten), discoverability (Durch URLs können API Endpunkte leicht gefunden werden), -> intuitiv, effizient, accessible, driving broader adoption



## Implementierung des Suchfunktions-Prototyps



## UI

Mehr in Quelle [@nunkesserAppEntwicklungFuerMobile2023] ab Seite 122 ... 