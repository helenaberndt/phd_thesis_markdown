# Grundlagen

## Suchfunktionen in Mobilen Anwendungen

Suchfunktionen in mobilen Anwendungen sind heutzutage äußerst wichtig, da viele Nutzer regelmäßig mit ihren mobilen Geräten nach Produkten, Dienstleistungen und Informationen suchen. Unternehmen müssen daher sicherstellen, dass ihre mobilen Anwendungen ein gutes Such- und Entdeckungserlebnis bieten, um die Erwartungen der Zielgruppe zu erfüllen. [@deeBestPracticesInapp2024]

2012 wurde festgestellt, dass Nutzer weniger Suchanfragen pro Sitzung stellen, wenn sie ein Mobiltelefon verwenden, als wenn sie einen Desktop-PC verwenden. Dies deutet darauf hin, dass Nutzer die mobile Suche als größere Hürde empfinden.[@komakiHowDoesMobile2012]

<!-- Quelle [@gettoStateMobileUX2020]:
- Allgemein: There is also strong consensus that mobile applications should meet the same criteria for usability as desktop applications -->

Trotzdem besteht ein starker Konsens darüber, dass mobile Anwendungen die gleichen Usability-Anforderungen erfüllen sollten wie Desktop-Anwendungen. [@gettoStateMobileUX2020]

Bei der mobilen Suche muss die Balance gefunden werden, dem Nutzer die relevanten, gesuchten Inhalte, die er sucht, zu liefern, ihn aber nicht zu überfordern, was dazu führen kann, dass die Suche verfeinert und wiederholt werden muss. Es ist sinnvoll, die Benutzerfreundlichkeit durch Funktionen wie Filter, Rechtschreibfehlertoleranz, Vorschläge und frühere Suchanfragen zu verbessern. [@deeBestPracticesInapp2024]

_todo Missing: Hier noch mehr Quellen suchen_

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

Damit Apps möglichst viele Kunden erreichen, müssen sie mit den unabhängigen Plattformen iOS und Android kompatibel sein. Derzeit laufen etwa 70 % der Mobiltelefone weltweit mit dem Betriebssystem Android, 29 % mit iOS [@SmartphoneUsageOperating2024]. Dies stellt Unternehmen oftmals vor Schwierigkeiten, da sie mit der Komplexität plattformübergreifender Anwendungen umgehen müssen. Entwickler benötigen oft unterschiedliche Skillsets und müssen Apps aufgrund der unterschiedlichen Plattformen mehrfach bauen.
Mit Flutter, das 2016 von Google als mobiles SDK angekündigt worden ist, haben Entwickler nun die Möglichkeit ein plattformübergreifendes Framework zu nutzen, das hochperformante mobile Anwendungen für beide Plattformen, iOS und Android, baut.
Flutter-Apps werden in der Programmiersprache Dart geschrieben, die ursprünglich JavaScript ersetzen sollte und deshalb eine Java-ähnliche Syntax hat.
Entwickler können nur die 'just-in-time' Kompilierung verwenden, wobei der Computercode während der Programmausführung zur Laufzeit kompiliert wird. Darüber hinaus hilft die 'Hot-Reload' Funktion den Entwicklern, Benutzeroberflächen zu bauen oder Features hinzuzufügen, ohne dass diese Änderungen lange neu geladen werden müssen. Denn die aktualisierten Quelldaten werden in die laufende Dart Virtual Machine eingefügt, die die betroffenen Klassen aktualisiert und den Widget-Tree automatisch neu baut.
Flutter erleichtert somit die Entwicklung von Apps, indem es den Entwicklern zeitsparende Tools bietet und durch die plattformübergreifende Entwicklung wertvolle Ressourcen schont. [tashildarApplicationDevelopmentUsing2020]


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

Im Jahr 2020 hat die BMW Group die MyBMW- bzw. Mini-App veröffentlicht, die den Kunden einen digitalen Zugang zu ihrem Fahrzeug ermöglicht. Die Entwicklung basiert auf dem Feedback und den Erkenntnissen aus dem Nutzerverhalten der Vorgängergenerationen, der BMW i Remote App und der BMW Connected App. [koenigYourWorldMy2020]

