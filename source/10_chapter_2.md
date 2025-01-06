# Grundlagen

## Die MyBMW App

Im Jahr 2020 wurde von der BMW Group die MyBMW- bzw. Mini-App publiziert, die Kunden einen digitalen Zugang zu ihrem Auto ermöglicht. Ihre Entwicklung basierte auf dem Feedback und den Erkenntnissen aus dem Nutzerverhalten der vorherigen Generationen der BMW i Remote App und der BMW Connected App. [koenigYourWorldMy2020]
Zum aktuellen Zeitpunkt benutzen über 13 Millionen Nutzer die App. Sie wird etwa fünf Mal im Jahr durch Updates aktualisiert. [@tholundUmfangreicheUpdatesMy2024]

Für die Entwicklung der App wurde Flutter verwendet, ein Open-Source-Framework welches nativ kompilierte und plattformübergreifende Anwendungen aus einer einzigen Code-Basis erstellt. [flutterFlutterBuildApps] Auf dieser Grundlage ist es möglich, die App sowohl für Android und IOS, sowie für die verschiedenen Skins und Regionen zu bauen. Die Skins repräsentieren die Marken BMW, BMW M, Mini und Toyota. Darüber hinaus existieren spezifische Versionen für ausgewählte Regionen, wie Nordamerika oder Korea. Daraus resultieren ca. 30 Apps, die den Kunden in Apps Stores angeboten werden. Das Team von ca. 250 Entwicklern, von denen einige bereits seit 2018 an der App arbeiten, stellt eines der größten Flutter-Entwicklungsteams dar. [@tasiorDevelopersCars]
Die App bieten den Kunden eine universelle Schnittstelle zum Fahrzeug. So können Remote-Funktionen ausgeführt werden, mit denen aus der Ferne über das Mobiltelefon der Fahrzeug- oder Ladestatus, die Reichweite oder Türen und Fenster des Autos überprüft werden können. Dabei sind die Funktionen optimiert für Fahrzeuge ab dem Baujahr 2014 und abhängig von Fahrzeugausstattung und länderspezifischen Vorgaben. [@bmwgroupHighlightsMyBMW]
Mit der App können Kunden nach Anmeldung mit ihrer BMW-ID einen mobilen Zugriff auf ihr Fahrzeug, BMW Services und Store haben. Dabei ist die App in mehrere Unterseiten (Tabs) aufgeteilt. Im Fahrzeug-Tab kann der Kunde einen Überblick über den aktuellen Zustand seines Autos bekommen, also Fahrzeugstatus und Remote-Funktionen, so wie unter anderem Zugriff auf die Funktionen 'Meine Fahrten'. In dem Karten-Tab können Ziele zur Navigation gesucht und ausgewählt werden. Der BMW-Services- und Store-Tab gibt den Kunden direkten Zugriff auf Updates und Finanzdienstleistungen und bietet Kontakt zu Service Partnern. Im Profil-Tab können persönliche Einstellungen vorgenommen werden. [@bmwHowErsteSchritteMit2024]
Ein besonderes Feature ist das Remote Software Upgrade. Damit können Updates für die Fahrzeug-Software direkt 'over-the-air' auf das Auto oder erst auf die MyBMW-App und dann auf das Auto geladen werden. [@julichUpdateFuerFreude2021] 


<!-- Quelle [koenigYourWorldMy2020]:
- Davor: BMW i Remote App 2013, BMW Connected App
- myBMW App seit 2020 neue App Generation, auf Feedback und Nutzerverhalten der vorherigen App Generationen
- intuitiver, vereinfachte Benutzerführung -->
<!-- Quelle [@tasiorDevelopersCars]:
- Zunächst Native Entwicklung, dann Android und dann alles neu in Flutter ab 2018/2019
-  BMW, BMW M, Mini und Toyota -> gleiche App aber unterschiedliche Skins, mit verschiedenen Regionen (Nord Amerika, Korea etc.) ca 30 Apps im Apps Store
- Eines der größten Flutter-Entwicklungsteams überhaupt
- ca. 250 Developers arbeiten an der App
- 23 Sprachen werden unterstützt -->
<!-- Quelle[@bmwgroupHighlightsMyBMW]:
- Funktionen wie: Aus Ferne Fahrzeugstatus, ladestatus, Reichweite, Türen/Fenster überprüfen; Fahrten planen; Klimatisierung; Software-Upgrades buchen
- universelle Schnittstelle zum Fahrzeug und weiteren Produkten und Services von BMW
- App ist optimiert für Fahrzeuge ab dem Baujahr 2014
- Verfügbarkeit der Funktionen ist abhängig von Fahrzeugausstattung, ConnectedDrive Vertrag und Ländern -->
<!-- Quelle[@julichUpdateFuerFreude2021]:
- My BMW App verbindet Kunden über das Smartphone mit Ihrem Fahrzeug und macht es zu einer intelligenten Schnittstelle
- Remote Software Upgrade
    - Mit dem BMW Operating System 7 und Remote Software Upgrade seit 2018
    - Fahrzeug auf den neusten Softwarestand bekommen
    - über die My BMW App oder over-the-air direkt ins Fahrzeug
    - Ablauf: Installationsdateien im Hintergrund vorbereitet, Installation selber dauert unter 20 Minuten
    - Mittlerweile ist RSU für über 30 BMW Modelle verfügbar
    - Verfügbarkeit ist abhängig von Fahrzeugmodell, Ausstattung und jeweiligem Land -->
