# Grundlagen

## Suchfunktionen in Mobilen Anwendungen

In der heutigen Zeit ist die Relevanz von Suchfunktionen in mobilen Anwendungen signifikant gestiegen, da eine Vielzahl von Nutzern regelmäßig mit ihren mobilen Geräten nach Produkten, Dienstleistungen und Informationen sucht. Unternehmen müssen daher sicherstellen, dass ihre mobilen Anwendungen ihren Kunden ein gutes Such- und Entdeckungserlebnis bieten, um die Erwartungen der Zielgruppe zu erfüllen. [@deeBestPracticesInapp2024]

Die Suche in mobilen Anwendungen unterscheidet sich von den Suchfunktionen in Desktop-Anwendungen. Im Jahr 2012  wurde festgestellt, dass Nutzer weniger Suchanfragen pro Sitzung stellen, wenn sie ein Mobiltelefon verwenden, als wenn sie einen Desktop-PC verwenden [@komakiHowDoesMobile2012]. Dies deutet darauf hin, dass Nutzer die mobile Suche als größere Hürde empfinden. Trotzdem besteht ein starker Konsens darüber, dass mobile Anwendungen die gleichen Usability-Anforderungen erfüllen sollten wie Desktop-Anwendungen. [@gettoStateMobileUX2020]

<!-- Quelle [@gettoStateMobileUX2020]:
- Allgemein: There is also strong consensus that mobile applications should meet the same criteria for usability as desktop applications -->

Bei der mobilen Suche muss die Balance gefunden werden, dem Nutzer die relevanten, gesuchten Inhalte, die er sucht, zu liefern, ihn aber nicht zu überfordern, was dazu führen kann, dass die Suche verfeinert und wiederholt werden muss. Es ist sinnvoll, die Benutzerfreundlichkeit durch Funktionen wie Filter, Rechtschreibfehlertoleranz, Vorschläge und frühere Suchanfragen zu verbessern. [@deeBestPracticesInapp2024]

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

## Flutter

Die Entwicklung plattformübergreifender Anwendungen ist für Unternehmen von entscheidender Bedeutung, um die breite Masse an Kunden zu erreichen. Dies ist jedoch mit einer gewissen Komplexität verbunden, da die Plattformen iOS und Android, auf denen die Anwendungen ausgeführt werden, unterschiedliche Funktionalitäten und Anforderungen aufweisen. Aktuell werden weltweit etwa 70 % der Mobiltelefone mit dem Betriebssystem Android und 29 % mit iOS betrieben [@SmartphoneUsageOperating2024]. Entwickler benötigen in der Regel unterschiedliche Fertigkeiten und müssen Apps aufgrund der unterschiedlichen Plattformen mehrfach erstellen. [@tashildarApplicationDevelopmentUsing2020]

Mit Flutter steht Entwicklern nun ein plattformübergreifendes Open-Source-Framework zur Verfügung, das die Erstellung hochperformanter mobiler Anwendungen aus einer einzigen Codebasis für die beiden Plattformen iOS und Android ermöglicht [flutterFlutterBuildApps]. Die mobile SDK wurde 2015 durch Google angekündigt [@napoliBeginningFlutterHands2019] und der erste Release wurde Ende 2018 publiziert [@FlutterSDKArchive].

Flutter-Apps werden in der Programmiersprache Dart verfasst, die ursprünglich die Funktion von JavaScript übernehmen sollte und daher eine der Programmiersprache Java ähnliche Syntax aufweist. Flutter erleichtert die Entwicklung durch Funktionen und zeitsparende Tools. So können Entwickler die 'just-in-time' Kompilierung verwenden, bei der der Computercode während der Programmausführung zur Laufzeit kompiliert wird. Darüber hinaus ermöglicht die 'Hot-Reload' Funktion den Entwicklern, Benutzeroberflächen zu gestalten oder Features hinzuzufügen, ohne dass diese Änderungen lange neu geladen werden müssen. Denn die aktualisierten Quelldaten werden in die laufende Dart Virtual Machine eingefügt, die die betroffenen Klassen aktualisiert und den Widget-Tree automatisch neu baut. [@tashildarApplicationDevelopmentUsing2020]

BMW hatte in der nativen Entwicklung früherer Anwendungen Schwierigkeiten, da die Entwicklungsprozesse als zu aufwendig erachtet wurden. Daher wurde bei der Konzeption einer neuen Anwendung von Beginn an die Entscheidung getroffen, Flutter als Entwicklungsframework zu verwenden. Diese Wahl ermöglicht es, die Vorteile der SDK zu nutzen und eine plattformübergreifende Entwicklung zu realisieren. [@tasiorDevelopersCars]

