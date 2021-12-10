---
Title: Laddningstid och användbarhet
Description: Analys from kmom04/05/06
Template: analysis
---

Laddningstid och användbarhet
===========================
I den här rapporten kommer vi att analysera tre webbplatser och jämföra hur snabba sidorna är och därmed också hur användbara dessa är.


Urval
-----------------------
I den här rapporten har vi valt att analysera tre stora nyhetssidor. De sidor vi har valt är <a href="http://aftonbladet.se">Aftonbladet</a>, <a href="http://svt.se">SVT</a> och <a href="http://cnn.com">CNN</a>. Vi valde dem eftersom de alla är sidor med mycket innehåll och många besökare. På varje hemsida har vi valt ut att kolla startsidan, sportsidan och kultursidan.

Metod
-----------------------
Vi har använt oss av Firefox Devtools, PageSpeed och Google Lighthouse för att samla in mätvärden för de tre hemsidorna. I tabellen har vi med det genomsnittliga värdet av laddningstid, storlek och antal resurser både med och utan adblock från Devtools samt betyg från Google Lighthouse. Vi har inte med något från PageSpeed då vi inte fick fram värden till alla sidor och därför inte fick resultat som vi kunde analysera. Vi har även använt Google Lighthouse för att se vad sidorna skulle kunna förbättra för att bli snabbare.

Resultat
-----------------------

<iframe class="tabell" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSJv6LVpTcky13QiQ1xpSzFhe6pODYxv8QuM12Vngtz3EHMSbXDRFFJmYyCpvAvTjCP5v2_jHP7twyx/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

### Aftonbladet
![Snapshot Aftonbladet](../assets/img/aftonbladet.png){.snapshot}

Aftonbladet skulle kunna förbättra sin webbplats genom att skicka rätt storlek på sina bilder, alltså inte onödigt stora bilder samt att minska JavaScript i reklam. Överlag skulle reklamen kunna ta mindre plats då det är den som tar mest plats och gör sidan långsam.

### SVT
![Snapshot SVT](../assets/img/svt.png){.snapshot}

SVT får generellt ett bra betyg från Google Lighthouse men om den ska förbättras så skulle det kunna vara genom att kolla över JavaScript. Bilderna som skickas är små men med bra kvalitet så det gör de bra.

### CNN
![Snapshot CNN](../assets/img/cnn.png){.snapshot}

CNN har stor förbättringspotential och skulle kunna göras snabbare om de ser över fontladdningen, vilken font de använder. De kan också skicka rätt storlek på bilderna, ta bort oanvänd JavaScript, se över DOM-trädets storlek samt använda document.write() i lägre utsträckning då det kan ställa till problem för användare med dålig uppkoppling.


Analys
-----------------------
Ganska snabbt in i undersökningen såg vi att reklamen på Aftonbladet och CNN spelar stor roll för både snabbhet och storlek på sidorna. Därefter kunde vi i resultatet se att SVT, som inte har någon reklam på sin webbplats,  har en betydligt mycket snabbare sida än de andra. Vi kan se att startsidan på varje webbsida är snabbare än undersidorna sport och kultur, det är genomgående för alla tre webbsidor. 

Den vanligaste förbättringsåtgärden som vi kan se på alla tre webbplatser verkar vara att kolla över och rensa onödig JavaScript. Utöver det är en annan förbättringsåtgärd att se över storleken på bilderna, något som både Aftonbladet och CNN skulle kunna justera för att göra sidorna snabbare. 

När vi använde Pagespeed för att analysera sidorna tyckte vi att resultaten var orimliga, till exempel fick vissa sidor 30-40 sekunder innan de var interactive vilket inte återspeglade vår upplevelse när vi själva besökte sidorna. För vissa av sidorna fick vi inget resultat överhuvudtaget vilket gjorde att vi valde att överge Pagespeed till förmån för Google Lighthouse som verktyg för våra analyser.

Rangordning baserat på laddningstid
-------------------------------------
Vi har diskuterat och kom fram till att en sida som laddar på 1 sekund och mindre är en snabb och bra webbsida. När en webbsida laddar långsammare än så, upp mot 2-3 sekunder och även långsammare så klassar vi det som en långsam sida. Vi tror att det kan göra att besökaren tappar intresset och inte uppskattar besöket.

Baserat på de uppmätta värdena anser vi att SVT är den klara vinnaren med 0.9 sekunders laddningstid för startsidan och under 1.5 sekunders laddningstid för sport- och kultursidorna. SVT har också på ett bra sätt optimerat sina bilder vilket bidrar till det fina resultatet.

På andra plats i vår bedömning kommer Aftonbladet vars förstasida laddas in på i snitt 1.51 sekunder, inget dåligt resultat men den längre laddningstiden är kännbar.

Sist kommer CNN. Här tar det hela 2.25 sekunder för förstasidan att laddas in vilket är en markant skillnad mot SVT och gör att hela sidan känns långsam.


Referenser
-----------------------
<a href="https://pagespeed.web.dev/">Pagespeed</a>,
<a href="https://developer.mozilla.org/en-US/docs/Tools?retiredLocale=sv-SE">Firefox Devtools</a> och 
<a href="https://developers.google.com/web/tools/lighthouse">Google Lighthouse</a>


Övrigt
-----------------------
Agnes Rodhe, Mattias Eriksson och Oscar Idberg