<!-- Quelle [@bmwHowErsteSchritteMit2024]:
- Mobiler Zugriff auf Fahrzeug, BMW Services und Stores
- Einloggen mit BMW ID
- Fahrzeug-Tab (Vehicle Tab): Überblick über Fahrzeugstatus und Remote-Funktionen, "Meine Fahrten" mit Informationen über Fahrten und Fahrverhalten, Charging Hub für Informationen über Elektrofahrzeuge
- Karten-Tab: Karte mit Sonderzielen (Park-, Tank, Ladestationen), Ziele können an Fahrzeug geschickt werden
- Explore-Tab: Neuigkeiten und praktische Tipps zu Benutzung des BMW-Fahrzeuges
- Message Center: personalisierte Informationen (z.B. RSU verfügbar)
- BMW Services und Store Tab: BMW Connected Drive Upgrades, Kontakt zu Service Partnern, Finanzdienstleistungen, BMW Stores, Buchung von Probefahrt
- Profil-Tab: persönliche Einstellungen, Hilfecenter, Datenschutzeinstellungen -->
<!-- Quelle [@julichNeueSoftwareFuer2023] - nicht benutzt!
- Remote Software Upgrade ist für über 30 Modelle und damit fast alle BMW Modelle mit BMW Operating System 7 und 8 verfügbar
- Kunden können im Einstellungsmenü des Fahrzeugs unter Remote Software Upgrade den Softwarestand abrufen und verfügbare Updates suchen -->
<!-- Quelle [@tholundUmfangreicheUpdatesMy2024]
- Über 13 Millionen Nutzer weltweit (My BMW und Mini)
- fünf Updates pro Jahr -->


## Suchfunktionen in Mobilen Anwendungen

Suchfunktionen stellen in einigen mobilen Anwendungen eine wichtige Funktion dar. In den letzten Jahren wurden in diesem Bereich einige interessante Erkenntnisse gewonnen. 
So wurde 2012 festgestellt, dass Nutzer bei der Verwendung von mobilen Telefonen weniger Anfragen per Sitzung schicken, als bei der Verwendung eines Desktop PCs. Das impliziert, dass Nutzer die Suche am Handy als eine größere Hürde sehen. [@komakiHowDoesMobile2012]

<!-- Quelle [@komakiHowDoesMobile2012]:
- In Studie: Mehr Anfragen per Session an einem Desktop PC als an einem Mobilen Telefon, was impliziert, dass Mobile Nutzer weniger dazu bereit sind Themen in Tiefe zu erkunden wegen größeren Hürden beim Suchen, wie Query-Eingabe
- Nützlich für Suchanfragen: Voice search, push-based information recommendation services -->
<!-- Quelle [@churchLargeScaleStudy2008]: unused.
- This study analyzed one million page requests from Google and focused on features such as query length, target content, and relationship between queries and device characteristics. They found that users with less sophisticated input capabilities submitted shorter queries and adult content was the most prevalent search topic. -->
<!-- Quelle [@kamvarDecipheringTrendsMobile2007] (von 2007, also bisschen Alt): unused
- durchschnittliche Mobile Query: 2.56 Wörter und 16.8 Charakter (auch andere Studien zeigen ähnliche Ergebnisse) -->
<!-- Quelle [@maMashDroidApproach2015]: unused
- Im Kontext, Apps für Durchsuchung des App-Stores oder einfach aller Funktionen durchsuchbar zu machen (man sucht nach Inhalt der App im AppStore und bekommt dann App vorgeschlagen, z.b. "Harry Potter" und man bekommt Apps mit Ebooks oder Filmen angezeigt und landet dann direkt im gesuchten Inhalt):
    - Kein tieferes Wissen darüber, welche Daten oder Funktionalitäten eine App bereitstellt. Wenn man jede App als eine einzelne Webseite sehen würde, könnte man mit einem WebCrawler oder einer Search Engine durchsuchen, um den dynamischen Content zu bekommen. Damit bekommt man eine tieferes Verständnis für für die Daten und Content innerhalb der App und könnte Korrelationen zwischen den Apps finden.
    - Dies ist jedoch ziemlich schwierig, da die Genehmigung von App-Entwicklern erforderlich ist, um ein Codefragment für die Indexerstellung zu instrumentieren, genauso wie Webentwickler Google Analytics-Code in ihre HTML-Codes aufnehmen, um die Seiten zu indizieren. 
    - Neben des Beschreibung im App Store sind Apps Black-Boxes (nur .apk / .ipa file)