<!--Quelle [tashildarApplicationDevelopmentUsing2020]: -->
<!-- - damit App möglichste viele Kunden erreicht, müssen Apps mit den zwei unabhängigen Plattformen IOS und Android familiarizen, diese sind sehr unterschiedlich, weshalb es oft verschiedene Entwickler mit einem unterschiedlichen Skill-Set braucht, Firmen haben also oft Schwierigkeiten mit der Komplexität der Entwicklung plattformübergreifenden Anwendungen umzugehen -->
<!-- - eigentlich: 
    - Entwickler müssen bzw. mussten wegen der verschiedenen Plattformen Apps mehrfach bauen oder eine Lösung mit niedrigerer Qualität akzeptieren, wenn sie ähnliche Ansätze für verschiedene Plattformen verwenden müssen (z.b. Native Speed und Accuracy for portability)
    - mit Flutter: Flutter ist abhängig von den OEM widets des Devices, anstatt, dass web views konsumiert werden; benutzt eine high-performance rendering enging, um jedes component einzeln genutzt werden kann -->
<!-- - Entwicklung: in zweiten Hälfte von 2016 hat Google eine mobile SDK angekündigt namens 'Flutter' -->
<!-- - Plattformübergreifendes Framework, das hochperformante Mobile Anwendungen baut -->
<!-- - Features von Flutter:
    - Flutter kann auf beiden Plattformen, also iOS und Android laufen. Das reduziert die Kosten und Komplexität der Appentwicklung
    - Just-in-time compilation: bei der der Computercode, der die Kompilierung umfasst, während der Programmausführung zur Laufzeit und nicht vor der Ausführung ausgeführt wird
    - Hot-Reload: 
        - Hilft beim Entwickeln (rumexperiementieren, UI bauen, features hinzufügen, Bugs bzw. Fehler lösen)
        - Funktionsweise: Aktualisierte Quell-Dateien  werden in die laufende Dart Virutal Machine (Dart VM) eingefügt, die VM updated dann Klassen mit der neuen Version der Felder und Funktionen; das Flutter Framework baut dann automatisch den Widget-Tree neu, wodurch der Entwickler seine Änderunden schnell sehen kann; ohne Änderung der inneren Struktur der Applikation. Transaktionen und Aktionen der App sind well-preserved -->
<!-- - Dart:
    - Jede flutter-App ist mit Dart geschrieben, programmiert worden
    - Dart sollte ursprünglich JavaScript ersetzen und nachfolgen
    - Dart hat eine Java-ähnliche Syntax -->


## Die MyBMW App

Im Jahr 2020 hat die BMW Group die MyBMW- bzw. Mini-App veröffentlicht, die den Kunden einen digitalen Zugang zu ihrem Fahrzeug ermöglicht. Die Entwicklung der App basiert auf dem Feedback und den Erkenntnissen aus dem Nutzerverhalten der Vorgängergenerationen, der BMW i Remote App und der BMW Connected App. [koenigYourWorldMy2020]

Derzeit nutzen mehr als 13 Millionen Nutzer die App. Sie wird etwa fünf Mal im Jahr durch Updates aktualisiert. [@tholundUmfangreicheUpdatesMy2024]

Für die Entwicklung der App wurde Flutter verwendet. Auf dieser Grundlage ist es möglich, die Applikation sowohl für Android und iOS als auch für die verschiedenen Skins und Regionen mit der gleichen Code-Basis zu entwickeln und bauen. Die Skins repräsentieren die Marken BMW, BMW M, Mini und Toyota. Darüber hinaus existieren spezifische Versionen für vorgegebene Regionen, wie Nordamerika oder Korea. Daraus resultieren ca. 30 Apps, die den Kunden in den Apps Stores angeboten werden. Das Team von ca. 250 Entwicklern ist eines der größten Flutter Entwicklungsteams. [@tasiorDevelopersCars]

Die Applikation stellt dem Kunden eine universelle Schnittstelle zum Fahrzeug bereit. Mittels dieser Schnittstelle können Remote-Funktionen ausgeführt werden, womit der Fahrzeug- oder Ladestatus, die Reichweite sowie die Türen und Fenster des Autos aus der Ferne über das Mobiltelefon überprüft werden können. Die Funktionsweise ist jedoch auf Fahrzeuge ab dem Baujahr 2014 optimiert und kann sich abhängig von der Fahrzeugausstattung sowie länderspezifischen Vorgaben unterscheiden. [@bmwgroupHighlightsMyBMW]

Nach erfolgter Anmeldung mit der BMW-ID ermöglicht die App den Zugriff auf das Fahrzeug, BMW Services und den Store. Die App ist in mehrere Unterseiten, so genannte Tabs, unterteilt. Im Fahrzeug-Tab erhält der Kunde einen Überblick über den aktuellen Zustand seines Autos, also Fahrzeugstatus und Remote-Funktionen. Im Karten-Tab können Ziele zur Navigation gesucht und ausgewählt werden. Der BMW-Services- und Store-Tab bietet den Kunden direkten Zugriff auf Updates und Finanzdienstleistungen und ermöglicht den Kontakt zu Service Partnern. Im Profil-Tab können persönliche Einstellungen vorgenommen werden. [@bmwHowErsteSchritteMit2024]

