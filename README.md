# Software semester 3 portfolio
Teun Hurkmans, S3-DB01 van Fontys Eindhoven 

## Belangrijke linkjes
  ### Het groepsproject
  - [Git repository voor de frontend](https://github.com/einstein43/swipper_frontend)
  - [Git repository voor de backend](https://github.com/Exurbia404/SwipperASP)
  ### Het individuele project
  - [Git repository voor de frontend](https://github.com/vlottetonny/s3-individueel-Frontend)
  - [Git repository voor de backend](https://github.com/vlottetonny/s3-individueel-Backend)
  ### Portfolio
  - [Mijn portfolio](https://github.com/vlottetonny/s3-portfolio/tree/main) ← Je bent hier

---

## Table of contents
- [1. Introductie](#1-introductie)
- [2. Leeruitkomsten](#2-leeruitkomsten)
- [3. Onderzoeken](#3-onderzoeken)
  - [3.1 De Grote ORM Showdown](#31-de-grote-orm-showdown)
  - [3.2 Culturele verschillen](#32-culturele-verschillen)
  - [3.3 Security](#33-security)
  - [3.4 Agile methodes](#34-agile-methodes)
- [4. Het groepsproject: Swipper](#4-het-groepsproject-swipper)
- [5. Het individuele project: Housekeeper](#5-het-individuele-project-housekeeper)
  - [5.1 De aanpak](#51-de-aanpak)
  - [5.2 De stackkeuze](#52-de-stackkeuze)
  - [5.3 User stories](#54-user-stories)
  - [5.3 De uitvoering](#54-de-uitvoering)
  - [5.4 Gebruikers testen](#54-gebruikers-testen)
- [6. Zelfreflectie](#6-zelfreflectie)
  - [6.1 Wat heb ik geleerd](#61-wat-heb-ik-geleerd)
  - [6.2 Wat ging er goed](#62-wat-ging-er-goed)
  - [6.3 Wat doe ik voortaan anders](#63-wat-doe-ik-voortaan-anders)

## 1. Introductie

HEE HOI, Leuk dat je mijn software portfolio bezoekt! Op dit moment zit ik in mijn derde semester bij Fontys ICT & Software-engineering. Hier heb ik de nodige kennis en vaardigheden opgedaan, die ik graag met je deel via mijn recente werk. Denk hierbij aan onderzoeksrapporten, zowel individuele als groepsprojecten, en reflecties op mijn persoonlijke leerproces. Ik hoop dat je het interessant vindt om hier doorheen te bladeren. <br/>
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

### 3.1 Objext relational mappers
>Disclaimer: Dit is het eerste onderzoek wat ik schreef en is in principe waardeloos. Ik heb het toch toegevoegd voor de totaliteit en om de groei binnen dit semester aan te tonen. Dit onderzoek is niet beoordeeld voor de rubric met semester-voortgang.

>[ De grote ORM Showdown! ](https://github.com/vlottetonny/s3-portfolio/blob/main/Research/ORM's.md)

### 3.2 Culturele verschillen

>[ Culturele verschillen tussen Nederland en Finland in software engineering ](https://github.com/vlottetonny/s3-portfolio/blob/main/Research/CulturalDifferences.md)

### 3.3 Security

>[ OWASP Top 10 en JWT Tokens ](https://github.com/vlottetonny/s3-portfolio/blob/main/Research/Security.md)

### 3.4 Agile methodes

>[ Agile Project Management voor het Swipper Project ](https://github.com/vlottetonny/s3-portfolio/blob/main/Research/Agile.md)

## 4. Het groepsproject (Swipper)

Voor het groepsproject in semester drie heb ik samen met mijn groepsgenoten een app gemaakt voor het kopen en verkopen/ter adoptie aanbieden van huisdieren. <br/>

### 4.1 Business processen

Voor het groepsproject moesten we een aantal business processen uitwerken. Deze processen zijn te vinden in de map [Business Processes](

## 5. Het individuele project (Housekeeper)

Voor mijn individuele project in semester drie heb ik gekozen voor het maken van een app die kan dienen als een groepsplanner voor je huishouden. Het idee is dat je een groep/huishouden aanmaakt met je huisgenoten en dat je dan klusjes en dergelijke kunt toevoegen zodat je huisgenoten een idee hebben van wat er gebeuren moet. Deze taken kunnen dan door de groepsleden worden opgepakt. <br/>
Naast taken kunnen gebruikers ook een gezamenlijke boodschappenlijst bijhouden, een gezamenlijke kalender bijhouden en briefjes achterlaten voor hun huisgenoten <br/>

### 5.1 De aanpak
Voordat ik kon beginnen aan het maken van de app moest ik een aantal dingen uitzoeken. Zo bijvoorbeeld waar ik mijn voortgang en planning bij ging houden. Hier heb ik voor Trello gekozen. <br/>
Ik heb moeten nadenken over hoe ik de applicatie voor me zag. Hierbij heb ik me scenarios voorgesteld waarin ik persoonlijk de app zou gebruiken. Met deze scenarios in mijn achterhoofd heb de keuze voor een mobiele applicatie gemaakt. Voor het doel wat de app heeft leek het me onwaarschijnlijk dat ik er telkens voor naar een internet address zou willen surfen. <br/>
Hierna heb ik een aantal schetsen gemaakt van hoe ik de app voor me zag. Deze schetsen heb ik vervolgens in figma gezet. Toen dat af was ben ik gaan nadenken over mijn stackkeuze. <br/>

### 5.2 De stackkeuze

#### 5.2.1 Frontend
Voor mijn Frontend heb ik gekozen voor React-native in combinatie met Expo. Ik heb hiervoor gekozen omdat ik interesse had in het leren van React, maar omdat ik al was uitgekomen op een mobiele app leek het me een goed idee om React-native te leren. <br/>
Daar komt ook bij kijken dat ik me dit semester wilde focussen op het leren van Typescript. React-native is een framework waarmee ik dus twee vliegen in één klap kon slaan.  <br/>

#### 5.2.2 Backend
Voor mijn backend heb ik mijn keuze in eerste instantie laten lijden door het deze verlangen om Typescript te leren. Ik heb gekozen voor een nodejs project met Typescript en Express. Express heb ik erbij genomen, omdat dit in een fireship tutorial werd gebruikt die ik aan het volgen was. En het me goed beviel. Ook moest ik dit semester een ORM kiezen. Zoals [eerder in dit portfolio](#31-de-grote-orm-showdown) te lezen is, is mijn keuze gevallen op Prisma ORM. Waarom staat in het onderzoeksrapport.<br/>
De backend is een REST API die CI/CD heeft met behulp van Github Actions. De API is gehost op Microsoft Azure. <br/> 

#### 5.2.3 Database
Voor mijn database heb ik gekozen voor een SQL-database. Ik heb hiervoor gekozen omdat ik hier al ervaring mee had en van eerdere projecten, maar ook omdat we dit semester gebruik moeten maken van een ORM en dus een relational database een vereiste is. <br/>
Nu ik eenmaal zo'n ORM heb gebruikt ga ik nooit meer met de hand SQL queries schrijven... Hoop ik... <br/>
De Database is gehost op Microsoft Azure. 

### 5.3 User stories
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

### 5.4 De uitvoering

#### 5.3.1 Security
Ik heb mijn eigen login systeem voor de Housekeeper app gemaakt. Dit omdat ik al eerdr met Auth0 heb gewerkt en ik het leuk en nuttig vond om het zelf te maken. <br/>
De app hashed wachtwoorden tijdens het registreerproces. Deze worden vervolgens opgeslagen in de database. Zo blijven gebruikersgegevens veilig. <br/>
Voor de security van mijn app heb ik gebruik gemaakt van JWT-tokens. Deze tokens worden gegenereerd door de backend en worden vervolgens opgeslagen in de async storage van de app. 
Deze tokens worden gebruikt om de gebruiker te identificeren en om te bepalen of de gebruiker toegang heeft tot bepaalde endpoints. 
De tokens worden gegenereerd met een secret die alleen bekend is bij de backend. <br/>

#### 5.3.2 CI/CD
Ik heb CI/CD toegepast op mijn backend. Dit heb ik gedaan met behulp van Github Actions. 
Github actions runt alle tests uit de "__tests__" folder. Het test framework dat ik gebruik heet Jest. Het is de eerste keer dat ik hier mee werk, maar ik vind het erg intuïtief.<br/>
De CI/CD-pipeline zorgt ervoor dat de backend automatisch wordt getest en redeployed wanneer er een nieuwe commit wordt ge-pushed naar de master branch. De testen bestaan uit de zelfde stappen als die een gebruiker maakt wanneer hij bepaalde handelingen doet. Denk aan registreren, inloggen, boodschappenlijsten beheren etc. <br/>
De CI/CD-pipeline zorgt er ook voor dat de backend automatisch wordt redeployed wanneer er een nieuwe commit wordt ge-pushed naar de master branch. De backend wordt redeployed op Microsoft Azure. <br/>
Ook gebruik ik sonarcloud om de code quality van mijn backend te meten. Sonarcloud geeft mij inzicht in de code quality van mijn backend. Zodra er bugs in mijn project zitten die door sonarcloud worden gedetecteerd, ga ik deze direct fixen. <br/>

#### 5.3.3 
### 5.5 Gebruikers testen
Voor de Frontend van mijn app heb ik gebruikerstesten gedaan. Ik heb dit gedaan in de expo variant van mijn app. <br/>

#### 5.5.1 Test 1
**Doel:** Een gebruiker maakt een account aan. 

**Resultaat:** 
- Geslaagd: 2/2
- Foutloos: 0/2

**Feedback:** 
- Er ontbreekt een toetsenbord omlaag knop, de gebruiker kon niet direct de "doorgaan" knop vinden.
- De registreerknop werd over het hoofd gezien.

**Fixes:**
- De "Return" knop op het toetsenbord kan een "doorgaan" of "gereed" knop worden.
- De registreerknop kan een andere kleur krijgen zodat deze meer opvalt.


#### 5.5.2 Test 2
**Doel:** Een gebruiker maakt een household aan. 

**Resultaat:** 
- Geslaagd: 2/2
- Foutloos: 2/2

**Feedback:** n.v.t.

**Fixes:** n.v.t. 

#### 5.5.3 Test 3
**Doel:** Een gebruiker logt in.

**Resultaat:**
- Geslaagd: 2/2
- Foutloos: 2/2

**Feedback:** n.v.t.

**Fixes:** n.v.t.

#### 5.5.4 Test 4
**Doel:** Een gebruiker voegt een item toe aan de grocery list.

**Resultaat:**
- Geslaagd: 2/2
- Foutloos: 0/2

**Feedback:** 
- De tekst "Extra item information" was mogelijk te klein. De gebruiker twijfelde of het input veld verplicht was.
- De "+" knop was niet responsief genoeg, hij veroorzaakte twijfel bij de gebruiker over wat er zou gebeuren als er op geklikt werd.

**Fixes:**
- Het input veld kan iets worden ingekort of verkleint zodat het duidelijk is dat het een subtext is en dus eventueel kan worden weg gelaten.
- De "+" knop kan de border en achtergrond kleuren verwisselen wanneer er op geklikt is, om aan te geven dat de knop nu een andere functie heeft. Dit is duidelijker voor de gebruiker.

## 6. Zelfreflectie

### 6.1 Wat heb ik geleerd

### 6.2 Wat ging er goed

### 6.3 Wat doe ik voortaan anders
