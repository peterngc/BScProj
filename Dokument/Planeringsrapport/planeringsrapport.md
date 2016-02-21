<span style="font-variant:small-caps;">Chalmers tekniska högskola</span>

------------------------------------------------------------------------

<span> Programmering som undervisningsverktyg för signaler och system
</span>

------------------------------------------------------------------------

*Författare:
Filip Lindahl
Cecilia Rosvall
Peter Ngo
Jacob Jonsson
Joakim Olsson
*

Bakgrund
========

På Chalmers Tekniska Högskola har det funnits en lång trend där studenterna på utbildningen för Datateknik har haft svårigheter med kurserna *Transformer, Signaler och System*, hädanefter omnämnd som ”TSS”, och *Reglerteknik*. Dessa svårigheter tror examinatorerna i kurserna beror till stor del på att studenterna inte är tillräckligt bekväma i det matematiska språket. Studenterna på Datateknik har inte tillräcklig vana att tolka innebörden av de matematiska beskrivningarna och är allmänt ovana vid matematiskt hantverk. Därför lägger datastudenterna det mesta av sin energi på att få ihop matematiken rent praktiskt, istället för att se vad matematiken står för.

Detta syns bland annat i statistiken för hur många datastudenter som klarar kurserna, under perioden från 2010 till 2016 blev i genomsnitt 51% av alla som skrev tentamen godkända i TSS och under samma period blev 53% godkända i Reglerteknik 1. Det finns även ett mörkertal i dessa siffror eftersom inte alla studenter skriver tentan, exempelvis valde 48 studenter utav 122 registrerade att inte tentera Reglerteknik 2014 2.

För att minska svårigheterna som studenterna har för dessa kurser påbörjades ett pedagogiskt projekt, DSLsOfMath, som hittills resulterat i kursen *Matematikens domänspecifika språk*, där man använder funktionell programmering för att beskriva matematiska problem 3. Resonemanget bakom detta var att funktionell programmering är ett verktyg som datastudenterna har erfarenhet av och som använder en notation med fokus på tydlighet som lämpar sig relativt väl för att lära ut matematiska begrepp 4.

Detta projekt uppstod som en avgrening av DSLsOfMath-projektet med fokus mer på signal- och systemteoretiska färdigheter snarare än en allmän matematisk grund.

Syfte
=====

Syftet med projektet är att underlätta för studenter inom datateknik att ta till sig signal- och systemteoretiska ämnen genom att utnyttja deras kunskaper inom programmering och även göra det möjligt att betrakta ämnet ur en programmerares perspektiv. Tanken bakom detta är att man ska göra gapet mellan datateknik och signalteori mindre och minska problemen som nämns i bakgrundsavsnittet.

Projektet är tänkt att resultera i en handledningsguide, en så kallad tutorial, som kan fungera som ett komplement till de kurser som ges inom signalteori på den datatekniska grundutbildningen. Denna guide ska innehålla förklaringar och programmeringsövningar som är anpassade för studenter på den datatekniska utbildningen på Chalmers tekniska högskola.

Problemanalys
=============

Uppgiften i detta projekt är att utarbeta en tutorial som komplement till kurserna Reglerteknik och TSS.

För att kunna utveckla denna tutorial kommer först omfattande förstudier behöva bedrivas innan den skrivs och den kommer även behövas testas.

Förstudier
----------

För att komma till rätta med datastudenternas största svårigheter med förståelsen inom ämnena behövs först en undersökning för att ta reda på var dessa ligger mer i detalj. Dessutom behövs efterforskningar och litteraturstudier inom såväl pedagogik som teorin bakom de tidigare nämnda kurserna för att kunna skriva en tutorial med korrekt och tydligt innehåll.

Produkten
---------

Efter förstudierna kommer en tutorial utvecklas. Innehållet i denna kommer bestå av förklarande teori, exempel inom såväl teori som programmering, samt övningar med tillhörande lösningar.

Produktens målgrupp är studenter vid datateknikprogrammet på Chalmers Tekniska Högskola som läser andra eller tredje året på utbildningen.

Produkten kommer sedan behöva testas på den aktuella målgruppen för möjligheten att uppdatera och förbättra den slutgiltiga produkten.

Avgränsning
===========

Det kommer endast fokuseras på svårigheterna inom kurserna TSS och Reglerteknik. Det vill säga, projektet är inte tänkt att resultera i ett hjälpmedel som täcker allt i kurserna utan ska vara ett komplement som minskar svårigheterna för målgruppen.

Dessutom kommer denna tutorial inte innehålla något av momenten kursen *Matematikens domänspecifika språk* täcker.

Metod
=====

Projektet kommer att bestå av tre delar: Förstudier, produktutveckling och testning. Dessa delar kommer sedan itereras för att få en genomarbetad slutprodukt.

Förstudier
----------

För att samla in information om vilka moment i kurserna TSS och Reglerteknik som datastudenter har svårast för har vi intervjuat examinatorerna om de övergripande svårigheterna inom båda kurserna. Vi kommer under projektets gång ha fler intervjuer med examinatorerna där det läggs mer fokus på detaljer.

