# Software semester 3 portfolio
Teun Hurkmans, S3-DB01 van Fontys Eindhoven 

## Belangrijke linkjes
  ### Het groepsproject
  - [Git repository voor de frontend](toevoegen)
  - [Git repository voor de backend](toevoegen)
  ### Het individueele project
  - [Git repository voor de frontend](https://github.com/vlottetonny/s3-individueel-Frontend)
  - [Git repository voor de backend](https://github.com/vlottetonny/s3-individueel-Backend)
  ### Portfolio
  - [Mijn portfolio](https://github.com/vlottetonny/s3-portfolio/tree/main)     <- Je bent hier

---

## Table of contents
- [1. Introductie](#1-introductie)
- [2. Leeruitkomsten](#2-leeruitkomsten)
- [3. Onderzoeken](#3-onderzoeken)
  - [3.1 De Grote ORM Showdown](#31-de-grote-orm-showdown)
  - [3.2 Culturele verschillen](#32-culturele-verschillen)
  - [3.3 Ethiek](#33-ethiek)
  - [3.4 Veiligheid in webdevelopment](#34-veiligheid-in-webdevelopment)
- [4. Het groepsproject: Swipper](#4-het-groepsproject-swipper)
- [5. Het individuele project: Housekeeper](#5-het-individuele-project-housekeeper)
  - [5.1 De aanpak](#51-de-aanpak)
  - [5.2 De stackkeuze](#52-de-stackkeuze)
  - [5.3 De uitvoering](#53-de-uitvoering)
  - [5.4 Gebruikers testen](#54-gebruikers-testen)
- [6. Zelfreflectie](#6-zelfreflectie)
  - [6.1 Wat heb ik geleerd](#61-wat-heb-ik-geleerd)
  - [6.2 Wat ging er goed](#62-wat-ging-er-goed)
  - [6.3 Wat doe ik voortaan anders](#63-wat-doe-ik-voortaan-anders)

## 1. Introductie

HEY HOI, Leuk dat je mijn software portfolio bezoekt! Op dit moment zit ik in mijn derde semester bij Fontys ICT & Software Engineering. Hier heb ik de nodige kennis en vaardigheden opgedaan, die ik graag met je deel via mijn recente werk. Denk hierbij aan onderzoeksrapporten, zowel individuele als groepsprojecten, en reflecties op mijn persoonlijke leerproces. Ik hoop dat je het interessant vindt om hier doorheen te bladeren. <br/>
Verder ook alvast een kleine shout-out naar mijn docenten Samuil Angelov en Jean Paul Ligthart, mogen jullie het een voldoende waard vinden.

## 2. Leeruitkomsten

| # | Naam | Korte beschrijving | Verduidelijking |
|---|------|-------------------|---------------|
| 1 | Webapplicatie | Je ontwerpt en bouwt gebruiksvriendelijke, full-stack webapplicaties. | **Gebruiksvriendelijk:** Je past basisgebruikerstests en -ontwikkelingstechnieken toe. <br> **Full-stack:** Je ontwerpt en bouwt een full-stack applicatie met behulp van veelgebruikte front-end (JavaScript-gebaseerde frameworks) en back-end technieken (bijv. Object Relational Mapping), kiest en implementeert relevante communicatieprotocollen en behandelt asynchrone communicatieproblemen. |
| 2 | Softwarekwaliteit | Je gebruikt software **tooling en methodologie** die de softwarekwaliteit tijdens softwareontwikkeling continu bewaakt en verbetert. | **Tooling en methodologie:** Voer unit-, integratie-, regressie- en systeemtests uit, met aandacht voor beveiligings- en prestatieaspecten, en pas statische code-analyse en code reviews toe. |
| 3 | Agile methode | Je **kiest** en implementeert de meest geschikte agile softwareontwikkelingsmethode voor je softwareproject. | **Kies:** Je bent op de hoogte van de meest populaire agile methoden en hun onderliggende agile principes. Je keuze van een methode is gemotiveerd en gebaseerd op goed gedefinieerde selectiecriteria en contextanalyses. |
| 4 | CI/CD | Je **implementeert** een (semi)geautomatiseerd software release proces dat past bij de behoeften van de projectcontext. | **Implementeren:** Je implementeert een continue integratie en implementatie-oplossing (bijv. Gitlab CI en Docker). |
| 5 | Culturele verschillen en ethiek | Je **herkent** en **houdt rekening met** culturele verschillen tussen project belanghebbenden en ethische aspecten in softwareontwikkeling. | **Herkennen:** Erkenning is gebaseerd op theoretisch onderbouwd bewustzijn van culturele verschillen en ethische aspecten in software engineering. <br> **Rekening houden met:** Pas uw communicatiestijlen, werkstijlen en gedrag aan om projectbelanghebbenden uit verschillende culturen weer te geven. Adres een van de standaard programmeer ethische richtlijnen (bijv. ACM Code of Ethics and Professional Conduct) in uw werk. |
| 6 | Requirements en Design | Je analyseert (niet-functionele) eisen, uitgebreide (architectonische) ontwerpen en valideert deze met behulp van **meerdere soorten testtechnieken**. | **Meerdere soorten testtechnieken:** Je past gebruikerstests en feedback van belanghebbenden toe om de kwaliteit van de eisen te valideren. U evalueert de kwaliteit van het ontwerp (bijvoorbeeld door testen of prototyping) rekening houdend met de geformuleerde kwaliteitseigenschappen zoals beveiliging en prestaties. |
| 7 | Bedrijfsprocessen | Je analyseert en beschrijft **eenvoudige** bedrijfsprocessen die **gerelateerd** zijn aan je project. | **Eenvoudige:** Het betreft belanghebbenden, overwegend sequentiële processen met één of twee alternatieve paden.<br>**Gerelateerd:** Bedrijfsprocessen tijdens welke de software die je ontwikkelt zal worden gebruikt (bedrijfsprocessen die de software moeten ondersteunen door deze volledig of gedeeltelijk te automatiseren).<br>**of**<br>Bedrijfsprocessen die nodig zijn voor het succes van je softwareontwikkelingsproject (bijv. productrelease, marktrelease, financiële verzekering). |
| 8 | Professionaliteit | Je handelt op een **professionele manier** tijdens softwareontwikkeling en leren. | **Professionele manier:** Je ontwikkelt software als een teaminspanning volgens een voorgeschreven softwaremethodologie en volgt teamafspraken. Je kunt je werkvoortgang bijhouden en communiceren met het team.<br>Je vraagt actief om feedback van belanghebbenden en past deze toe bij het adviseren van de meest optimale technische en ontwerp (architectonische) oplossingen. Je kiest en onderbouwt oplossingen voor een gegeven probleem. |

Kleine disclaimer, dit is vertaald door chatGPT. 

## 3. Onderzoeken

### 3.1 De Grote ORM Showdown

Geachte lezer, deze disclaimer schrijf ik om je even voor te bereiden op het onderzoek rapport dat je zo gaat lezen. Ik had namelijk een schandalige portie geen zin om hier aan te beginnen, dus ik heb het maar een beetje opgeleukt. Ik hoop dat je het leuk vindt, en anders heb je pech. 

WELKOM! Welkom bij de grote ORM Showdown. Het onderzoeksrapport waar ORM's de grote hoofdprijs kunnen winnen; Gemplementeerd worden in mijn project. Woehoe! Laten we beginnen!

Eventjes het zakelijke, ik schrijf dit onderzoeksrapport met twee redenen. Ten eerste ben ik vanuit mijn studie verplicht om een aantal van deze onderzoeken uit te voeren. Maar er is een tweede, en misschien wel belangrijkere, reden: ik heb geen duidelijk beeld van wat een ORM is. Hoewel ik weet waar de afkorting voor staat (Object Relational Mapping framework), kan ik niet precies uitleggen wat het doet. Maar dat gaat veranderen, want ik ga het nu voor jullie uitzoeken.

Dus wat is een ORM? Ik ben het internet, en dan met name Wikipedia af gegaan en dit is hoe ik het begrijp. Stel je voor dat je baas op je werk zegt je een tekening moet gaan maken, maar als de ware kleurplaat fanaat die je bent schiet je gelijk in de stress. Je hebt geen eens een potlood vriend, alleen je Stabilo stiften set. Dus daar zit je dan, met een blanco vel papier voor je en zou je elk detail zelf moeten tekenen en inkleuren om het eindresultaat te krijgen. Maar wat als iemand je al een prachtige tekening aanbiedt, waar de lijnen al zijn getrokken en de vlakken al zijn verdeeld? Dan hoef je alleen maar de kleuren in te vullen en voilà, je hebt een geweldige tekening gemaakt! Dat is wat een ORM doet, maar dan met databases en objecten. Het vertaalt de data in de database naar objecten die je kunt gebruiken in je code, zonder dat je zelf SQL-query's hoeft te schrijven. Pittig ziek als je het mij vraagt.

Oke, nu dat duidelijk is, moet ik het gaan toepassen op mijn eigen project. Voordat ik ga bepalen welke ORM het beste bij mijn project past, wil ik eerst wat informatie delen over mijn project. Ik ben bezig met het maken van een react native app voor mijn individuele project en ik gebruik daarvoor een backend API. Deze API is geschreven in TypeScript en maakt gebruik van het ExpressJS-framework. De database die ik gebruik is een SQL Server-database die ik host op Azure. Het is dus belangrijk om te kijken welke ORM's geschikt zijn voor deze combinatie van API en database.

En dan nu voor de contenders. Dit zijn de beste opties die ik op het internet heb gevonden: <br>
**TypeORM** - Dit is een bekend ORM-framework dat goed werkt met TypeScript en ExpressJS. Het is super gebruiksvriendelijk en ondersteunt verschillende databases, waaronder SQL Server. <br/>
**Sequelize** - Dit is een sterk ORM-framework dat ondersteuning biedt voor TypeScript en verschillende databases, zoals SQL Server. Het heeft ook geavanceerde functies voor het beheren van de relaties tussen tabellen. <br/>
**Prisma** - Dit is een modern ORM-framework dat werkt met TypeScript en ExpressJS. Het heeft een intuïtieve API en maakt typeveilige code aan op basis van jouw database schema. <br/>

Mijn keuze is nu gevallen op Prisma, van harte gefelictiteerd. Dit voornamelijk omdat het lekker makkelijk lijkt te werken. Hun API is heel logisch en simpel te begrijpen, dus het schrijven van queries en het werken met de database is een makkie. Het helpt ook dat ze typesafety hebben, zodat ik fouten kan opsporen voor ik de code run. <br/>
Verder biedt Prisma goede ondersteuning voor zowel TypeScript als SQL-databases, waardoor het goed past bij de technologieën die je voor jouw project hebt gekozen. En hoewel de andere twee ORM's ook goed presteren in deze categorieën, kan Prisma met de ingebouwde codegenerator nog sneller en eenvoudiger te implementeren zijn. <br/>
Prisma werkt dus ook goed met de Typescript en SQL server combinatie. Hoewel de andere twee ORM's ook goed presteren in deze categorieën, is Prisma nóg beter vanwege de ingebouwde codegenerator. Hierdoor kan ik nog sneller en makkelijker aan de slag met het implementeren van mijn database als met de andere twee ORM's. Terwijl TypeORM soms omslachtige syntax kan hebben bij het schrijven van complexere queries, kan Sequelize minder veilig zijn door het ontbreken van typesafety. Gelukkig biedt Prisma al deze voordelen zonder de bijbehorende nadelen!

Ik denk dat ik me zo voldoende heb geinformeerd op het gebied van orm's en voel me comfortabel met mijn keuze. Ik wil de ORM's bedanken voor hun deelname aan De Grote ORM Showdown. Ik wil jou bedanken voor het lezen, dan ga ik nu werk maken van het implementeren van onze winnaar. 

### 3.2 Culturele verschillen

Voor iedere software engineer is het belangrijk om culturele verschillen te begrijpen. Dit is omdat je vaak samenwerkt met mensen uit andere landen en culturen. Het is belangrijk om te weten hoe je met deze mensen moet omgaan, zodat je een goede samenwerking kunt hebben. In dit onderzoek zal ik kijken naar de culturele verschillen tussen Nederland en Finland. Finland omdat het groepsproject in samenwerking met de Finse Oulu Universiteit was. 

** Wat is cultuur? ** <br/>
Cultuur is een verzameling van normen en waarden die een groep mensen met elkaar delen. Deze normen en waarden bepalen hoe mensen zich gedragen en hoe ze met elkaar omgaan. Cultuur is dus een belangrijk onderdeel van het leven van mensen. Het bepaalt hoe ze zich gedragen en hoe ze met elkaar omgaan.

** Wat zijn de culturele verschillen tussen Nederland en Finland? ** <br/>
Er zijn veel culturele verschillen tussen Nederland en Finland. Op basis van de samenwerking met de Oulu-studenten en de ervaring die ik heb opgedaan van de reis naar Finland aan de start van het project zet ik hier de belangrijkste verschillen op een rij: <br/>
- Nederlanders zijn directer dan Finnen. Nederlanders zeggen wat ze denken en voelen. Finnen zijn meer terughoudend en zeggen niet altijd wat ze denken en voelen. <br/>
- Nederlanders zijn meer individualistisch dan Finnen. Nederlanders zijn meer gericht op hun eigen leven en hun eigen doelen. Finnen zijn meer gericht op het grotere geheel en de gemeenschap.<br/>
- Nederlanders zijn meer open dan Finnen. Nederlanders zijn meer open over hun gevoelens en emoties. Finnen zijn meer gesloten over hun gevoelens en emoties. <br/>

** Wat zijn de gevolgen van deze culturele verschillen? ** <br/>
Deze culturele verschillen kunnen leiden tot misverstanden en conflicten. Als je niet weet hoe je met deze verschillen moet omgaan, kan dit leiden tot misverstanden en conflicten. Het is dus belangrijk om te weten hoe je met deze verschillen moet omgaan. <br/>
Bijvoorbeeld het minder direct zijn van finnen kan er voor zorgen dat ze niet altijd voor hun eigen visie opkomen tijdens het plannen van de appstructuur en dergelijke. Waar je voor uit moet kijken is dat je niet een plan trekt waar een gedeelte van je projectgroep het niet mee eens is. Dan zul je geen optimaal resultaat behalen. <br/>
Ook zou het natuurlijk kunnen dat bepaalde dingen waar wij van uit gaan voor hun helemaal niet vanzelfsprekend zijn of andersom, daarom is het belangrijk dat alle plannen duidelijk met elkaar besproken worden. <br/>

** Andere culturele verschillen om rekening mee te houden ** <br/>
Op een ietwat ander niveau zijn en praktische verschillen waar je rekening mee moet houden. Zo is het in Finland bijvoorbeeld een uur later dan in Nederland. Dit kan er voor zorgen dat je niet altijd op hetzelfde moment kunt overleggen. <br/>
Ook is het zo dat de Finse studenten een andere taal spreken dan wij. Dit kan er voor zorgen dat je niet altijd alles goed begrijpt. Uiteraard overleggen we in het Engels, maar het is niet onvoorstelbaar dat er ooit details verloren raken in de vertaling. <br/>

** Hoe ga ik om met deze culturele verschillen? ** <br/>
Zoals in de alinea's hierboven eigenlijk al beschreven staat is het belangrijkste dat we alles gewoon een tikje extra duidelijk met elkaar bespreken. <br/> Communicatie is key. <br/>

### 3.3 Ethiek

### 3.4 Veiligheid in webdevelopment
Voor het maken van een maken van mijn applicatie is het belangrijk om 


## 4. Het groepsproject (Swipper)

## 5. Het individuele project (Housekeeper)

Voor mijn individuele project in semester drie heb ik gekozen voor het maken van een app die kan dienen als een groepsplanner voor je huishouden. Het idee is dat je een groep/huishouden aanmaakt met je huisgenoten en dat je dan klusjes en dergelijke kunt toevoegen zodat je huisgenoten een idee hebben van wat er gebeuren moet. Deze taken kunnen dan door de groepsleden worden opgepakt. <br/>
Naast taken kunnen gebruikers ook een gezamelijke boodschappenlijst bijhouden, een gezamelijke kalender bijhouden en briefjes achterlaten voor hun huisgenoten <br/>

### 5.1 De aanpak
Voordat ik kon beginnen aan het maken van de app moest ik een aantal dingen uitzoeken. Zo bijvoorveeld waar ik mijn voortgang en planning bij ging houden. Hier heb ik voor Trello gekozen. <br/>
Ik heb moeten nadenken over hoe ik de applicatie voor me zag. Hierbij heb ik me scenarios voorgesteld waarin ik persoonlijk de app zou gebruiken. Met deze scenarios in mijn achterhoofd heb de keuze voor een mobiele applicatie gemaakt. Voor het doel wat de app heeft leek het me onwaarschijnlijk dat ik er telkens voor naar een internet adress zou willen surfen. <br/>
Hierna heb ik een aantal schetsen gemaakt van hoe ik de app voor me zag. Deze schetsen heb ik vervolgens in figma gezet. Toen dat af was ben ik gaan nadenken over mijn stackkeuze. <br/>

### 5.2 De stackkeuze

#### 5.2.1 Frontend
Voor mijn Frontend heb ik gekozen voor React-native in combinatie met Expo. Ik heb hiervoor gekozen omdat ik interesse had in het leren van React, maar omdat ik al was uitgekomen op een mobiele app leek het me een goed idee om React-native te leren. <br/>
Daar komt ook bij kijken dat ik me dit semester wilde focussen op het leren van Typescript. React-native is een framework waarmee ik dus twee vliegen in één klap kon slaan.  <br/>

#### 5.2.2 Backend
Voor mijn backend heb ik mijn keuze in eerste instantie laten lijden door het eerder genoemde verlangen om Typescript te leren. Ik heb gekozen voor een nodejs project met Typescript en Express. Express heb ik erbij genomen, omdat dit in een fireship tutorial werd gebruikt die ik aan het volgen was. En het me goed beviel. Ook moest ik dit semester een ORM kiezen. Zoals [eerder in dit portfolio](#31-de-grote-orm-showdown) te lezen is, is mijn keuze gevallen op Prisma ORM. Waarom staat in het onderzoeksrapport.<br/>
De backend is een REST API die CI/CD heeft met behulp van Github Actions. De API is gehost op Microsoft Azure. <br/> 

#### 5.2.3 Database
Voor mijn database heb ik gekozen voor een SQL database. Ik heb hiervoor gekozen omdat ik hier al ervaring mee had en van eerdere projecten, maar ook omdat we dit semester gebruik moeten maken van een ORM en dus een relational database een vereiste is. <br/>
Nu ik eenmaal zo'n ORM heb gebruikt ga ik nooit meer met de hand SQL queries schrijven... Hoop ik... <br/>
De Database is gehost op Microsoft Azure. 

### 5.3 De uitvoering

### User stories
**Als een user wil ik een "Household" kunnen aanmaken zodat ik een groep kan maken met mijn huisgenoten.** <br/>
Benodigd voor deze user story: <br/>
- Een frontend pagina waar een user een account aan kan maken. <br/>
- Een backend endpoint om een user aan te maken. <br/>
- Een frontend pagina waar een user een household aan kan maken. <br/>
- Een backend endpoint om een household aan te maken. <br/>
- Een frontend pagina waar een user een household kan joinen. <br/>
- Een backend endpoint om een user aan een household toe te voegen. <br/>

**Als een user wil ik een gezamenlijke grocery list bij kunnen houden.** <br/>
Benodigd voor deze user story: 
- Een frontend pagina waar de user een grocery list te zien krijgt. <br/>
- Een frontend venster waar de user een item kan toevoegen aan de grocery list kan toevoegen. <br/>
- Een backend endpoint om een item aan de grocery list toe te voegen. <br/>
- Een frontend knop waar de user een item kan markeren "als in het mandje". <br/>
- Een frontend knop waar de user de grocery list kan markeren als gekocht. <br/>
- Een backend endpoint om de grocery list te markeren als gekocht. <br/>

**Als een user wil ik een lijst kunnen zien van eerdere grocery lists van mijn huishouden.** <br/>
Benodigd voor deze user story: <br/>
- Een frontend pagina waar de user een lijst van eerdere grocery lists te zien krijgt. <br/>
- Een backend endpoint om een lijst van eerdere grocery lists op te halen. <br/>

**Als een user wil ik een gezamenlijke kalender bij kunnen houden.** <br/>
Benodigd voor deze user story: <br/>
- Een frontend pagina waar de user een kalender te zien krijgt. <br/>
- Een backend endpoint om kalender events op te halen.<br/>
- Een frontend venster om kalender events aan te maken. <br/>
- Een backend endpoint om kalender events aan te maken. <br/>

**Als een user wil ik een gezamenlijke todo list bij kunnen houden.** <br/>
Benodigd voor deze user story: <br/>
- Een frontend pagina waar de user een todo list te zien krijgt. <br/>
- Een backend endpoint om todo items op te halen. <br/>
- Een frontend venster om todo items aan te maken. <br/>
- Een backend endpoint om todo items aan te maken. <br/>
- Een frontend knop om todo items te markeren als gedaan. <br/>
- Een backend endpoint om todo items te markeren als gedaan. <br/>

**Als een user wil ik een gezamenlijke notitie lijst bij kunnen houden.**<br/>
Benodigd voor deze user story: <br/>
- Een frontend pagina waar de user een notitie lijst te zien krijgt. <br/>
- Een backend endpoint om notitie items op te halen. <br/>
- Een frontend venster om notitie items aan te maken. <br/>
- Een backend endpoint om notitie items aan te maken. <br/>

### hier moet de rest komen

### 5.4 Gebruikers testen

## 6. Zelfreflectie

### 6.1 Wat heb ik geleerd

### 6.2 Wat ging er goed

### 6.3 Wat doe ik voortaan anders