Derzeit nutzen mehr als 13 Millionen Nutzer die App. Sie wird etwa fünf Mal im Jahr durch Updates aktualisiert. [@tholundUmfangreicheUpdatesMy2024]

Für die Entwicklung der App wurde Flutter verwendet, ein Open-Source-Framework, das nativ kompilierte und plattformübergreifende Anwendungen aus einer einzigen Codebasis erstellt. [flutterFlutterBuildApps] Auf dieser Grundlage ist es möglich, die App sowohl für Android und iOS als auch für die verschiedenen Skins und Regionen zu bauen. Die Skins repräsentieren die Marken BMW, BMW M, Mini und Toyota. Zusätzlich gibt es spezifische Versionen für ausgewählte Regionen, wie Nordamerika oder Korea. Daraus resultieren ca. 30 Apps, die den Kunden in Apps Stores angeboten werden. Das Team von ca. 250 Entwicklern, von denen einige bereits seit 2018 an der App arbeiten, ist eines der größten Flutter Entwicklungsteams. [@tasiorDevelopersCars]

Die App bietet dem Kunden eine universelle Schnittstelle zum Fahrzeug. Damit können Remote-Funktionen ausgeführt werden, mit denen der Fahrzeug- oder Ladestatus, die Reichweite oder die Türen und Fenster des Autos aus der Ferne über das Mobiltelefon überprüft werden können. Die Funktionen sind optimiert für Fahrzeuge ab dem Baujahr 2014 und abhängig von Fahrzeugausstattung und länderspezifischen Vorgaben. [@bmwgroupHighlightsMyBMW]

Mit der App können Kunden nach Anmeldung mit ihrer BMW-ID auf ihr Fahrzeug, BMW Services und Store zugreifen. Dabei ist die App in mehrere Unterseiten (Tabs) aufgeteilt. Im Fahrzeug-Tab kann sich der Kunde einen Überblick über den aktuellen Zustand seines Autos verschaffen, also Fahrzeugstatus und Remote-Funktionen, sowie unter anderem auf die Funktion 'Meine Fahrten' zugreifen. Im Karten-Tab können Ziele zur Navigation gesucht und ausgewählt werden. Der BMW-Services- und Store-Tab gibt den Kunden direkten Zugriff auf Updates und Finanzdienstleistungen und bietet Kontakt zu Service Partnern. Im Profil-Tab können persönliche Einstellungen vorgenommen werden. [@bmwHowErsteSchritteMit2024]

Ein besonderes Feature ist das Remote Software Upgrade. Damit können Updates für die Fahrzeugsoftware direkt 'over-the-air' ins Fahrzeug oder zunächst in die MyBMW-App und dann auf das Auto geladen werden. [@julichUpdateFuerFreude2021] 

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

APIs sorgen für eine nahtlose Kommunikation zwischen Software Komponenten und Services. Sie sind unverzichtbar für die Verbindung verschiedener Systeme und ermöglichen die Nutzung von Diensten, Daten und Funktionalitäten Dritter. [@selvarajMasteringRESTAPIs2024]

Sie vereinfachen und beschleunigen die Entwicklung von Anwendungen und Software. Daten können gemeinsam genutzt werden, wobei nur die notwendigen Informationen freigegeben werden und systeminterne Details verborgen bleiben können. [@ibmWhatAPIApplication2024]

_todo Missing: Mehr zu internen APIs_

Eine gute Implementierung ist besonders bei mobilen Applikationen wichtig, da Instabilität und Fehleranfälligkeit der API den Erfolg der Software beeinträchtigen können. Google Play-Bewertungen haben gezeigt, dass APIs, die von erfolgreichen Apps verwendet werden, weniger fehleranfällig sind. APIs, die zu Fehlern neigen, können zu Fehlfunktionen und Abstürzen führen. [@linares-vasquezAPIChangeFault2013]


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

**Anmerkungen von Wischhof**

hier dann noch vll mehr zur bedienbarkeit von suchfunktionen und ux noch mehr 

- suchfunktionen allgemein
- wie user interfaces
- prototyping für interfaces

- my bmw app nicht gleich zu beginn