För att få information av datastudenterna om vad de tyckte var svårt kommer vi utarbeta en enkät om såväl kurserna som deras förkunskaper och analysera resultatet från denna.

För att kunna skriva en lättläst och begriplig tutorial kommer vi studera litteratur inom pedagogik samt alternativa inlärningsformer som exempelvis boken och hemsidan *Learn you a Haskell for great good* 5. Litteraturen kommer väljas baserat på rekomendationer från projektets handledare och anställda vid Chalmers bibliotek samt egna efterforskningar.

Produkten
---------

Programeringskoden till projektet kommer skrivas i Haskell, vilket från början var specifierat från instutitionen för Data och Informationsteknik som skapade projektet. Haskell är ett programeringsspråk med syntax som liknar den matematiska notationen. Språket har dessutom egenskaper som gör att det lämpar sig väl som värdspråk för ett domänspecifikt språk, Haskell har till exempel stöd för att skapa egna datatyper. Därför såg vi ingen anledning att ändra specifikationen.

Rent strukturellt planerar vi att dela upp vår tutorial i sex delavsnitt som kommer att innehålla informativ text som förklarar delavsnittet och runt 15 – 20 uppgifter vardera. I uppgifterna får studenterna lära sig om signaler och system genom att implementera de inblandade typerna och relationerna som domänspecifika språk i Haskell.

Testa produkten
---------------

För att testa svårighetsgraden på vår produkt kommer vi först att testa vår tutorials övningar internt. Tanken är att vi kommer dela upp delavsnitten så att två till tre personer skriver ett delavsnitt och sedan kan gruppmedlemmarna testa varandras arbete. På detta sätt kommer vi ha möjlighet att förbättra och utveckla delavsnitten innan de testas på andra studenter.

Sedan kommer vi att testa vår tutorial på datastudenter genom att de får läsa texterna och göra uppgifter till ett eller flera avsnitt. Efter att de har läst och implementerat uppgifterna kommer de att få svara på frågor angående hur de upplevde texten och uppgifter i en enkät. I enkäten kommer vi också att testa studenternas förståelse av det avhandlade avsnittet.

Utifrån dessa tester och enkäter kommer vi sedan vidareutveckla och förfina slutprodukten.

Tidsplan
========

För att göra projektet mer överskådligt ur ett tidsperspektiv har ett antal milstolpar tagits fram. Samtliga av dessa har en preliminär deadline för att ge gruppen något att arbeta mot.

Milstolpar
----------

-   2016-02-10 - Planeringsrapport och grov planering klar

-   2016-02-11 - Fackspråkshandledningstillfälle 1

-   2016-02-12 - Planeringsrapport inlämning

-   2016-02-24 - Intervjuer, grundläggande efterforskningar om TSS och reglerkurserna klara

-   2016-02-24 - Litteraturstudier inom pedagogik klara

-   2016-03-01 - Utkast för grov tutorial klar (uppgifter ej klara)

-   2016-03-01 - Få klart ett litet avsnitt för halvtidsredovisningen, med förslag på uppgifter och text

-   2016-03-01 - Halvtidsredovisning

-   2016-03-15 - Uppgifter och utkast till text för två av sex delavsnitt i tutorial klara

-   2016-03-22 - Första utkast till rapporten klart

-   2016-03-22 - Fackspråkshandledningstillfälle 2

-   2016-03-28 - Bearbetning av feedback från fackspråk

-   2016-04-11 - Uppgifter och utkast till text för fyra av sex delavsnitt i tutorial klara

-   2016-04-25 - Uppgifter och utkast till alla delavsnitt i tutorial klara

-   2016-04-27 - Eventuell engelsk (forskningsinriktad) uppsats klar

-   2016-04-28 - Andra utkast till rapporten klart

-   2016-05-04 - Tutorial klar och testad

-   2016-05-11 - Rapporten klar

-   2016-05-13 - Fackspråkshandledningstillfälle 3

-   2016-05-16 - Rapportinlämning

-   2016-05-17 - Utställning

-   2016-05-26 - Deadline för opposition

-   2016-05-26/27 - Slutredovisning

-   2016-06-01 - Sista inlämningen

Gantt schema
------------

Nedan följer ett Gantt schema för att ge en överblick om hur gruppens arbete fördelas över projekttiden.

\[1\] C. T. Högskola, “Statistik över kursresultat,” 2016. \[Online\]. Available: <http://document.chalmers.se/doc/00000000-0000-0000-0000-00001C968DC6>.

\[2\] C. T. Högskola, “ERE102 - reglerteknik,” 2014. \[Online\]. Available: <http://document.chalmers.se/doc/b1ebfabc-b2c1-41a3-bf22-35711526aae8>.

\[3\] C. T. Högskola, “DAT325 - matematikens domänspecifika,” 2016. \[Online\]. Available: <https://www.student.chalmers.se/sp/course?course_id=24179>.

\[4\] C. Ionescu and P. Jansson, “Domain-specific languages of mathematics: Presenting mathematical analysis using functional programming.” p. 15, 2015.

\[5\] M. Lipovača, *Learn you a haskell for great good!* No Starch Press, 2011.