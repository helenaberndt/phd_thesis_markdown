# Grundlagen

## Die MyBMW App

Quelle [@tasiorDevelopersCars]:

- Zunächst Native Entwicklung, dann Android und dann alles neu in Flutter ab 2018/2019
-  BMW, BMW M, Mini und Toyota -> gleiche App aber unterschiedliche Skins, mit verschiedenen Regionen (Nord Amerika, Korea etc.) ca 30 Apps im Apps Store
- Eines der größten Flutter-Entwicklungsteams überhaupt
- ca. 250 Developers arbeiten an der App
- 23 Sprachen werden unterstützt

Quelle[@bmwgroupHighlightsMyBMW]:

- Funktionen wie: Aus Ferne Fahrzeugstatus, ladestatus, Reichweite, Türen/Fenster überprüfen; Fahrten planen; Klimatisierung; Software-Upgrades buchen
- universelle Schnittstelle zum Fahrzeug und weiteren Produkten und Services von BMW
- App ist optimiert für Fahrzeuge ab dem Baujahr 2014
- Verfügbarkeit der Funktionen ist abhängig von Fahrzeugausstattung, ConnectedDrive Vertrag und Ländern

Quelle[@julichUpdateFuerFreude2021]:

- My BMW App verbindet Kunden über das Smartphone mit Ihrem Fahrzeug und macht es zu einer intelligenten Schnittstelle
- Remote Software Upgrade
    - Mit dem BMW Operating System 7 und Remote Software Upgrade seit 2018
    - Fahrzeug auf den neusten Softwarestand bekommen
    - über die My BMW App oder over-the-air direkt ins Fahrzeug
    - Ablauf: Installationsdateien im Hintergrund vorbereitet, Installation selber dauert unter 20 Minuten
    - Mittlerweile ist RSU für über 30 BMW Modelle verfügbar
    - Verfügbarkeit ist abhängig von Fahrzeugmodell, Ausstattung und jeweiligem Land

Quelle [@bmwHowErsteSchritteMit2024]:

- Mobiler Zugriff auf Fahrzeug, BMW Services und Stores
- Einloggen mit BMW ID
- Fahrzeug-Tab (Vehicle Tab): Überblick über Fahrzeugstatus und Remote-Funktionen, "Meine Fahrten" mit Informationen über Fahrten und Fahrverhalten, Charging Hub für Informationen über Elektrofahrzeuge
- Karten-Tab: Karte mit Sonderzielen (Park-, Tank, Ladestationen), Ziele können an Fahrzeug geschickt werden
- Explore-Tab: Neuigkeiten und praktische Tipps zu Benutzung des BMW-Fahrzeuges
- Message Center: personalisierte Informationen (z.B. RSU verfügbar)
- BMW Services und Store Tab: BMW Connected Drive Upgrades, Kontakt zu Service Partnern, Finanzdienstleistungen, BMW Stores, Buchung von Probefahrt
- Profil-Tab: persönliche Einstellungen, Hilfecenter, Datenschutzeinstellungen

Quelle [@julichNeueSoftwareFuer2023]

- Remote Software Upgrade ist für über 30 Modelle und damit fast alle BMW Modelle mit BMW Operating System 7 und 8 verfügbar
- Kunden können im Einstellungsmenü des Fahrzeugs unter Remote Software Upgrade den Softwarestand abrufen und verfügbare Updates suchen

Quelle [@tholundUmfangreicheUpdatesMy2024]

- Über 13 Millionen Nutzer weltweit (My BMW und Mini)
- fünf Updates pro Jahr


## Suchfunktionen in Mobilen Anwendungen

Quelle [@komakiHowDoesMobile2012]:

- In Studie: Mehr Anfragen per Session an einem Desktop PC als an einem Mobilen Telefon, was impliziert, dass Mobile Nutzer weniger dazu bereit sind Themen in Tiefe zu erkunden wegen größeren Hürden beim Suchen, wie Query-Eingabe
- Nützlich für Suchanfragen: Voice search, push-based information recommendation services

Quelle [@churchLargeScaleStudy2008]:

- This study analyzed one million page requests from Google and focused on features such as query length, target content, and relationship between queries and device characteristics. They found that users with less sophisticated input capabilities submitted shorter queries and adult content was the most prevalent search topic. 

*Quelle [@kamvarDecipheringTrendsMobile2007] (von 2007, also bisschen Alt):

- durchschnittliche Mobile Query: 2.56 Wörter und 16.8 Charakter (auch andere Studien zeigen ähnliche Ergebnisse)*

Quelle [@maMashDroidApproach2015]:

- Im Kontext, Apps für Durchsuchung des App-Stores oder einfach aller Funktionen durchsuchbar zu machen (man sucht nach Inhalt der App im AppStore und bekommt dann App vorgeschlagen, z.b. "Harry Potter" und man bekommt Apps mit Ebooks oder Filmen angezeigt und landet dann direkt im gesuchten Inhalt):
    - Kein tieferes Wissen darüber, welche Daten oder Funktionalitäten eine App bereitstellt. Wenn man jede App als eine einzelne Webseite sehen würde, könnte man mit einem WebCrawler oder einer Search Engine durchsuchen, um den dynamischen Content zu bekommen. Damit bekommt man eine tieferes Verständnis für für die Daten und Content innerhalb der App und könnte Korrelationen zwischen den Apps finden.
    - Dies ist jedoch ziemlich schwierig, da die Genehmigung von App-Entwicklern erforderlich ist, um ein Codefragment für die Indexerstellung zu instrumentieren, genauso wie Webentwickler Google Analytics-Code in ihre HTML-Codes aufnehmen, um die Seiten zu indizieren. 
    - Neben des Beschreibung im App Store sind Apps Black-Boxes (nur .apk / .ipa file)
