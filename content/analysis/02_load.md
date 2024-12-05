---
Title: Load
Description: This is load page.
Template: analys
---

Analys av hemsidor: laddningstid och användbarhet
=======================

Uppgiften handlar om att analysera tre olika hemsidor och undersöka laddningstiden och användbarheten för de valda webbplatserna.

Urval
-----------------------

De tre hemsidor jag har valt att analysera är BookBeat, Nextory och Storytel. Jag valde att utgå från kategorin streamingtjänster för ljud- och e-böcker i min analys. Urvalet gjordes utifrån de streamingtjänster som jag själv använt tidigare och hade en tidigare kännedom om.

I uppgiften skulle tre sidor på de valda webbplatserna analyseras. Jag valde sidor som fanns på samtliga webbplatser vilket var sidorna Startsida, Ljudböcker och Kategorier. Jag valde 2 sekunder som gränsvärde för absolut laddningstid. 


Metod
-----------------------
Metoden för denna uppgift var att hämta data för prestanda, laddningstid, resurser och totala storlek för de tre valda webbplatserna. Prestandan hämtades genom Google Pagespeed. Den specifika webbplatsens URL angavs och prestandan räknades sedan ut både mobilt och dator. Detta gjordes för tre olika sidor på vardera hemsida. Den insamlade datan fördes sedan in i ett Excel-ark. 

Verktyget DevTools användes för att få fram sidans laddningstid, resurser som laddas in och sidans totala storlek. Detta gjordes genom fliken Network och sidornas värden mättes genom att ladda om den aktuella sidan. Mätning gjordes totalt tre gånger för varje separat sida och snittvärdet fördes sedan in i ett Excel-ark.

För att ta skärmdumpar av varje webbplats används det inbyggda verktyget “Ta skärmdump” i webbläsaren Firefox.

Resultat
-----------------------

<h3> Storytel </h3>

<a target="_blank" href="../assets/img/storytel_1.png">
    ![me](%assets_url%/img/storytel_1.png) {.img-color} 
</a>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSjGtq8kPc8WAsDty4MQ-TACv6dT3y7-ljggcW2qpEddVQnHPbv4DxG9MYj7lrauUfiEyUTRMKIXoxL/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="result"></iframe>

Enligt resultatet i Google PageSpeed har webbplatsen för Storytel en lite sämre prestanda. För det mobila läget var prestandan mellan värdet 33 och 35 för de tre olika sidorna. Prestandan var däremot bättre för datorn. Värdet för prestandan var 64 för sidorna Startsida och Ljudböcker och 87 för sidan Kategorier. Google PageSpeed nämner förbättringar såsom att minska körningstiden med JavaScript, använda bilder med rätt storlek och modernare bildformat. Man kan se att hemsidan för Storytel innehåller många olika element, bilder, effekter och animeringar vilket kan vara en anledning till den sämre prestandan.  

Mätningen med DevTools resulterade i laddningstider under det valda gränsvärdet, 2 sekunder, för samtliga tre sidor. Laddningstiden var som längst för sidan Startsida med tiden 1,59 sekunder. Detta kan bero på att denna sida är den sida som består av mest innehåll och olika element av de tre valda sidorna. 

<h3> Nextory </h3>

<a target="_blank" href="../assets/img/nextory_1.png">
    ![me](%assets_url%/img/nextory_1.png) {.img-color} 
</a>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQdlCYhIXOoJLFsPYd7PQyeRDSzeR8KmGzx7TuqYiTper_8IZBRcu5zdysU0X7iPvcqOzXhCZTPARtx/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="result"></iframe>

Nextory hade generellt en hög prestanda för både mobilen och datorn i resultatet för Google PageSpeed. Värdet för prestandan för mobilen var mellan 96 och 98 medan för datorn var värdet 100. Verktyget nämnde några få förbättringar såsom att använda bilder med rätt storlek och reducera CSS som inte används. Anledningen till den höga prestandan kan vara webbplatsens mer simpla design med färre bilder och element. Detta stämmer även överens med mätvärdena i DevTools där laddningstiden var snabb, under 1 sekund för alla tre sidor. Man kan även se att storleken för resurserna som laddades in var ganska liten vilket även ligger i linje med de snabba laddningstiderna.

<h3> BookBeat </h3>

<a target="_blank" href="../assets/img/bookbeat_1.png">
    ![me](%assets_url%/img/bookbeat_1.png) {.img-color}  
</a>
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRcCJeYsK2MyeYDfsFuUzOt-OSuXEwvPx-YHZ3123loZD1lyPShjkKPJYT67Slop98pVTRZtJYuopVL/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="result"></iframe>

Resultatet för BookBeats prestanda i Google PageSpeed visade generellt låga värden. Prestandan för mobilen var för sidorna Startsida och Kategorier värdet 31 och för sidan Ljudböcker 43. Värdet var däremot högre för dator som visade värdet 60 för sidan Startsida, 56 för sidan Ljudböcker och 86 för sidan Kategorier. Google PageSpeed nämner förbättringar såsom att minska körningstiden för JavaScript, reducera CSS och JavaScript som inte används och att undvika ett onödigt stort DOM-träd. 

Laddningstiden för BookBeat var under gränsvärdet 2 sekunder och den långsammaste sidan var Kategorier, 1,51 sekunder, vilket även var den sida med flest resurser som laddades in. Hemsidan innehåller många olika bilder, animeringar och JavaScript vilket antagligen påverkar både prestandan och laddningstiden.


Analys
-----------------------
De vanligaste förbättringsåtgärderna för urvalet av webbplatser är att använda bilder med rätt storlek, reducera kod, undvika att ladda in för många resurser och att minska körningstiden med JavaScript. De hemsidor med mer bilder, element och innehåll hade sämre mätvärden än de hemsidor som hade mindre innehåll.

Vid rangordning av webbplatsernas mätvärden blev resultatet:
<ol>
    <li> Nextory </li>
    <li> Storytel </li>
    <li> BookBeat </li>
</ol>

Vid analys så ser man att Nextory hade de bästa mätvärden både gällande prestanda och laddningstid. Därmed blev Nextory vinnaren av testet. Detta beror troligtvis på den simpla designen med ett fåtal element, bilder och inga flashiga animationer. Medan både Storytel och BookBeat fick ganska svaga prestanda-värden med längre laddningstider. I mätvärdena kan man även se att det var de hemsidor som laddade in flest resurser, vilket stämmer överens med resultatet. 

Den valda gränsen för absolut laddningstid var två sekunder. Samtliga webbplatser klarade gränsvärdet. Laddningstiden för Nextory var snabbast, under en sekund. Medan Storytel och BookBeat hade en laddningstid mellan en och två sekunder. Det är ingen skillnad jag märker direkt med blotta ögat utan jag upplever att samtliga sidor laddas in snabbt och smidigt.

Övrigt
-----------------------

Skriven av Liv Frej