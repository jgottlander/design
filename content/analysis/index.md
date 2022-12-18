---
Title: Analys
Description: This is my analysis page.
---

# Analys av diverse webbsidor

Uppgiften är att dokumentera olika webbplatsers färgpalett och typografi. Därefter argumentera för om layouten återspeglar vad webbsidan vill kommunicera.

## Urval

Jag valde att analysera tre olika slags webbsidor, från olika delar av samhället. En offentlig-, en privat- och en kultursida, nämligen Folkhälsomyndigheten, datortillverkaren Lenovo, samt Folkoperan i Stockholm. Dels för att se om det kunde finnas några likheter men också skillnader.

## Metod

Jag använde först en funktion som heter HEX Color Extractor på [hexcolor.co](https://hexcolor.co/css-color-extractor). Där man klistrar in länken till webbplatsens CSS-fil och får sedan en tabell med alla färger som används, och hur många gånger respektive färg användes. Men jag ville också jämföra med andra verktyg som t.ex. [Color Combos](https://www.colorcombos.com), som är en annan webbsida där man endast behövde skriva in webbadressen och så fick man ut alla färger. Men jag testade också verktyget Color palette from image på [ColorDesigner](https://colordesigner.io), där jag använde en skärmdump av respektive sida. Resultatet varierade väldigt mycket och framförallt den sistnämnda gav inte så bra resultat av Lenovos och Folkoperans sidor eftersom de använder mycket bilder och gradienter som ger väldigt många olika färger som nödvändigtvis inte existerar i färgprofilen. Nedan har jag använd resultaten från hexcolor.co.

För typsnitt använde jag webbläsarens Inspektör och klickade på respektive rubrik och brödtext för att se vilket typsnitt som användes.


(Berätta kort om din "metod", hur du gör för att utföra undersökningen. Berätta om du använder något speciellt verktyg.)

## Resultat

### Folkhälsomyndigheten

Folkhälsomyndighetens CSS-fil hade 90 olika färger i sig, nedan är de 10 vanligaste. Men man kunde tydligt se att förutom vit och svart så rörde det sig om många olika nyanser av mörkblå samt ljusgrå, plus enstaka grön och röd, men dessa två kan jag inte se på framsidan. Här rör det sig helt klart om en monokromatiskt färgschema, om man ser grå som en variant av vit. Det förekommer också en variant av turkos/grön som skulle kunna ses som en variant av blå. Men det rör sig snarare om en accentfärg.

<table class="color-palette">
<tr>
<td style="height: 50px; width: 50px; background-color: #FFFFFF">
<td style="height: 50px; width: 50px; background-color: #000000">
<td style="height: 50px; width: 50px; background-color: #2D5492">
<td style="height: 50px; width: 50px; background-color: #15AF97">
<td style="height: 50px; width: 50px; background-color: #005C9A">
<td style="height: 50px; width: 50px; background-color: #EBEBEB">
<td style="height: 50px; width: 50px; background-color: #EAEEF4">
<td style="height: 50px; width: 50px; background-color: #E5F0F7">
<td style="height: 50px; width: 50px; background-color: #E3E3E3">
<td style="height: 50px; width: 50px; background-color: #15AF9B">
</tr>
</table>

För rubrikerna används ett typsnitt som heter *Klavika* som är en sans-serif. I brödtexten används Microsoftypsnittet *Tahoma* som också är en sans-serif. Värt att nämna är att *Klavika Light* används till den lilla introtexten på varje sida.

Jag tror inte att det är en slump att de har valt en blå färg som huvudfärg på sidan, eftersom den signalerar lugn men även öppenhet och intelligens. Vilket är bra egenskaper för en myndighet som bland annat skall förmedla information om eventuella faror som existerar just nu och samtidigt inte sprida panik. Överlag en rätt enkel och ren stil som utstrålar ett proffsigt utseende.

### Lenovo

Det fanns också rätt många färger i paletten hos Lenovo, dock inte lika många som på föregående sida. Nedan är de 5 vanligaste.
Även om röd inte förekom så ofta i paletten så är det helt klart den dominerande färgen på förstasidan, men det beror på att de använder mycket bilder med rött i sig.

Förutom svart, vitt och nyanser av grått så finns det också blått och rött, samt lite grönt på vissa ställen, vilket får mig att tro att detta rör sig om ett triadiskt färgschema. Och blått är helt klart accentfärg.

Både rubriker och brödtext använder Googletypsnittet Lato, som är en sans-serif.

Jag tycker att webbsidan utstrålar ett professionellt men kanske aningen föråldrat/traditionellt utseende, som skulle kunna symbolisera stabilitet om något.

<table class="color-palette">
<tr>
<td style="height: 50px; width: 50px; background-color: #FFFFFF">
<td style="height: 50px; width: 50px; background-color: #1976A1">
<td style="height: 50px; width: 50px; background-color: #000000">
<td style="height: 50px; width: 50px; background-color: #E6E6E6">
<td style="height: 50px; width: 50px; background-color: #777777">
</tr>
</table>

### Folkoperan

Folkoperans webbsida är väldigt modern och visuell, använder sig av mycket bilder och gradienter, med svart på vitt eller omvänt. Röd som tydlig accentfärg. Jag vet inte riktigt hur jag skulle klassificera deras färgschema, men jag lutar nog mest åt monokromatisk då olika nyanser av rött är egentligen den enda färgen som förekommer, förutom svart, vitt och grått.

Det typsnitt som används genomgående på rubriker och brödtext heter *Folkoperan Futura ND*, som antaligen är en modifierad version av Adobetypsnittet Futura, som också ligger som reservtypsnitt. Det är en sans-serif.

Folkoperans image är att leverar opera till hela folket, och med sitt moderna och slitrena utseende tycker jag att att de utstrålar en modern och sjusig image som jag tror appilerar till de flesta i befolkningen.

<table class="color-palette">
<tr>
<td style="height: 50px; width: 50px; background-color: #FFFFFF">
<td style="height: 50px; width: 50px; background-color: #231F20">
<td style="height: 50px; width: 50px; background-color: #D31245">
<td style="height: 50px; width: 50px; background-color: #F1607C">
<td style="height: 50px; width: 50px; background-color: #0A0A0A">
</tr>
</table>

## Analys

Alla sidor använde sig av svart och vitt; svart text på vit bakgrund, eller ibland omvänt. Blått förekom också på något sätt på alla sidor; de två första i själva färgpaletten som accentfärg och på Folkoperans sida på en del bilder.

Jag tycker att det är lite intressant att ingen av sidorna använder sig av seriftypsnitt. Jag misstänker att det ger ett mer modernt utseende med en sans-serif, samt att seriffer nog för tankarna till böcker eller annan tryckt text, där dessa sidor nog önskar att förmedla lättare stoff som inte är lika tungt att läsa som t.ex. en roman eller publicerade rapporter.

En annan intressant sak var att alla sidor CSS-filer innehöll många färger. Folkoperan hade 18 st olika färger, Lenovo 30 st, och Folkhälsomyndigheten hela 90 st unika färger i sin stil. Jag tänker nog att inte alla används på sidan, och att det nog rör sig om olika versioner av teman och att inte alla färger används i det aktuella temat.

## Referenser

dbwebb (u.å). Färg. [https://dbwebb.se/guide/design-med-html5-och-css3/farg](https://dbwebb.se/guide/design-med-html5-och-css3/farg)

Beaird J. (2014) 'Color' in The *Principles of Beautiful Web Design*. SITEPOINT

## Övrigt

Josef Gottlander har skrivit denna rapport.