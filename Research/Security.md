# OWASP Top 10 en JWT Tokens

## Inhoudsopgave

  - [Inhoudsopgave](#inhoudsopgave)
  - [Inleiding](#inleiding)
  - [Methodologie](#methodologie)
  - [Onderzoeksstrategieën](#onderzoeksstrategieën)
  - [Instrumenten](#instrumenten)
  - [Beperkingen](#beperkingen)
  - [Resultaten](#resultaten)
  - [Bronnen](#bronnen)

Hier zijn een paar voorbeelden van hoe JWT-tokens (een soort 'sleutel' die we gebruiken om gebruikers te herkennen) kunnen bijdragen aan deze risico's als ze niet op de juiste manier worden gebruikt:
**Injection (A1)**: Dit is als iemand slechte data 'injecteert' in jouw systeem, zoals een valse gebruikersnaam. Hoewel dit meestal niet gebeurt met JWT-tokens, kan het wel gebeuren als we niet voorzichtig zijn met hoe we die tokens behandelen.

**Broken Authentication (A2)**: JWT-tokens helpen ons om te bevestigen wie een gebruiker is. Maar als we niet veilig met die tokens omgaan (bijvoorbeeld door ze te verzenden over een verbinding die niet beveiligd is), dan kunnen slechteriken ofzo die tokens misschien stelen en zich voordoen als iemand anders.

**Sensitive Data Exposure (A3)**: Soms kunnen JWT-tokens informatie bevatten die privé moet blijven. Als we die tokens niet goed beveiligen (zoals door ze niet te versleutelen), dan kunnen die privégegevens op straat komen te liggen.

**Broken Access Control (A5):** Als we niet goed controleren of een JWT-token geldig is, dan kan een slechterik misschien een vals of gestolen token gebruiken om toegang te krijgen tot dingen waar hij geen toegang tot zou moeten hebben.

**Using Components with Known Vulnerabilities (A9)**: Als we oude of onveilige software gebruiken om JWT-tokens te maken of te controleren, dan kunnen slechteriken die zwakke plekken misschien misbruiken om dingen te doen die ze niet mogen.


## Inleiding

De Open Web Application Security Project (OWASP) Top 10 is een standaard beveiligingsbenchmark voor webapplicaties. Een van de meest voorkomende beveiligingsrisico's in deze benchmark is de onveilige behandeling van JWT (JSON Web Tokens) bij authenticatieprocedures. In dit onderzoek zal de focus liggen op JWT's in het login systeem van mijn React Native-app, HouseKeeper.

Het onderwerp van dit onderzoek kwam aan bod door uitdagingen binnen mijn HouseKeeper-project. Tijdens het opzetten van het authenticatiesysteem, kwamen er diverse beveiligingsvragen naar voren. Aangezien dit een essentieel onderdeel is van de applicatie, en ook omdat het verplicht is dit semester, is besloten dat dit een goed onderzoeksthema zou zijn.

## Methodologie

In dit onderzoek zal een gekeken worden naar JWT-tokens en de OWASP Top 10. De belangrijkste onderzoeksvraag die beantwoord zal worden is:

>Hoe kunnen ontwikkelaars veilig JWT-tokens implementeren in hun webapplicatie?

Om deze vraag te helpen beantwoorden, is deze opgesplitst in meerdere subvragen:

1. Wat zijn JWT-tokens?
2. Wat zijn de beveiligingsrisico's van het onveilig omgaan met JWT-tokens?
3. Hoe kunnen ontwikkelaars JWT-tokens veilig implementeren? 

### Onderzoeksstrategieën
Het onderzoek zal worden uitgevoerd met behulp van het DOT (Development Oriented Triangulation) framework. Voor de vragen worden de volgende onderzoeksstrategieën gebruikt:

| Onderzoeksvraag                                                                   |	Onderzoeksstrategie |
|-----------------------------------------------------------------------------------| --- |
| **(1)** Wat zijn JWT-tokens?	                                                     | Internet-onderzoek |
| **(2)** Wat hebben JWT-tokens te maken met de OWASP Top 10?	                      | Internet-onderzoek |
| **(3)** Wat zijn de beveiligingsrisico's van het onveilig omgaan met JWT-tokens?	 | Internet-onderzoek |
| **(4)** Hoe kunnen website-ontwikkelaars JWT-tokens veilig implementeren?         |	Internet-onderzoek en praktijktesten |

### Instrumenten
Instrumenten worden gebruikt om het onderzoek te beheren en uit te voeren. In dit onderzoek worden de volgende instrumenten gebruikt:

HouseKeeper applicatie

Deze applicatie zal worden gebruikt als voorbeeldproject waarin JWT-tokens worden gebruikt.

### Beperkingen
De enige beperking van dit onderzoek is dat het zich zal beperken tot het type applicatie, in dit geval: React Native-applicaties. Dit betekent dat het onderzoek mogelijk niet voor iedereen even nuttig is, aangezien de methoden voor het omgaan met JWT-tokens kunnen verschillen tussen applicatietypes.

## Resultaten

### Wat zijn JWT-tokens?<br/>
JWT staat voor JSON Web Token en is een compacte, URL-veilige manier om informatie te coderen en over te dragen tussen twee partijen. De informatie wordt gecodeerd als een JSON-object, dat vervolgens wordt gecomprimeerd in een compacte token. JWT's worden veel gebruikt voor authenticatie en informatie-uitwisseling in webapplicaties.

### Wat hebben JWT-tokens te maken met de OWASP Top 10?<br/>
OWASP Top 10 is een lijst van de meest voorkomende veiligheidsrisico's op het web. Hier zijn een paar voorbeelden van hoe JWT-tokens (een soort 'sleutel' die we gebruiken om gebruikers te herkennen) kunnen bijdragen aan deze risico's als ze niet op de juiste manier worden gebruikt:<br/>
**Injection (A1)**: Dit is als iemand slechte data 'injecteert' in jouw systeem, zoals een valse gebruikersnaam. Hoewel dit meestal niet gebeurt met JWT-tokens, kan het wel gebeuren als we niet voorzichtig zijn met hoe we die tokens behandelen. <br/>
**Broken Authentication (A2)**: JWT-tokens helpen ons om te bevestigen wie een gebruiker is. Maar als we niet veilig met die tokens omgaan (bijvoorbeeld door ze te verzenden over een verbinding die niet beveiligd is), dan kunnen slechteriken of zo die tokens misschien stelen en zich voordoen als iemand anders.<br/>
**Sensitive Data Exposure (A3)**: Soms kunnen JWT-tokens informatie bevatten die privé moet blijven. Als we die tokens niet goed beveiligen (zoals door ze niet te versleutelen), dan kunnen die privégegevens op straat komen te liggen.<br/>
**Broken Access Control (A5):** Als we niet goed controleren of een JWT-token geldig is, dan kan een slechterik misschien een vals of gestolen token gebruiken om toegang te krijgen tot dingen waar hij geen toegang tot zou moeten hebben.<br/>
**Using Components with Known Vulnerabilities (A9)**: Als we oude of onveilige software gebruiken om JWT-tokens te maken of te controleren, dan kunnen slechteriken die zwakke plekken misschien misbruiken om dingen te doen die ze niet mogen.

### Wat zijn de beveiligingsrisico's van het onveilig omgaan met JWT-tokens?<br/>
Onveilig gebruik van JWT-tokens kan leiden tot een aantal ernstige beveiligingsproblemen, waaronder:<br/>
**Tokenontvreemding:** Als een aanvaller een JWT-token kan stelen, kan hij zich voordoen als de gebruiker die door het token wordt gerepresenteerd. Dit kan leiden tot verboden toegang tot de applicatie en mogelijk tot het lekken van gebruikersgegevens.<br/>
**Slechte tokenbeveiliging:** Als een JWT-token niet goed is beveiligd, kan een aanvaller mogelijk de inhoud ervan lezen of manipuleren. Dit kan leiden tot ongeoorloofde toegang tot de applicatie en het lekken van gevoelige gebruikersgegevens.<br/>
**Slecht tokenbeheer:** Als een applicatie geen goede strategieën heeft voor het uitgeven, vernieuwen en intrekken van tokens, kan dit leiden tot tokens die te lang geldig zijn, wat het risico op tokenontvreemding vergroot.<br/>

### Hoe kunnen website-ontwikkelaars JWT-tokens veilig implementeren?
Ontwikkelaars kunnen een aantal maatregelen nemen om JWT-tokens veilig te implementeren in hun applicaties, waaronder:<br/>
Gebruik HTTPS: Het gebruik van HTTPS helpt bij het beschermen van de overdracht van JWT-tokens tussen de server en de client, waardoor het risico op tokenontvreemding wordt verminderd.
Beveilig tokens: Het is essentieel om JWT-tokens te beveiligen, zowel in rust als tijdens transport. Dit kan onder andere worden bereikt door het gebruik van veilige cookies voor het opslaan van tokens aan de clientzijde.
Beperk de levensduur van tokens: Het beperken van de levensduur van tokens helpt het risico op tokenontvreemding te verminderen. Dit kan worden bereikt door gebruik te maken van korte levensduren en door het gebruik van refresh tokens.
Valideer tokens: Het is essentieel om JWT-tokens aan de serverzijde te valideren om ervoor te zorgen dat ze afkomstig zijn van een vertrouwde bron.

Dit is een voorbeeld van hoe ik de JWT-tokens in mijn applicatie heb geïmplementeerd:

```javascript
    const payload = await UserRepository.loginUser(user);
    let success: boolean;
    success = payload !== null;
    const userId = payload?.id || null;
    const authToken = jwt.sign(payload, process.env.JWT_SECRET);
```

## Conclusie
JWT-tokens in je React Native-app zijn super belangrijk voor de veiligheid wanneer je je eigen login systeem maakt. Zonder de juiste stappen, kunnen ze echt problemen veroorzaken. Gelukkig kunnen we dat fixen door slimme beveiligingsstappen te volgen.

## Bronnen
https://owasp.org/www-project-top-ten/ <br/>
https://jwt.io/ <br/>
https://www.youtube.com/watch?v=7Q17ubqLfaM <br/>
https://auth0.com/blog/a-look-at-the-latest-draft-for-jwt-bcp/ <br/>
