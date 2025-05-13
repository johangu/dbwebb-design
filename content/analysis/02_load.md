Laddningstids- och Användbarhetsanalys
=======================

Den här delen av undersökningen fokuserar på tre webbplatsers tekniska prestanda. Genom att mäta laddningstider, antalet resurser och total datamängd har vi fått en bild av hur väloptimerade sajterna är och hur det påverkar användbarheten.

Urval
-----------------------

Likt analysen för färg och typografi har urvalet för denna analys fallit på nyhetsförmedling. Public service TV, en traditionell nyhetssagt samt en med inriktning på populärkultur. Intresset ligger i att se hur tillgängliga dessa är samt hur väl de följer best practices.
De tre webbplatserna som analyseras är:
- [Sveriges Television](https://www.svt.se) – Sveriges public service TV.
- [Svenska Dagbladet](https://www.svd.se) – en av Sveriges ledande dagstidningar.
- [Polygon](https://www.polygon.com) – en populärkultur- och dataspelsinriktad nyhetssajt.

Metod
-----------------------

Tre undersidor per webbplats valdes och testades med *Google PageSpeed Insights* för både mobil och desktop. Även webbläsarens DevTools (fliken Network) för att mäta laddningstid, sidstorlek och antal resurser. Varje sida laddades tre gånger och ett medelvärde beräknades. Resultaten redovisas nedan.

Resultat
-----------------------

<div class="embed-container">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRu3ZNfpdm-TClo3PNn7bT0LHR4s1SuxZifyGeSLRxvgM-TJ0ZdzXY8VvKoplH7pVMoE9OTEePK9dTK/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
</div>

### Sveriges Television

<img src="%base_url%/image/svt.png?w=1200&save-as=webp" alt="Screenshot of svt.se">

### Svenska Dagbladet
<img src="%base_url%/image/svd.png?w=1200&save-as=webp" alt="Screenshot of svd.se">

### Polygon
<img src="%base_url%/image/polygon.png?w=1200&save-as=webp" alt="Screenshot of polygon.com">


Analys
-----------------------

Mätresultaten visar tydligt att *Sveriges Television* har den snabbaste och mest konsekventa tekniska prestandan av de undersökta sajterna. Laddningstiderna är snabba, antalet resurser är lågt och sidstorleken hålls nere, vilket talar för att sajten är väl optimerad. Särskilt på desktop når SVT nästan toppbetyg i PageSpeed. Förbättringspotentialen är liten, men ytterligare prestanda skulle kunna vinnas genom mer aggressiv caching och fortsatt optimering av bildformat och kodladdning.

På andra plats finner vi *Svenska Dagbladet*. Prestandan för desktop är god, men mobilt lämnar mer att önska. SvD laddar många resurser, i vissa fall upp mot 96 förfrågningar, och sidvikten är ofta högre än nödvändigt. Det påverkar både laddningstid och användbarhet. Prestandan skulle kunna förbättras genom att slå ihop och minska antalet skript, optimera bilder och anpassa innehållstyngden bättre för mobila enheter.

Jumboplatsen går till *Polygon*. Undersidorna är både tunga och långsamma, särskilt på mobil där prestandan är svag. Flera sidor väger över 4 MB och laddningstiderna överstiger ofta 1 sekund. Det påverkar användarupplevelsen negativt, särskilt på långsammare nätverk. Vanliga flaskhalsar är många externa tredjepartsresurser, icke-optimerade bilder och onödigt stora skript. För att förbättra prestandan bör Polygon införa bildoptimering (till exempel WebP), minska antalet förfrågningar, ladda skript asynkront och använda lazy loading för tungt innehåll.

Jag upplever en snabb webbplats som en som laddar under 0,5 sekunder, medan en laddningstid på över 1 sekund känns märkbart långsam. Med det som gräns klarar SVT alla sidor utan problem. SvD ligger nära gränsen men passerar den ibland, medan Polygon ofta ligger över och upplevs som långsam. Resultaten speglar också den subjektiva användarupplevelsen: SVT känns snabb och lättanvänd, SvD fungerar men har en viss tröghet, och Polygon upplevs som långsam, särskilt på mobil.


Övrigt
-----------------------

Rapporten framtagen av jogm23.
