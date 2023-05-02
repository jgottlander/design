---
Title: Analys av laddningstider för valda webbsidor
Description: This is my analysis page.
---

# Analys av diverse webbsidors laddningstid

Denna analys går ut på att undersöka 3 olika webbsidors laddningstid, och om det kan förbättras

## Urval

Jag har vald webbsidor från DN, Canonicals Ubuntu samt Tesla. Liksom förra rapporten tänker jag att det hade varit roligt att jämföra olika företag. DN som nyhetsbolag har ju rätt många olika bilder till sina rubriker och artiklar, Ubuntu har mest text med en del visuell grafik och ikoner, medan Tesla visar stora helskärmsbilder, och se hur det påverkar laddningstiden.

## Metod

Jag använde dels [PageSpeed Insights](https://pagespeed.web.dev/) och mätte värdena för både mobil och skrivbord. Därefter använde jag devtool för Firefox och kollade på laddningstid (load), resurser (antal begäran) samt storlek på alla förfrågningar. Jag inaktiverade också cachen för detta, gjorde tre test och tog snittet av dessa.

## Resultat

### Tabell med alla resultat
<iframe style="width: 48em; height: 16em; border: none" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vS_fvykHWGMY15Ejp48cacC_uYzYsB5P3YCFENQTX4rEIUgDzi_KnbIwcORV4h9YQc4LFZNPcxNNhRl/pubhtml?gid=0&single=true&widget=true&headers=false"></iframe>

DN behöver framförallt fixa sin sida som skiftar medan den laddas. För Ubuntus sida så tar det väldigt lång tid att få första informationen, så alla laddningstider påverkas av detta. Tesla har mycket stora bilder tar lång tid att ladda.

## Analys

### Dagens Nyheter

DN hade bra värden i Insights-testet. De hade dock positiva värden i CLS (Cumulative Layout Shift), dvs. hur mycket av sidan som ändrar sig efterhand den laddas. Ett värde under 0,1 är godkänt. För skrivbord var värdet 0,12 vilket altså är för högt. Ett sätt att åtgärda detta är att ange hur mycket utrymme element tar upp så att den platsen kan reserveras innan t.ex. bilden har laddats.

DN har också den högsta laddningstiden av alla sidor, när jag testar på min dator. Vad jag kan se när jag kollar på alla indivuella begär så är det fonter, skript och reklam som tar längst tid.

Sidan har mycket reklam vilket nog de flesta tidningar utnyttjar sig av för att tjäna extra pengar. Och dessa sköts högst sannoligt av skript och bilder som tar tid att ladda, så det mest realistiska är att optimera skript och bilder, för reklamen är nog svårt att dra ned på.

### Ubuntu

Ubuntu var den sidan som laddadest snabbast på min dator, men fick inte godkänt av Insights på många värden i mobilversionen. LCP låg på 3,2 s, dvs Largest Contentful Paint, där största delen av sidan visas.
Tid för första byte (TTFB) var 1,1 s för mobil, vilken låter väldigt mycket, och har antaligen med servern eller kopplingen att göra, vilken också bidrar till att de andra värdena var så dåliga. På skrivbordsversionen får alla värden godkänt, även om TTFB är nära gränsen; 700 ms där värden under 800 ms är godkända.

Denna sida var också den minsta, storleksmässigt, av de tre, så anledningen att den laddar långsamt har antaligen med bandbredd och serverkapacitet att göra, eventuellt kan DNS- eller serverinställningar också bidra till långsamma laddningstider.

### Tesla

Tesla får inte godkänt i LCP, som visar hur lång tid det tar innan användaren kan se något överhuvudtaget, under 1,8 s är godkänt. Den hade också färst resurser men störst storlek, vilket antagligen tyder på stora bilder, vilket devtools också bekräftar. Så för stora bilder är altså flaskhalsen på denna sida.
Den har också en del skript som tar tid, där många kommer från Google Analytics, vilket alltså har med webbanalys att göra.

Jag får lite motsägelsefulla mätvärden med Insights kontra devtools på min egen dator. T.ex. för Ubuntu så fick jag en LCP på 3,2 resp. 2,3 sekunder för mobil och skrivbord. Men när jag mäter på min egen dator får jag en total laddningstid på drygt 1 sekund, vet inte riktigt hur det kommer sig.

Jag använder normalt en reklamblokerare ((Pi-hole)[https://pi-hole.net/]) på mitt hemmanätverk. Och när den är aktiverad så minskar laddningstiden på alla sidor, framförallt DN:s sida minskar med upp till en sekund i vissa fall, och antalet resurser minskar från 134 till runt 45.

## Referenser

- [Dagens Nyheter](https://www.dn.se/)
- [Ubuntu](https://ubuntu.com/)
- [Tesla](https://www.tesla.com/)
- [PageSpeed Insights](https://pagespeed.web.dev/)

## Övrigt

Josef Gottlander har skrivit denna rapport.