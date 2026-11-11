# Monster-værkstedet – browserprototype

**Version 1.0 – til voksen-test, ikke til indsamling af børnestemmer endnu.**

## Det kan denne version

- Viser brugerens egen monsterfigur fra billedcollagen.
- Siger hej med en dansk computerstemme fra browseren (hvis der er en dansk stemme tilgængelig).
- Lytter til en talebeskrivelse via browserens danske talegenkendelse, hvor understøttet.
- Giver den voksne mulighed for at rette teksten.
- Laver en **simpel demoillustration med JavaScript** ud fra udvalgte ord: farver, øjne, ben, horn, vinger, hale mv.
- Lader barnet/voksne fortælle ændringer og tegne en ny version.
- Gemmer testbilledet som PNG.
- Bruger ingen cookies, login, database eller lokal lagring i selve appen.

**Vigtigt:** Illustrationerne er **ikke AI-genererede** i denne version. Den tidligere billedprompt er ikke koblet på en billedgenerator endnu. Der skal senere bygges en sikker serverfunktion med en AI-billedtjeneste, hvis billedet skal fortolke hele barnets beskrivelse som i jeres Copilot-afprøvning. En API-nøgle må aldrig lægges i GitHub Pages-koden.

## Sådan prøver du den

1. Udpak ZIP-filen.
2. Åbn `index.html` i en browser for at teste knapper, oplæsning og eksempeltekst. Mikrofonen virker ofte kun på `https://` eller localhost.
3. Til browser- og mikrofontest: læg **indholdet** af mappen i roden af et nyt offentligt GitHub-repository og aktivér **Settings → Pages → Deploy from a branch → main / root**. Åbn GitHub Pages-adressen, når den er klar.
4. Prøv i Chrome eller Edge. Tillad adgang til mikrofonen, hvis du selv tester med stemmen.

Hvis du ikke har oprettet et repository endnu, skal det ske, før denne ZIP kan lægges derind. Appen er fuldt statisk og kræver ikke installering af npm-pakker.

## Data og børns privatliv

Browserbaseret talegenkendelse kan sende mikrofonens lyd til browserleverandørens tjeneste. Appen gemmer ikke en lydfil, men det **betyder ikke**, at mikrofondata kun behandles lokalt. Afprøv derfor mikrofonen med **voksnes teststemmer eller opdigtet indhold**, indtil samtykke, leverandørforhold og databehandling er afklaret med den relevante institution.

Tekst og testillustration holdes i browserfanens hukommelse, indtil fanen lukkes, eller barnet begynder forfra. Ved klik på "Gem billedet" downloades filen til enheden.

## Næste tekniske del (ikke indbygget endnu)

En serverfunktion med hemmelig API-nøgle, passende adgangskontrol og omkostningsbegrænsning kan bruge jeres eksisterende billedprompt – omskrevet til alene at basere sig på barnets beskrivelse. Et rent GitHub Pages-site kan ikke holde en API-nøgle skjult.