- Funktion von "Wandoujia App Store (WDJ)": Damit Apps Zugriff auf In-App Search (IAS) haben, muss jeder Content eine assigned APP-URL haben und das URL Pattern muss registered in the intent by intent-filter sein. Zusätzlich dazu dann: Semantische Analyse, Filter, Ranking Algorithms, um die most likely App to be used zu finden
- Modellierung von Apps für Suchfunktionen:
    - Das RESTful-Stil-App-Modell abstrahiert Apps als Sammlungen von Ressourcen, auf die über standardisierte Operationen (GET, POST, etc.) zugegriffen werden kann
    - Das ressourcenorientierte App-Beschreibungsmodell ermöglicht eine strukturierte Erfassung der Inhalte und Funktionalitäten der Apps
    - Diese Modellierung erleichtert das maschinelle Verständnis und die gezielte Suche nach relevanten App-Funktionen
- Ansatz ist technisch umsetzbar, Algorithmus um dann die Durchsuchung mehrere Apps zu machen ist nicht relevant. -->

## API-Entwicklung

APIs, Application Programming Interfaces, sorgen für eine nahtlose Kommunikation zwischen Software Komponenten und Services. Sie sind unverzichtbar für die Verbindung verschiedener Systeme und ermöglichen die Nutzung von Drittanbieterdiensten, wie Services, Daten und Funktionalitäten. [@selvarajMasteringRESTAPIs2024]
Sie vereinfachen und beschleunigen Entwicklung von Anwendungen und Software. Daten können gemeinsam genutzt werden, wobei nur notwendige Informationen freigegeben werden und systeminterne Details verborgen bleiben können. [@ibmWhatAPIApplication2024]

**Missing**: Mehr zu internen APIs

Eine gute Implementierung ist besonders bei Mobilen Applikationen wichtig, da sich API-Instabilität und Fehleranfälligkeit auf den Erfolg der Software auswirken können. Google Play Bewertungen haben gezeigt, dass APIs, die von erfolgreichen Apps verwendet werden weniger fehleranfällig sind. Denn Fehleranfällige APIs können zu Fehlfunktionen und Abstürzen führen. [@linares-vasquezAPIChangeFault2013]


<!-- Quelle [@selvarajMasteringRESTAPIs2024]:
- APIs:
    - spielen eine pivotal Rolle darin, eine nahtlose Kommunikation zwischen Software Komponenten und Services herzustellen
    - APIs sind unverzichtbar für die Verbindung verschiedener Systeme, ermöglichen es Entwicklern, die Leistungsfähigkeit von Drittanbieterdiensten zu nutzen und die Interoperabilität zu fördern
    - Wichtigkeit: pivotal Rolle als das verbindene Tissue zwischen verschiedenen Software Systemen
    - ermöglichen nahtlose Integration und Kommunikation, damit können Entwickler existierende Services, Daten und Funktionalitäten nutzen und damit den Entwicklungsprozess beschleunigen und die Effizienz verbessern

    - RESTful Apis: 
        - Typ von Web-API, das einen Satz von Architektur-Prinzipen und Conventions folgt, für das die Design und die Intraktion mit Ressourcen über das Internet. Weitverbreitet für die Erstellung von Web Services und building distributed and scalable Web Anwendungen. 
        - Bild davon: 
        ![Source: Source: comScore MMX Multi-Platform, January 2017 (falls ich des brauche) \label{martinMobilesHierarchiyNeeds2017_composition}](source/figures/selvarajMasteringRESTAPIs2024_RESTAPI_image.png){ width=100% }       -->
    
APIs in Mobile Apps:

<!-- - Quelle [@maMashDroidApproach2015]: unused
    - Fast alle "networked Mobile Apps" greifen auf RESTful Web services/APIs zu und verwenden HTTP(s) als Transfer-Protokol
    - Dienstanbieter stellen ihre Funktionen über über das Internet zugängliche APIs als Dienste zur Verfügung, und die mobilen Apps könnten diese APIs aufrufen, die normalerweise in RESTful-Form bereitgestellt werden. Derzeit treten mobile Apps an die Stelle von Desktop-Anwendungen wie Browsern als neuer dominanter Dienstleistungsverbraucher. -->