Ein besonderes Feature ist das Remote Software Upgrade (RSU), mit dem Updates für die Fahrzeugsoftware direkt 'over-the-air' ins Fahrzeug oder zunächst in die MyBMW-App und dann auf das Auto geladen werden. [@julichUpdateFuerFreude2021] 

*todo: hier Bilder?*

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

## API-Entwicklung

APIs sind entscheidend für die nahtlose Kommunikation zwischen Softwarekomponenten und -diensten. Sie sind essenziell für die Verbindung verschiedener Systeme und ermöglichen die Nutzung von Diensten, Daten und Funktionalitäten Dritter. [@selvarajMasteringRESTAPIs2024]

Mit APIs kann auf unterschiedliche Komponenten zugegriffen werden, darunter Hardwarekomponenten, Datenbanken, einzelne Programmfunktionen oder auch Oberflächen. [@luberAPIEntwicklungGrundlagenEigenschaften2024]

Der Begriff API ist vielseitig interpretierbar und kann sich auf eine rein technische Schnittstellenbeschreibung, ein Kommunikationsmittel für Software oder auch um ein digitales Produkt beziehen. In allen Fällen sind APIs kein separates Softwaresystem, sondern lediglich eine Kommunikationsschnittstelle, die der Interaktion mit der Software dient. [@frankBausteineDigitalenTransformation2021] 

Darüber hinaus wird zwischen funktions-, datei-, objekt- und protokollorientierten APIs differenziert. [@luberAPIEntwicklungGrundlagenEigenschaften2024]

Die Eigenschaften von APIs lassen sich wie folgt zusammenfassen: Modularität, das heißt die Zusammensetzung eines Services aus mehreren Services, Interoperabilität, also die Existenz von Standards in der Kommunikation zwischen Diensten, und die Kapselung, bei der die Programmlogik und die Datenbasis des Services verborgen bleiben. [@frankBausteineDigitalenTransformation2021]

Die Modularisierung von Software führt zur Trennung einzelner Programmteile, die spezifische Funktionen erfüllen, und zur Trennung vom Rest der Applikation. Die Kommunikation erfolgt über eine genau definierte Schnittstelle, was zu einer sauberen Gesamtstruktur innerhalb des Projektes führt. Dies kann besonders komplexe Programme vereinfachen. Die einzelnen Programmteile sind leichter wartbar und damit weniger fehleranfällig. [@luberAPIEntwicklungGrundlagenEigenschaften2024]

Die Verwendung von APIs hat sich als signifikant effizienter und beschleunigender Faktor in der Entwicklung von Anwendungen und Software erwiesen. Die gemeinsame Nutzung von Daten ermöglicht die Freigabe spezifischer Informationen, während systeminterne Details verborgen bleiben, was zu einer Optimierung der Sicherheit und Vertraulichkeit beiträgt. [@ibmWhatAPIApplication2024]

Die Implementierung ist ein wesentlicher Faktor für den Erfolg mobiler Applikationen. Instabilität und Fehleranfälligkeit der API können den Erfolg der Software erheblich beeinträchtigen.Die Auswertung der Google Play-Bewertungen hat ergeben, dass APIs, die von erfolgreichen Apps verwendet werden, tendenziell weniger fehleranfällig sind. APIs, die zu Fehlern neigen, können zu Fehlfunktionen und Abstürzen führen. [@linares-vasquezAPIChangeFault2013]


<!-- Quelle [@luberAPIEntwicklungGrundlagenEigenschaften2024]:
- Programmierschnittstelle: standartisierter Austausch von Informationen zweischen Anwendung und einzelnen Programmteilen
- Modularisierung:
    - einzelne Programmteile erfüllen spezifische Funktion, sind von Rest der Applikation klar getrennt
    - Kommunikation nur über genau spezifizierte Schnittstelle
    - komplexe Programme können vereinfacht werden durch Aufteilung
    - damit weniger fehleranfällig und leichter wartbar
    - saubere Gesamtstruktur
- API definiert, in welcher Form Daten entgegengenommen und zurückgesendet werden
- MIt API zugriff auf Hardwarekomponenten, DAtenbanken, einzelne Programmfunktionen oder Oberflächen 
- Schnittstelle auf Quellebene, nicht wie bei User Interface (Benutzerschnittstelle), wo zwischen Anwender und Programm
- unterschiedliche Programmierschnittstellen: funktions-, datei-, objekt-, protokollorientierte APIs -->

<!-- Quelle [@frankBausteineDigitalenTransformation2021]:
- "API" vielseitiger Begriff, kann unterschiedlich interpretiert:
    - rein technische Schnittstellenbeschreibung
    - Kommunikationsmittel für Software
    - digitales Produkt
- API kein seperates Softwaresystem, sondern Kommunikationsschnittstelle, die der Interaktion mit der Software dient
- Eigenschaften: Modularität (Applikation setzt sich aus mehreren SErvices zusammen), Interoperabilität (Standards für Kommunikation zwischen verschiedenen Systemen), Kapselung (Programmlogik und Datenbasis des Software-Bausteins bleibt verborgen) -->

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
    
<!-- APIs in Mobile Apps: -->

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

