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
- [4. Het groepsproject: Swipper](#4-het-groepsproject-swipper)
- [5. Het individuele project: Housekeeper](#5-het-individuele-project-housekeeper)
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

Geachte lezer, WELKOM! Welkom bij de grote ORM Showdown. Het onderzoeksrapport waar ORM's de grote hoofdprijs kunnen winnen; Gemplementeerd worden in mijn project. Woehoe! Laten we beginnen!

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

### 3.3 Ethiek

## 4. Het groepsproject (Swipper)

## 5. Het individuele project (Housekeeper)

## 6. Zelfreflectie

### 6.1 Wat heb ik geleerd

### 6.2 Wat ging er goed

### 6.3 Wat doe ik voortaan anders
