# Benjamins sida om stjärnbilder

Det här är min sida om stjärnbilder.

## Instruktioner

Hur man öppnar och navigerar på webbplatsen:

1. Clona det här git-repot.
2. Öppna i vscode.
3. Öppna index.html i live server.

## Kortfattad teknisk beskrivning hur jag uppfyllde kraven.

1. HTML-struktur:
    1. Använde section och article för att dela upp innehållet på sida. Gjorde en header med nav och en footer.
    2. En hemsida index.html och en undersida forum.html.
    3. Navigationsmenyn är likdan på alla sidor med endaskillnaden att aktuell sida är markerad.
2. CSS-styling
    1. Responsiv design: sidan anpassar sig till olika skärmstorlekar och är en kolumn i minsta och två i större. Flexbox i header och i main, grid i article. Clamp för bildernas storlek.
    2. Media quieries: Välxar mellan grid och inte i article vid smartphonestorlek. På smartphone och platta är länkarna större och luftigare.
    3. God praxis för namngivning och css-organisering: Jag har använd classnamn som säger vad det är och delat upp css-filen i sektioner med rubriker i kommertarer.
3. Responsiv design
    1. Webbplatsen är responsiv och fungerar väl eftersom layouten ändras enligt ovan.
    2. Flexbox: header och nav ul och grid article.
    3. clamp för bilder och textstorlek på p (den gör så att användaren inte kan råka ställa in för liten eller stor textstorlek i sin webbläsare)
4. Tillgänglighet
    1. Alt på alla bilder
    2. en h1 först som är rubrik för hela sidan därefter h2 som underrubriker till varje stjärnbild.
    3. Tillräcklig färgkontrast testat med wave.
    4. Beskrivande länkar, alla länkar förutom loggan beskriver vad de går till. Att loggan länkar till startsida är ett vanligt mönster men för den som inte vet om det finns alla länkar i navigeringsraden.
5. Webbläsarverktyg
    1. Jag har använd chrome devtools för att lösa html och css-problem. t. ex. så skrev jag id="#polstjärnan" och då funkde inte länken. Också för att visa grid-linjerna och prova ändra saker.
    2. Jag använde funktionen för att testa olika skärmstorlekar.
    3. Jag använde wave och lighthouse. Lighthouse tycker att jag ska placera länkarna glesare även på enheter utan touch.
6. Git
    1. Jag har använt git och branches. Skrivit tydliga commit meddelanden och delat upp branches för html och innehåll och en för stil.
7. Dokumentation
    1. Jag skriver i den här readme-filen instruktioner och beskrivning hur jag uppfyller kraven.
8. Presentation
    1. Jag förbereder presentationen genom att tänka igenom och öva punkterna som krävs.
    2. Jag är förberedd på frågor genom att ha sett till att kunna det jag har använt och ansträngt mig att förstå koden jag skrivit.

## TL;DR Ännu kortare

Ännu kortare beskrivning hur jag uppfyllt kraven: Jag har tittat på kraven, planerat min webbsida, skrivit koden och tittat på kraven, tittat på kraven en gång till när sida var klar.

## Utmaningar och lösningar

_Utmaning:_ Några av länkarna fungerar inte. _Lösning:_ id="#polstjärnan" till id="polstjärnan". Jag skrev rätt på de första sen blev det blandat fel.

_Utmaning:_ Grid sträcks ut på höjden som standard. _Lösning:_ grid-template-rows.

_Utmaning:_ Trött, begränsat med tid. _Lösning:_ Gör klar ändå, förenkla layouten. (Första sektionen skulle ha länkarna utspridda på sidorna om bilden, jag har skissat upp hur det ska vara med flexbox och grid kombinerat.)

_Utmaning:_ Kommer inte på hur jag ska få till image map (`<map><area>`) över bilden med alla stjärnbilder på ett sätt som är responsivt för mobil. Skärmlasare och tangentbord går bra men det verkar inte klara att bilden ändrar storlek i css. _Lösning:_ Hoppa över det här. Kanske lösa med svg eller position i framtiden. Hade gått låta bilden scrolla i sidled på mobil.

_Utmaning:_ Blir inte klok på om jag ska använda `<ul>` eller `<menu>` till listan med länkar i `<nav>`. Menu fanns i gammal html och var skrotad i html 4.01 men nu verkar den ha kommit tillbaka och är supported och semantisk i ny html. _Lösning:_ Kör ul för att det är vanligare. Gör ingen praktisk skillnad.

_Utmaning:_ Nu har jag kört branches lokalt med git i vscode, de syncas till github. Jag har mergeat i vscode men eftersom jag har jobbat själv och inte haft konflikter och inte mergeat via github webbsida så är det bara en rak tidslinje med commitsar och inga pull request. Jag vill veta mer om vad som är skillnaden på olika sätt att merga branches. _Lösning:_ experimentera mer med git och github och branches.

_Utmaning:_ Det krävs disciplin att jobba på endast en sak i varje commit. Nu när jag har skrivit dokumentationen så har jag samtidigt rättat och ändrat kanske tre andra saker. _Lösning:_ Att stagea inte bara vissa filer utan även endast delar av filer och därefter göra flera commits. Stash och commit amend hjälper också.