- Funktion von "Wandoujia App Store (WDJ)": Damit Apps Zugriff auf In-App Search (IAS) haben, muss jeder Content eine assigned APP-URL haben und das URL Pattern muss registered in the intent by intent-filter sein. Zusätzlich dazu dann: Semantische Analyse, Filter, Ranking Algorithms, um die most likely App to be used zu finden
- Modellierung von Apps für Suchfunktionen:
    - Das RESTful-Stil-App-Modell abstrahiert Apps als Sammlungen von Ressourcen, auf die über standardisierte Operationen (GET, POST, etc.) zugegriffen werden kann
    - Das ressourcenorientierte App-Beschreibungsmodell ermöglicht eine strukturierte Erfassung der Inhalte und Funktionalitäten der Apps
    - Diese Modellierung erleichtert das maschinelle Verständnis und die gezielte Suche nach relevanten App-Funktionen
- Ansatz ist technisch umsetzbar, Algorithmus um dann die Durchsuchung mehrere Apps zu machen ist nicht relevant.

## API-Entwicklung
Quelle [@selvarajMasteringRESTAPIs2024]:

- APIs:
    - spielen eine pivotal Rolle darin, eine nahtlose Kommunikation zwischen Software Komponenten und Services herzustellen
    - APIs sind unverzichtbar für die Verbindung verschiedener Systeme, ermöglichen es Entwicklern, die Leistungsfähigkeit von Drittanbieterdiensten zu nutzen und die Interoperabilität zu fördern
    - Wichtigkeit: pivotal Rolle als das verbindene Tissue zwischen verschiedenen Software Systemen
    - ermöglichen nahtlose Integration und Kommunikation, damit können Entwickler existierende Services, Daten und Funktionalitäten nutzen und damit den Entwicklungsprozess beschleunigen und die Effizienz verbessern

    - RESTful Apis: 
        - Typ von Web-API, das einen Satz von Architektur-Prinzipen und Conventions folgt, für das die Design und die Intraktion mit Ressourcen über das Internet. Weitverbreitet für die Erstellung von Web Services und building distributed and scalable Web Anwendungen. 
        - Bild davon: 
        ![Source: Source: comScore MMX Multi-Platform, January 2017 (falls ich des brauche) \label{martinMobilesHierarchiyNeeds2017_composition}](source/figures/selvarajMasteringRESTAPIs2024_RESTAPI_image.png){ width=100% }      
    
APIs in Mobile Apps:

- Quelle [@maMashDroidApproach2015]:
    - Fast alle "networked Mobile Apps" greifen auf RESTful Web services/APIs zu und verwenden HTTP(s) als Transfer-Protokol
    - Dienstanbieter stellen ihre Funktionen über über das Internet zugängliche APIs als Dienste zur Verfügung, und die mobilen Apps könnten diese APIs aufrufen, die normalerweise in RESTful-Form bereitgestellt werden. Derzeit treten mobile Apps an die Stelle von Desktop-Anwendungen wie Browsern als neuer dominanter Dienstleistungsverbraucher.

- Quelle [@selvarajMasteringRESTAPIs2024]:
    - Mobile Apps als Use Case für APIs: RESTful APIs spielen eine entscheidende Rolle umd Mobile Apps mit Backend-Servern zu verbinden
    - Mobile Apps können Daten abrufen, User authentifizieren, verschiedene Aktionen durchführen indem sie mit RESTful APIs interagieren

Quelle [preibischAPIDevelopmentPractical2018]:

- Client-seitige API: 
    - versteckt die Komplexität die hinter den Requests an den Server steckt
    - Eine einzigee client-side API interagiert häufig mit einer oder mehreren Server-seitigen APIs
- Server-seitige API:
    - Eine serverseitige API bietet einen klar definierten Einstiegspunkt in ein geschlossenes System und aus diesem heraus
- Vorteile von Benutzung von APIs
    - Integration: Unternehmen wollen in der Lage sein, sich in andere Systeme zu integrieren und, dass andere Systeme in ihre Systeme integriert werden. 
    - Modernisierung: trotz Modernisierung bleiben APIs relevant
    - Automatisierung: APIs können verwendet werden, um den Build-Prozess von Software Produkten zu automatisieren

Quelle [@linares-vasquezAPIChangeFault2013]:

- API-Instabilität und Fehleranfälligkeit können sich auf den Erfolg der Software auswirken: APIs die von erfolgreichen (anhand von Google Play Bewertung gemessen) Apps verwendet werden sind weniger fehleranfällig, als jene, die von erfolgloseren verwendet werden
- denn: fehleranfällige APIs können zu Fehlfunktionen und Craches in Mobilen Apps führen
- Veränderungen bei API: Updates häufiger notwendig

Quelle [@payneMakingRESTfulAPI2024]:

- Hintergrund: Server-Side Programm, um Daten in einer kontrollierten Art zu lesen und zu bearbeiten mithilfe von Protokollen wie https. Zum Lesen: http request mit credentials (username/password oder API key)
- APIs geben die Daten fast immer in einem JSON Format zurück
![Source: Source: comScore MMX Multi-Platform, January 2017 (falls ich des brauche) \label{source/figures/payneMakingRESTfulAPI2024_table9_1}](source/figures/payneMakingRESTfulAPI2024_table9_1.png){ width=100% }

