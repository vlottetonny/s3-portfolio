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
| **(3) Hoe passen de specifieke kenmerken van deze databasetypen bij de behoeften van de Housekeeper applicatie?** 	 | Gap analysis, Domain modelling, Prototyping     |

### Instrumenten

De volgende instrumenten worden gebruikt:

1. Housekeeper applicatie: Dit project zal als voorbeeld worden gebruikt om een geschikte database voor te selecteren.
2. Literatuur: Wetenschappelijke artikelen, boeken, en betrouwbare online bronnen zullen worden gebruikt om de verschillende databasetypen te onderzoeken.

### Beperkingen

Het onderzoek zal zich alleen richten op de Housekeeper applicatie en de bevindingen zijn mogelijk niet van toepassing op andere applicaties met andere eisen en behoeften.

## Resultaten

### 1. Wat zijn de specifieke behoeften van de Housekeeper applicatie op het gebied van databeheer?

#### Stakeholder Analysis

#### Explore User Requirements

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

#### Domain modelling   

#### Prototyping    

## Conclusie