<!-- - Quelle [@selvarajMasteringRESTAPIs2024]: unused
    - Mobile Apps als Use Case für APIs: RESTful APIs spielen eine entscheidende Rolle umd Mobile Apps mit Backend-Servern zu verbinden
    - Mobile Apps können Daten abrufen, User authentifizieren, verschiedene Aktionen durchführen indem sie mit RESTful APIs interagieren -->
<!-- Quelle [preibischAPIDevelopmentPractical2018]: unused
- Client-seitige API: 
    - versteckt die Komplexität die hinter den Requests an den Server steckt
    - Eine einzigee client-side API interagiert häufig mit einer oder mehreren Server-seitigen APIs
- Server-seitige API:
    - Eine serverseitige API bietet einen klar definierten Einstiegspunkt in ein geschlossenes System und aus diesem heraus
- Vorteile von Benutzung von APIs
    - Integration: Unternehmen wollen in der Lage sein, sich in andere Systeme zu integrieren und, dass andere Systeme in ihre Systeme integriert werden. 
    - Modernisierung: trotz Modernisierung bleiben APIs relevant
    - Automatisierung: APIs können verwendet werden, um den Build-Prozess von Software Produkten zu automatisieren -->
<!-- Quelle [@linares-vasquezAPIChangeFault2013]:
- API-Instabilität und Fehleranfälligkeit können sich auf den Erfolg der Software auswirken: APIs die von erfolgreichen (anhand von Google Play Bewertung gemessen) Apps verwendet werden sind weniger fehleranfällig, als jene, die von erfolgloseren verwendet werden
- denn: fehleranfällige APIs können zu Fehlfunktionen und Craches in Mobilen Apps führen
- Veränderungen bei API: Updates häufiger notwendig -->
<!-- Quelle [@payneMakingRESTfulAPI2024]: unused
- Hintergrund: Server-Side Programm, um Daten in einer kontrollierten Art zu lesen und zu bearbeiten mithilfe von Protokollen wie https. Zum Lesen: http request mit credentials (username/password oder API key)
- APIs geben die Daten fast immer in einem JSON Format zurück -->
<!-- Quelle [@ibmWhatAPIApplication2024]:
- Definition
    - API = application programming interface, also Anwendungsprogrammierschnittstelle
    - Satz von Regeln oder Protokollen, die es Softwareanwendungen ermöglichen miteinander zu kommunizieren, um Daten, Merkmale und Funktionen auszutauschen
    - Vorteile:
        - vereinfachen und beschleunigen die Anwendungs- und Softwareentwicklung
        - ermöglichen es Entwicklern Daten, Dienste und Funktionen aus anderen Anwendungen zu integrieren, anstatt sie von Grund auf neu zu entwickeln
        - bieten Anwendungseigentümern eine einfache und sichere Möglichkeit, ihr Anwendungsdaten und -funktionen den Abteilungen innerhalb eines Unternehmens zur Verfügung zu stellen oder sie an Geschäftspartner / Dritte weiterzugeben oder zu vermarkten
    - ermöglichen gemeinsame Nutzung so, dass nur notwendige Informationen gezeigt werden und interne Systemdetails verborgen bleiben (verstärkt Systemsicherheit), APIs ermöglichen gemeinsame Nutzung kleiner Datenpakete, die für jeweilige Aufgabe relevant sind
    - Dokumentation: wie technische Bedienanleitung
- Funktionsweise:
    - API-Kommunikation ist wie Anfrage zwischen Client und Server (Client stellt Anfrage, Server liefert Antwort), API ist die Brücke die die Verbindung herstellt
- Arten von APIs:
    - Verschiedene Verwendungszwecke:
        - Daten(banken) APIs: zur Verbindung von Anwendungen und Datenbankverwaltungssystemen
        - Betriebssystem (lokale) APIs: legen fest, wie Anwendungen Dienste und Ressourcen des Betriebssystems nutzen
        - Entfernte (Remote) APIs: definieren, wie Anwendungen auf verschiedenen Geräten interagieren
        - Web-APIs: Übertragung von Daten und Funktionen mit HTTP-Protokollen
        - Meist verbreitet sind Web-APIs, auch dort gibt es offene APIs (quelloffene Schnittstelle zu Anwendungsprogrammierung), Partner APIs (verbinden strategische Geschäftspartner über Entwicklungsportal), Interne APIs (bleiben für externe Benutzer verborgen), zusammengesetzte (composite) API (kombinieren mehrere Daten- oder Service-APIs, damit mit einzelnem Aufruf Zugriff auf mehrere Eckpunkte)
- Verwendungen und Beispiele: Universal Logins (z.b. mit Google-Konto), Internet of Things (Smart Home Objekte), Vergleichsseiten z.B. für Flüge, Navigations-Apps (Daten über Tempolimit etc.)  etc. -->

# Flutter
