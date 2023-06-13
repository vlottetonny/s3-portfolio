## Inhoudsopgave

- [Inhoudsopgave](#inhoudsopgave)
- [Inleiding](#inleiding)
- [Methodologie](#methodologie)
- [Onderzoeksstrategieën](#onderzoeksstrategieën)
- [Instrumenten](#instrumenten)
- [Beperkingen](#beperkingen)
- [Resultaten](#resultaten)
- [Conclusie](#conclusie)
- [Bronnen](#bronnen)

## Inleiding

Dit onderzoek richt zich op het kiezen van de meest geschikte databasetype voor een Housekeeper applicatie. We gaan verschillende databasetypen vergelijken, hun voordelen en nadelen bespreken om zo tot een geïnformeerde beslissing te komen.

## Methodologie

Het onderzoek zal zich concentreren op de vraag:

> "Welke vorm van database is het meest geschikt voor mijn Housekeeper applicatie?"

Om deze hoofdvraag te beantwoorden, hebben we de volgende subvragen:

1. Wat zijn de specifieke behoeften van de Housekeeper applicatie op het gebied van databeheer?
2. Wat zijn de verschillende databasetypen en hun voordelen en nadelen?
3. Hoe passen de specifieke kenmerken van deze databasetypen bij de behoeften van de Housekeeper applicatie?

### Onderzoeksstrategieën

Het onderzoek zal worden uitgevoerd met behulp van het DOT (Development Oriented Triangulation) framework. Voor de vragen worden de volgende onderzoeksstrategieën gebruikt:

| Onderzoeksvraag                                                                                                     | 	Onderzoeksstrategie                            |
|---------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|
| **(1) Wat zijn de specifieke behoeften van de Housekeeper applicatie op het gebied van databeheer?**                | Stakeholder Analysis, Explore User Requirements |
| **(2) Wat zijn de verschillende databasetypen en hun voordelen en nadelen?** 	                                      | Literature Study, Competitive analysis          |
| **(3) Hoe passen de specifieke kenmerken van deze databasetypen bij de behoeften van de Housekeeper applicatie?** 	 | Gap analysis, Domain modelling                  |

### Instrumenten

De volgende instrumenten worden gebruikt:

1. Housekeeper applicatie: Dit project zal als voorbeeld worden gebruikt om een geschikte database voor te selecteren.
2. Literatuur: Wetenschappelijke artikelen, boeken, en betrouwbare online bronnen zullen worden gebruikt om de verschillende databasetypen te onderzoeken.

### Beperkingen

Het onderzoek zal zich alleen richten op de Housekeeper applicatie en de bevindingen zijn mogelijk niet van toepassing op andere applicaties met andere eisen en behoeften.

## Resultaten

### 1. Wat zijn de specifieke behoeften van de Housekeeper applicatie op het gebied van databeheer?

#### Stakeholder Analysis

**Stakeholder:** Eigenaar van de Housekeeper applicatie.

**Doel van de applicatie:** De Housekeeper applicatie is ontworpen om een huishouden te helpen bij het gezamenlijk beheren van hun taken, boodschappenlijsten, agenda's en het achterlaten van notities voor elkaar.

**Functies van de applicatie:**
- Het bijhouden van gezamenlijke boodschappenlijsten.
- Het bijhouden van een gezamenlijke agenda of kalender.
- Het achterlaten van notities voor elkaar.
- Het opstellen van takenlijsten zoals het uitruimen van de vaatwasser of het buitenzetten van afval.

**Gebruikers van de applicatie:**
- Gebruikers, die een huishouden kunnen creëren of zich kunnen aansluiten bij een bestaand huishouden.

**Datagebruik en -beheer:**
- De applicatie moet real-time reflecteren op de updates gemaakt door de gebruikers, dit omvat toevoegen, bijwerken en verwijderen van items van de lijsten, taken, notities en kalender.
- De login-informatie van de gebruikers wordt gehashed en veilig in de database opgeslagen.

**Data-integriteit en veiligheid:**
- Hoge mate van integriteit en veiligheid is vereist, met name voor het opslaan van gehashte gebruikerslogin-informatie.

**Prestaties en schaalbaarheid:**
- De applicatie begint klein, maar er moet ruimte zijn voor mogelijke schaalvergroting in de toekomst.

**Budget en tijd:**
- Er zijn geen specifieke budget- of tijdsbeperkingen voor de database-gerelateerde aspecten van de applicatie.

#### Conclusie
Deze analyse suggereert dat de databasemodellen die overwogen moeten worden, in staat moeten zijn om:

1. Real-time updates te ondersteunen.
2. Veilige opslag van gevoelige gegevens (zoals gehashte wachtwoorden) te garanderen.
3. Mogelijkheden te bieden voor toekomstige schaalvergroting.

Dit geeft ons een duidelijk beeld van de specifieke behoeften van de Housekeeper applicatie op het gebied van databeheer, die zullen helpen bij het beantwoorden van de volgende onderzoeksvragen.

#### Explore User Requirements

**Gebruikersprofielen:**

- Gebruikers van de Housekeeper-applicatie variëren in leeftijd en technische vaardigheden. De applicatie zal altijd ten minste één volwassene per huishouden bedienen, omdat elk huis minimaal één volwassen bewoner heeft.

**Taken:**

- Gebruikers verwachten dat ze gezamenlijke boodschappenlijsten kunnen bijhouden.
- Ze willen een gedeelde kalender bijhouden voor belangrijke data zoals verjaardagen.
- Ze willen taken kunnen toewijzen aan andere huisgenoten, zoals het buitenzetten van afval.

**Frequentie van gebruik:**

- Gebruikers zullen de applicatie meerdere keren per dag gebruiken.

**Functionaliteit en gebruiksvriendelijkheid:**

- De applicatie moet eenvoudig genoeg zijn om door gebruikers van alle leeftijden te worden gebruikt.

**Gegevensprivacy:**

- Gebruikers zijn bereid om gegevens te delen met hun huisgenoten.

**Fouttolerantie:**

- Dit aspect is niet specifiek besproken, maar op basis van algemene gebruikersverwachtingen kunnen we aannemen dat gebruikers een hoge fouttolerantie en snelle oplossingen verwachten in het geval van problemen.

### Conclusie

Op basis van deze vereisten, zullen we rekening moeten houden met een databasemodel dat kan voldoen aan:

1. De behoefte aan hoge frequentie updates.
2. De verwachting dat de database de toewijzing van taken, evenementen en boodschappenlijsten aan specifieke gebruikers zal ondersteunen.
3. De privacyvereisten van het delen van gegevens alleen tussen huisgenoten.
4. De noodzaak om eenvoudig en intuïtief te zijn, gezien de brede variatie in de technische vaardigheden van de gebruikers.

Met deze vereisten in gedachten, kunnen we de volgende onderzoeksvragen beter beantwoorden.

### 2. Wat zijn de verschillende databasetypen en hun voordelen en nadelen?

#### Literature Study
Er zijn veel verschillende soorten databases. Hier zijn enkele van de meest voorkomende:
- Relationele databases
- Object-georiënteerde databases
- NoSQL databases
- Hiërarchische databases
- Netwerkdatabases
- Document databases
- Grafische databases

Ik ga nu van de eerste drie typen databases onderzoeken om hun voordelen en nadelen te ontdekken. Ik doe ze niet allemaal omdat ik niet genoeg tijd heb om ze allemaal te vergelijken. In plaats daarvan heb ik ze allemaal vlug bekeken en ga ik in op de types die ik het meest interessant vond. Ik zal beginnen met het zoeken naar informatie over relationele databases.
Relationele databases hebben verschillende voordelen:
- Snelheid: Ondanks dat relationele databases niet altijd optimale prestaties leveren, zijn ze over het algemeen sneller vanwege hun eenvoud en verschillende optimalisaties die erin zijn opgenomen.
- Beveiliging: Bepaalde tabellen in een relationele database kunnen vertrouwelijk worden gemaakt en worden beschermd met een gebruikersnaam en wachtwoord, zodat alleen geautoriseerde gebruikers toegang hebben.
- Eenvoud: In vergelijking met andere soorten netwerkmodellen is een relationeel databasemodel veel eenvoudiger.
- Toegankelijkheid: Een relationele database kan worden benaderd zonder dat er een specifieke pad nodig is.
- Nauwkeurigheid: Alle opgeslagen gegevens zijn uniek, wat betekent dat er geen duplicaten zijn.
- Multi-user: Meerdere gebruikers kunnen tegelijkertijd toegang hebben tot een relationele database.

Er zijn echter ook nadelen:
- Kosten: de onderliggende kosten van een relationele database kunnen behoorlijk hoog zijn.
- Prestaties: de prestaties van de relationele database zijn afhankelijk van het aantal tabellen.
- Fysieke opslag: een relationele database vereist een enorme hoeveelheid fysiek geheugen.
- Complexiteit: wanneer de hoeveelheid gegevens in een relationele database toeneemt, kan het systeem ingewikkelder worden.
- Informatieverlies: dit kan een risico vormen bij het overdragen van informatie van het ene systeem naar het andere.
- Structuurbegrenzingen: de velden in een relationele database hebben beperkingen.

DatabaseTown. (n.d.)/ Relational Database Benefits and Limitations (Advantages & Disadvantages) Op June 13, 2023, van https://databasetown.com/relational-database-benefits-and-limitations/. <br/>
HiTechWhizz. (2021, April). 6 Advantages and Disadvantages of Relational Database | Limitations & Benefits of Relational Database. Op June 13, 2023, van https://www.hitechwhizz.com/2021/04/6-advantages-and-disadvantages-limitations-benefits-of-relational-database.html


Ook Object-georiënteerde databases hebben verschillende voordelen:

- Complexiteit: De object-georiënteerde databasemodel combineert gerelateerde pakketten. Met andere woorden, een gegevensset en al zijn attributen worden gecombineerd met een object. Op deze manier is alle informatie direct beschikbaar. In plaats van alles over verschillende tabellen te verspreiden, kunnen de gegevens in één pakket worden opgehaald. Naast de attributen worden methoden ook opgeslagen in de objecten. Dit is waar de nabijheid van de databases tot objectgeoriënteerde programmeertalen duidelijk wordt. Net als bij programmeren, heeft elk object bepaalde activiteiten die het kan uitvoeren.
- Toegankelijkheid: Objecten worden samengebracht in klassen. Dit genereert een hiërarchie van klassen en subklassen. Binnen een dergelijke constructie nemen subklassen de eigenschappen van hogere klassen over en breiden deze uit met hun eigen attributen. Tegelijkertijd kunnen objecten in één klasse ook worden verbonden met andere klassen. Dit breekt de strikte hiërarchie op en zorgt ervoor dat de objecten onderling verbonden zijn. Eenvoudige objecten kunnen worden gecombineerd met complexe objecten.
- Snelheid: Complexe gegevenssets kunnen snel en gemakkelijk worden opgeslagen en opgehaald.
- Integratie: Werkt goed met objectgeoriënteerde programmeertalen.

Er zijn echter ook nadelen:

- Adoptie: Objectdatabases zijn niet breed geadopteerd. Hoewel het model al sinds de jaren 80 is vastgesteld, hebben tot nu toe maar heel weinig databasebeheersystemen objectdatabases overgenomen. De community die met het model werkt, is dienovereenkomstig klein. De meeste ontwikkelaars geven daarom de voorkeur aan de meer verspreide, goed gedocumenteerde en zeer ontwikkelde relationele databases.
- Prestaties: In sommige situaties kan de hoge complexiteit prestatieproblemen veroorzaken. De complexiteit van de objecten betekent dat complexe queries en operaties veel sneller kunnen worden uitgevoerd dan in relationele modellen. Als de bewerkingen echter eenvoudig zijn, moet de complexe structuur nog steeds worden gebruikt, wat resulteert in een verlies van snelheid.

Phoenixnap. (2021, April). Object-oriented database: Explanation + Advantages & Disadvantages. Op June 13, 2023, van https://phoenixnap.com/kb/object-oriented-database

Als laatste ga ik NoSQL databases onderzoeken. NoSQL databases hebben verschillende voordelen:
- Veelzijdigheid van gegevenstypes: NoSQL-databases hebben het vermogen om een grote verscheidenheid aan gegevenstypes op te slaan, inclusief gestructureerde, semi-gestructureerde en ongestructureerde gegevens. Hierdoor zijn er minder (of geen) transformaties nodig wanneer gegevens worden opgeslagen of opgehaald.
- Schaalbaarheid: NoSQL-databases zijn ontworpen met internet en cloud computing als ondersteunende systemen, waardoor een schaalbare architectuur mogelijk is. Schaalbaarheid wordt bereikt door het datageheugen en de rekenprocessen te verspreiden over een cluster van computers. Het verhogen van de capaciteit vereist simpelweg het toevoegen van meer computers aan het cluster.
- Flexibiliteit van schema's: De schema's van veel NoSQL-databases zijn behoorlijk flexibel en kunnen door de ontwikkelaars worden gecontroleerd. Dit maakt het gemakkelijker om de database aan te passen voor nieuwe vormen van gegevens.
- Ontwikkelaarvriendelijk: NoSQL-databases zijn ontwikkelaarvriendelijk. Ontwikkelaars ontdekten dat ze specifieke applicaties vrij gemakkelijk konden ontwikkelen en aanpassen met NoSQL. Documentdatabases kunnen JSON gebruiken om gegevens om te zetten in een code-achtig formaat, wat de ontwikkelaar in staat stelt de structuur van de gegevens gemakkelijker te beheersen.

Er zijn echter ook nadelen:
- Gebrek aan SQL: Een veel voorkomende klacht over NoSQL is dat het SQL mist. SQL is een volwassen technologie, ontworpen voor het organiseren van gegevens, terwijl NoSQL dat niet is.
- Gebrek aan standaardisatie: Elk merk van NoSQL-database gebruikt zijn eigen unieke schema. Dit betekent dat elk uniek systeem zijn eigen sterke en zwakke punten heeft, die moeten worden geleerd voordat de juiste NoSQL-database voor de situatie kan worden gekozen.
- Gebrek aan ACID: ACID staat voor de vier sleutelkenmerken die een transactie definiëren (Atomicity, Consistency, Isolation, en Durability) en NoSQL ondersteunt deze eigenschappen niet.
- Gebrek aan JOINs: SQL gebruikt JOINs om verbindingen tussen databasetabellen te maken door kolommen te matchen, waardoor een relatie tussen die tabellen wordt gecreëerd. De meeste complexe queries die in een SQL-database worden gebruikt, bevatten join-commando's. In NoSQL databases is dit niet mogelijk.

DATAVERSITY. (n.d.). NoSQL Databases: Advantages and Disadvantages. DATAVERSITY. Op June 13, 2023, van https://www.dataversity.net/nosql-databases-advantages-and-disadvantages/

#### Competitive analysis
Nu kunnen we de drie database types - relationele databases, object-georiënteerde databases en NoSQL databases - met elkaar vergelijken.<br/>
Relationele databases zijn erg populair. Ze zijn snel en gemakkelijk te gebruiken. Maar ze kunnen duur zijn en ingewikkeld worden als je veel informatie hebt. Ook kunnen ze soms moeilijk zijn om te gebruiken als je veel verschillende soorten informatie hebt.<br/>
Object-georiënteerde databases maken het gemakkelijk om met complexe informatie om te gaan. Ze werken goed met objectgeoriënteerde programmeertalen, wat handig is voor programmeurs. Maar niet iedereen gebruikt dit type database. Ook kunnen ze soms traag zijn als je veel simpele taken moet doen.<br/>
NoSQL databases zijn heel flexibel. Je kunt veel verschillende soorten informatie opslaan. Ze zijn ook gemakkelijk te vergroten als je meer ruimte nodig hebt. Maar ze missen enkele functies die andere databases wel hebben, zoals SQL en JOINs. <br/>
In het algemeen kunnen we zeggen dat elk type database zijn eigen sterke punten heeft. Welke het beste is, hangt af van wat je nodig hebt. Als je bijvoorbeeld veel verschillende soorten informatie hebt, kan een NoSQL database een goede keuze zijn. Maar als je veel complexe informatie hebt, is een object-georiënteerde database misschien beter. En als je iets simpels en snels nodig hebt, kan een relationele database de beste keuze zijn. <br/>    

### 3. Hoe passen de specifieke kenmerken van deze databasetypen bij de behoeften van de Housekeeper applicatie?

#### Gap analysis   
Deze gap analysis kijkt naar de situatie voor er een database is gekozen. De gap analysis is gebaseerd op de requirements die zijn opgesteld in de explore user requirements fase. <br/>

**Vereiste:** Real-time updates ondersteunen met meerdere keren per dag per gebruiker.<br/>
**Gap:** Een gap kan ontstaan als de gekozen database geen efficiënte manier biedt om real-time updates af te handelen en ervoor te zorgen dat wijzigingen snel en betrouwbaar worden weergegeven voor alle gebruikers.<br/>

**Vereiste:** Opslaan en beheren van verschillende gegevenstypen, zoals boodschappenlijsten, agenda-items, notities en gebruikersgegevens. <br/>
**Gap:** Een gap kan ontstaan als de gekozen database niet geschikt is voor het opslaan van verschillende gegevenstypen of niet flexibel genoeg is om aan te passen aan toekomstige gegevensbehoeften.<br/>

**Vereiste:** Mogelijkheid om gegevens veilig op te slaan, inclusief het bewaren van gehashte wachtwoorden. <br/>
**Gap:** Een gap kan ontstaan als de gekozen database geen ingebouwde mechanismen heeft voor het veilig opslaan van gegevens, zoals hashing van wachtwoorden.<br/>

**Vereiste:** Schaalbaarheid om toekomstige groei en het aantal gebruikers te ondersteunen. <br/>
**Gap:** Een gap kan ontstaan als de gekozen database beperkingen heeft op het gebied van schaalbaarheid, zoals beperkte capaciteit of moeilijkheden bij het opschalen naar een groter aantal gebruikers.<br/>

**Vereiste:** Voor het semester waarin ik de applicatie ga ontwikkelen wordt er verwacht dat er een ORM gebruikt wordt. <br/>
**Gap:** Een gap kan ontstaan als de gekozen database geen ondersteuning biedt voor een ORM.<br/>

#### Domain modelling   
De database moet een aantal dingen kunnen bijhouden. De database moet:
- huishoudens en leden van huishoudens kunnen bijhouden en aan elkaar linken
- boodschappenlijsten kunnen bijhouden en aan huishoudens kunnen linken
- boodschappen kunnen bijhouden en aan boodschappenlijsten kunnen linken
- agenda-items kunnen bijhouden en aan huishoudens kunnen linken
- taken kunnen bijhouden en aan huishoudens kunnen linken
- notities per huishouden kunnen opslaan

## Conclusie
Om antwoord te geven op de hoofdvraag van dit onderzoek, voor de Housekeeper applicatie, is een SQL relationele database naar mijn mening de meest geschikte keuze op basis van de volgende redenen:

1. **Structuur**: Het relationele model is zeer geschikt voor het structureren van gegevens zoals boodschappenlijsten, agenda-items, notities, taken en gebruikersinformatie. Dit maakt het eenvoudig om relaties te leggen tussen verschillende entiteiten (zoals huishoudens, leden van huishoudens, boodschappenlijsten, enz.) en om complexe queries uit te voeren om relevante informatie te extraheren.

2. **Beveiliging**: SQL relationele databases bieden sterke beveiligingsfuncties, zoals de mogelijkheid om specifieke tabellen te beschermen met gebruikersnamen en wachtwoorden. Dit is erg belangrijk voor een toepassing als Housekeeper, die gevoelige gebruikersinformatie opslaat.

3. **Flexibiliteit**: Hoewel de NoSQL databases meer flexibiliteit bieden in termen van schaalbaarheid en verschillende gegevenstypes, wordt dit in de Housekeeper applicatie misschien niet volledig benut. De gegevensbehoeften van de Housekeeper applicatie zijn tamelijk gestructureerd en passen goed bij het relationele model.

4. **Schaalbaarheid**: Relationele databases kunnen schalen om een groot aantal gebruikers en transacties te ondersteunen. Bovendien zijn er veel technieken en technologieën beschikbaar om de prestaties en schaalbaarheid van SQL-databases te optimaliseren.

5. **Volwassenheid en ondersteuning**: SQL is een volwassen technologie met een sterke ondersteuning in termen van ontwikkeltools, bibliotheken, en een grote community van ontwikkelaars. Dit kan ontwikkeling en onderhoud eenvoudiger maken.

6. **ORM's**: dit semester is een ORM gebruiken vereist en NoSQL is niet geschikt voor ORM's.

Het is belangrijk op te merken dat dit niet betekent dat andere soorten databases niet geschikt kunnen zijn voor de Housekeeper applicatie. Afhankelijk van de specifieke behoeften en omstandigheden, kunnen objectgeoriënteerde databases of NoSQL databases ook voordelig zijn. Echter, op basis van de huidige eisen en behoeften van de applicatie, lijkt een SQL relationele database de beste keuze.
