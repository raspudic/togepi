# Gruppmöte 6/5

## Handledning med Jan-Philippe

- Funderingar kring ledighet/röda dagar - vanligtvis tas detta till hänsyn till vid sprint planning
- Lättare att ändra velocity efter detta än att försöka anpassa effort på tasks efter samma velocity på samma dagar (hellre ändra till typ 60 i velocity vid röd dag än att anpassa tasks)
- Blir klar med stories i förtid - bättre att avsluta sprint tidigare (om alla är klara) eller fråga andra om de behöver någon hjälp med sina stories
  - Annars kan man plocka fram nya stories från backlogen, men detta är lite risky för att backlogen kan ändras vid sprint planning
  - “Pool” av tasks - var försiktig med detta, eftersom det som är i sprintbacklogen ska levereras denna sprint. Lägger man user stories i sprintbacklogen ska de generellt levereras denna sprint. Isf bättre ha några estimerade kvar i produktbacklogen som kan tas in vid behov
- OK att ha “Som utvecklare vill jag…” som story, även om det är diskuterat om man ska ha detta eller inte
- Planeringen bör göras så man verkligen tror man hinner med allt - om man inte hinner så kan man dela upp user storyn i det som är klart → done och det som inte är klart → backlog
- Gränssnitt mellan user stories - är det en klar story om ex denna gång “Betala”-knappen inte fungerar? Hur hanteras det som ligger mellan user stories?
  - Som produktägare vill man minst se en alert eller liknande på demo-versionen vid en sprint review
  - Hellre en popup än skriva ut i terminal - ska vara synligt i användargränssnittet att något händer
  - Detta bör synas i Acceptance criterias
  - I detta fall - var user story rätt? Om betal-knappen egentligen inte ingick? När det finns en betal-knapp väcker det förväntningar i vad som har levererats, tråkigt när det inte ger någon feedback
- Viktigt att det som görs syns, så att produktägaren kan se att något händer - man vill ha något som är fullständigt i funktionaliteten
- Slutrapport - sammanfattande över alla gruppreflektioner som har gjorts
  - Är dessa bra sedan innan blir det mycket klippa och klistra

## Sprint Review

- Cart ska göras om lite
  - Kaffe-objekt ska ha en boolean på om det är egen mugg (true) eller lånad (false)
- Gruppen går igenom pull requests, Börjar med login
  - Some checks were not successful: Markus försöker fixa detta.
  - Vill ändra lite på flödet var login-sidan läggs. Emil upplever att den inte bör ligga direkt, utan vara en opt-in snarare än ett måste. Detta instämmer majoriteten av gruppen med. Man ska få tillgång till appen utan att ge den massa information. Eventuellt flyttas login-sidan till profilsidan vid tabsen.
- Vi diskuterar newCartField. Den uppfyller acceptance criteria.
- Vi diskuterar app/api som inte uppfyller kraven.
  - Den använder inte backenden utan använder fortfarande dummydata. Många i gruppen upplevde att det var många filer som ändrades, (24 st) men 14 st är filer som flyttats till backend och ca 4 st är omdöpningar av funktioner och variabelnamn. Vi avvaktar att mergea in den och ger Lucas och Robert mer tid på den.
- Vi diskuterar pull requesten med own-mug option.
  - Den är inte uppdaterad till dev som ändrades under veckan. Nu diskuteras det hur man kanske ska mergea sin branch till senaste dev medan man arbetar.
- Pull request: när ska dessa gås igenom och hur?
  - Just nu kan vi inte leverera dev vid sprint review - detta måste ändras
  - Ny taktik: gör en pull request tidigt och gör commits till denna, då är det mycket tydligare vad alla jobbar med. Alltså. Välj en user-story, skapa en branch, sätt upp en pull request om vad den ska innehålla och håll den uppdaterad.
- Produktägaren ska kolla Pull request och godkänna designen av dessa och funktioner
  - Ska vara klart när vi ses på måndag eftermiddag
- Koden i Pull requests ska kollas igenom avseende både logik och formatering
  - Detta ska få mer tid och utrymme än det har fått hittills i kursen
