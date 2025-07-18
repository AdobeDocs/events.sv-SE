---
title: Fråga experten - Mäta hastighet
description: Lär dig mäta och spåra hastigheten med hjälp av  [!DNL Workfront] -rapportering. Denna workshop spelades in den 14 augusti 2019.
doc-type: feature video
team: Technical Marketing
jira: KT-9912
last-substantial-update: 2023-08-15T00:00:00Z
exl-id: 83053de2-e386-4243-a9c8-a2ad9d51790f
duration: 4630
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '3962'
ht-degree: 0%

---

# Fråga experten - Mäta hastighet

Lär dig att mäta och spåra hastigheten med hjälp av [!DNL Workfront]-rapportering. Denna workshop spelades in den 14 augusti 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341057/?quality=12)

## Anpassade fält som används i presentationen

Spara tid genom att kopiera och klistra in beräkningarna nedan.

>[!NOTE]
>
>Syntaxen för anpassade fältberäkningar har ändrats sedan presentationen gjordes 2019, men de begrepp och andra instruktioner som ges i presentationen är fortfarande korrekta.
>&#x200B;>**De beräkningar som ingår nedan har uppdaterats för att återspegla de senaste syntaxreglerna.**

**Första implementeringsdatum**

Format: Datum

Beräkning:

```
IF(ISBLANK({DE:First Commit Date}),{defaultBaseline}.{plannedCompletionDate},{DE:First Commit Date})
```

**Första varaktighet**

Format: Text

Beräkning:

```
IF(ISBLANK({DE:First Duration}),{defaultBaseline}.{durationMinutes},{DE:First Duration})
```

**Förhållande mellan arbete och implementering**

Format:Number

Beräkning:

```
ROUND(DIV({actualDurationMinutes},{DE:First Duration}),1)
```

**Status för förhållandet mellan arbete och implementering**

Format:Text

Beräkning:

```
IF({DE:Work-to-Commit Ratio}>2,"Terrible",IF({DE:Work-to-Commit Ratio}>1.6,"Poor",IF({DE:Work-to-Commit Ratio}>1.2,"Not Bad","Excellent")))
```

**Justerad hastighet**

Format:Number

Beräkning:

```
ROUND(DIV({actualDurationMinutes},{durationMinutes}),1)
```

**Justerad hastighetsstatus**

Format:Text

Beräkning:

```
IF({DE:Adjusted Velocity}>2,"Terrible",IF({DE:Adjusted Velocity}>1.6,"Poor",IF({DE:Adjusted Velocity}>1.2,"Not Bad","Excellent")))
```

## Frågor och svar

**Fråga**

Tack för att du har organiserat det här webbinariet. Jag har en fråga om Field i Workfront. I vårt system skapade vi ett anpassat fält med namnet &quot;State&quot; som är en kombination av Status och Condition. Det här fältet innehåller många statyer i tusen projekt, vilket är mycket viktigt för vårt dataextrakt i Tableau. Men nu vill vi ta bort det här fältet och använda villkorsfältet, det inbyggda fältet i stället. Har du någon aning om hur jag kan vända det här fältet utan att förlora data? Allt jag kan tänka mig att göra utan att förlora data just nu är att växla manuellt från projekt till projekt.

**Svar**

I en sådan här situation kan du använda filtrering och massredigering för att delvis automatisera besväret med att fylla i villkorsfältet baserat på ditt anpassade tillståndsfält.

Gör följande:

1. Avgör vilka lägesvärden du vill koppla till villkorsvärden. Anta till exempel att du har ett lägesvärde på&quot;Late&quot; och&quot;Mycket sen&quot; som båda mappas till villkorsvärdet&quot;In Trouble&quot;
1. Skapa en projektrapport som visar alla projekt med det statliga värdet&quot;Late&quot; och&quot;Mycket Late&quot;
1. Kör rapporten. Se till att du visar alla projekt (se alternativen längst ned till höger i rapporten)
1. Klicka på kryssrutan uppe till vänster i rapporten i fältet med kolumnrubriker. Då väljs alla projekt i rapporten
1. Klicka på knappen Redigera ovanför rapportlistan
1. Ställ in villkorstypen till Manuell
1. Ställ in fältet Villkor till I problem
1. Klicka på Spara ändringar


**Fråga**

Hur definieras Utmärkt, Inte dåligt osv.?

**Svar**

Det här var bara ett exempel, men så här ställer jag in det. Först beräknade jag två index:

Justerad hastighet

Formeln för detta är Faktisk varaktighet/planerad varaktighet (som lagras i fältet Varaktighet i ett projekt). Eftersom den planerade varaktigheten för projektet kan ändras varje gång projektet planeras om, representerar den planerade varaktigheten den slutliga planen.

Förhållande mellan arbete och implementering

Formeln är som Justerad hastighet förutom att vi i stället för att använda värdet för planerad varaktighet från den slutliga omplaneringen vill använda den planerade varaktighet som först utlovades till kunden. Vi antar att originalplanen innehåller denna information (och vi planerar att från och med nu be våra projektledare att planera sina projekt på det här sättet så att vi kan samla in korrekta data). Vi hämtade det här varaktighetsvärdet från den ursprungliga baslinjen och kallade det First Duration.

Genom att dividera Faktisk varaktighet med antingen Planerad varaktighet eller Första varaktighet får vi ett tal som kan tala om för oss hur nära det var att vi var på måfå. Om den planerade varaktigheten eller den första varaktigheten är lika med den faktiska varaktigheten kommer indexvärdet att vara 1. Om den faktiska varaktigheten är större blir svaret mer än 1. Ju fler desto värre blev det när vi mötte vår dejt.

Med tanke på allt jag bestämde mig för att tilldela status för både Justerad hastighet och Förhållande mellan arbete och implementering enligt följande:

* 1.1 eller under Jag heter Excellent.
* 1.2 till 1.5 Jag kallade Inte dåligt.
* 1.6 till 1.9 Jag kallade Dålig.
* 2 eller högre kallade jag Terrible.

**Fråga**

Vad behöver arbetaren göra för att hålla reda på hur lång tid det tar att utföra projekten?

**Svar**

Vi spårar inte hur många timmar som har ägnats åt att arbeta med projekten här. Vi håller bara på att spåra och jämföra varaktigheten. Men om du spårar timmar och vill använda faktiska timmar över planerade timmar för att beräkna hastigheten, kan du göra samma typ av rapportering genom att jämföra planerade timmar med faktiska timmar. Du vill även hämta planerade timmar från den ursprungliga baslinjen.

**Fråga**

Kan du ange filter som används för Snabb?

**Svar**

Jag använde två filterregler för rapporten Velocity:

* Kategorier >> ID > > Jämn >> WPI-projektdata (det här är det anpassade formuläret som innehöll alla beräknade fält. Jag vill bara se projekt som använder det här anpassade formuläret)
* Projekt >> Status > > Jämn >> Fullständigt (jag vill bara se färdiga projekt eftersom de har ett värde för Faktisk varaktighet som anger hur lång tid det tog att få allting gjort. Aktuella projekt ger inte en korrekt faktisk varaktighet för beräkning av hastighet)

Jag har också lagt till annan filtrering så att min rapport hålls tillräckligt liten för att kunna hanteras för webbinariet, men i din produktionsmiljö vill du förmodligen se alla projekt med det anpassade WPI-formuläret under en viss tidsperiod. Du kanske vill filtrera efter projektets faktiska slutförandedatum.

**Fråga**

Om du kopierar ett projekt, innehåller det samma baslinjer som det nya projektet?

**Svar**

Nej, baslinjerna inkluderas inte i det kopierade projektet

**Fråga**

För en process för godkännande av uppgifter, kan du visa mig hur man skapar en rapport som ger en åtkomsthistorik per uppgift i ett projekt med en tids-/datumstämpel för varje godkännare?

**Svar**

Skapa en aktivitetsrapport. Klicka på Lägg till kolumn på fliken Kolumner (Visa). I rutan &quot;Visa i den här kolumnen:&quot; skriver du &quot;Godkänn&quot;. Här visas olika godkännandefält som du kan rapportera om. Jag föreslår att du först lägger till en kolumn för allt (förutom eventuella ID:n). Sedan kan du se vilken information som visas.

Gå sedan till fliken Filter och lägg till en filterregel för:

Aktivitet >> Är godkännande > > Lika >> Sant. Detta visar endast uppgifter som har ett godkännande bifogat.

Lägg till ytterligare filter efter behov.

**Fråga**

Jag vill skapa en korrekturrapport. En lista över projekt som visar hur många korrektur de har och hur många versioner av det korrekturet som finns.

**Svar**

Skapa en dokumentrapport.

Versionsnumret visas i standardvyn. Du ska lämna det där, men du kan ändra alla andra kolumner.

Gruppera rapporten efter projektnamn.

Filtrera rapporten med aktuellt version :Proof-ID är inte tomt.

Då visas en lista med alla korrektur i varje projekt. Den får en rad för varje korrektur och versionsnumret (som blir detsamma som det totala antalet versioner) visas.

**Fråga**

Kan du använda snabbhet på aktivitetsnivå? I stället för på projektnivå?

**Svar**

Ja, men du måste kopiera det anpassade projektformuläret och skapa ett anpassat uppgiftsformulär från det. Därefter måste du redigera beräkningen i fältet Första implementeringsdatum och ändra referensen till &quot;Standardbaslinje&quot; till &quot;Standardbaslinjeaktivitet&quot;. Gör på samma sätt för Första varaktighet. Därefter kan du bifoga det anpassade aktivitetsformuläret till de uppgifter du vill mäta. Du måste skapa aktivitetsrapporter istället för projektrapporter för dessa. Du måste dock fortfarande se till att originalprojektbaslinjen är inställd som standardbaslinje. Alla aktivitetsdata lagras i samma baslinje som projektdata.

**Fråga**

Måste det första implementeringsdatumet anges manuellt av projektägaren? Eller kan det dra från befintliga fält?

**Svar**

Första implementeringsdatum hämtas från standardbaslinjen. Så länge som standardbaslinjen är den ursprungliga baslinjen visas det planerade slutförandedatumet för projektet vid den tidpunkt det först ställdes in på Aktuell status.

**Fråga**

Beräknade fält i anpassade formulär behöver fortfarande uppdateras regelbundet? Eller kommer det att ske automatiskt över natten (eller vid någon annan utlösare) nu?

**Svar**

Beräknade fält beräknas om:

* När en användare redigerar objektet
* Vid massredigering med aktiverade Omberäkna anpassade uttryck
* Ändringar i formuläret med alternativet Uppdatera tidigare beräkningar valt

**Fråga**

Om hastigheten överväger Varaktighet, ska Procent färdigt i projektinställningen baseras på Varaktighet?

**Svar**

Nej, alternativet Projektinställningar avser bara hur Procent färdigt beräknas. Varaktighetsvärdet påverkas inte av den här inställningen.

**Fråga**

Vad är skillnaden mellan den första varaktigheten och planens varaktighet?

**Svar**

Första varaktighet är antalet dagar som du ursprungligen lovade kunden som projektet skulle ta. Vi får det här numret från den ursprungliga baslinjen som spelades in när projektet ändrades från Planering till Aktuell.

Planerad varaktighet är antalet dagar från projektstart till planerat slutförandedatum. Inledningsvis är de här två varaktigheterna desamma, men om projektet någonsin planerats om och det planerade slutförandedatumet ändrats så var det den planerade varaktigheten också.

Värdet i Velocity-rapporterna beror på att vi kan se hur mycket den planerade varaktigheten har ändrats från den första varaktigheten. Vi kan se detta så långt tillbaka som när vi började spela in baslinjer när projekt ändrades från Planning till Aktuell.

**Fråga**

Kan du ange arbetare efter färg så att de är desamma i alla rapporter?

**Svar**

Om du grupperar efter Tilldelad till >> Namn i en uppgiftsrapport kan du tilldela en färg till vissa arbetare på fliken Diagram. Välj bara alternativet Egna färger bredvid rutan Tilldelad >> Namn på fliken Diagram och lägg till en färg för varje arbetare.

**Fråga**

Jag försöker avgöra om det är möjligt att skapa en kontrollpanel med ett område som tittar på ett anpassat formulär på aktivitetsnivå för att se om det finns och sekundär om vissa fält inte är tomma. Är detta möjligt?

**Svar**

Låt oss se om jag förstår din fråga. Anta att jag har ett eget formulär som heter Tammy-formulär med ett fält i det som heter Tammy Field.

Du vill ha en uppgiftsrapport som visar alla uppgifter som har bifogade Tammy-formulär och där Tammy-fält har något värde.

Ja, det kan du göra. Du behöver bara ett filter i uppgiftsrapporten med två filterregler:

Kategorier >> ID-formulär med samma Tammy-format

Aktivitet >> Manipulerat fält är inte tomt

**Fråga**

Finns det något sätt att skapa en rapport som söker efter ett specifikt namngivet dokument i dokumentbiblioteket? En del av kontrollpanelen vi vill mäta om vissa dokument finns.

**Svar**

Ja. Du måste skapa en dokumentrapport. Det låter som om du vill ange ett specifikt dokumentnamn varje gång du kör rapporten. Om så är fallet rekommenderar jag att du går till Rapportalternativ och väljer Rapportfrågor. Lägg till en fråga för Dokument >> Namn.

**Fråga**

Kan du välja en färg/ett hexadecimalt värde som inte finns med på diagramfliken, men som är en ny färg som är ett nytt hexadecimalt värde, till exempel en ny färg från mitt varumärke, så att jag kan anpassa rapporterna?

**Svar**

Ja, du kan ange valfri RGB-kod som du kan ha hittat. Det här är en standardkod som anger mängden rött, grönt och blått i färgen. Workfront kommer att acceptera ett hexadecimalt värde från 00000 till FFFFFF, så om du vet koden för din varumärkesfärg kan du använda den.

**Fråga**

Kan du ange definitionen av rapporterna på nytt på kontrollpanelen (ange vilka rapportåtgärder som ska vidtas)?

**Svar**

Statusdiagram för justerad hastighet

> Detta visar hur bra vi gjorde när vi slutförde projekt i tid när vi jämförde projektets faktiska varaktighet med den planerade varaktigheten. Den planerade varaktigheten har justerats eftersom projektet planerades om under dess livscykel.

Statusdiagram för förhållandet mellan arbete och implementering

> Detta visar hur bra vi gjorde när vi slutförde projekt i tid när vi jämförde projektets faktiska varaktighet med den första varaktigheten. Den första tidsperioden är den ursprungliga tid då vi lovade kunden att projektet skulle ta att slutföra. Den första varaktigheten beräknades från varaktighetsvärdet för projektet när det först ändrades från Planering till Aktuell status. Detta var den varaktighet som spelades in i den ursprungliga baslinjen.

Rapport över snabbstatuslista

> Den här rapporten innehåller alla beräknade anpassade fält och viktiga datum för samma projekt i diagrammen. Syftet är att vi ska kunna kontrollera våra beräkningar och få mer detaljerad information om så önskas.

**Fråga**

Hur lade du till nya data på x-axeln?

**Svar**

När du grupperar efter något i en rapport kan du skapa ett diagram. Sedan kan du ange X- eller Y-axeln på fliken Diagram.

**Fråga**

Kan du gå över skillnaden mellan första varaktighet och faktisk varaktighet?

**Svar**

Första varaktighet är antalet dagar som du ursprungligen lovade kunden som projektet skulle ta. Vi får det här numret från den ursprungliga baslinjen som spelades in när projektet ändrades från Planering till Aktuell.

Faktisk varaktighet är antalet dagar från det att ditt projekt har startats till det faktiska slutförandedatumet.

**Fråga**

Hur räknas projektets baslinjefaktor in i den här rapporten?

**Svar**

Projektets ursprungliga baslinje innehåller det planerade slutförandedatumet och den planerade varaktighet som fanns när projektet först ändrades till statusen Aktuell. Om processen var att planera projektet innan det ställdes in på Aktuell skulle detta motsvara det datum då du åtagit dig att slutföra projektet senast.

**Fråga**

Finns det något sätt att masstillämpa det nya formuläret på gamla projekt?

**Svar**

Ja, du kan välja flera projekt i en lista. När du gör detta visas alternativet &quot;Redigera&quot; längst upp till vänster i listan. Om du klickar på Redigera när flera objekt är markerade hamnar du i det vi kallar&quot;massredigering&quot;. Du kan lägga till ett anpassat formulär i flera projekt på det här sättet.

En genväg för att lägga till anpassade formulär i ett stort antal projekt är att skapa en rapport som du filtrerar så att den bara innehåller de projekt du vill använda. I stället för att välja projekt var för sig klickar du bara på kryssrutan ovanför den första kryssrutan i listan så markeras hela listan.

**Fråga**

Går det att ta bort dubblettposter från grupperingen i en uppdragsrapport, men inte mellan grupperingar?

**Svar**

Det bästa sättet att tänka på grupperingar i listor är följande:

Först styr du vilka objekt som ska visas i listan på fliken Filter. Det kommer inte att finnas några dubblettposter. Filtret tillämpas på varje objekt. Om den passerar genom filtret visas den en gång i listan, om den inte syns alls.

Nästa gruppering används för den filtrerade listan. En gruppering identifierar en sak om objekten i listan, till exempel namnet på portföljen som den ingår i (du kan inte gruppera objekt i en lista, bara på en sak). Därefter visas alla objekt med samma värde i den grupperingen, precis som alla projekt i samma portfölj. Alla projekt som inte har en vald portfölj visas i grupperingen med namnet&quot;Inget värde&quot;.

Därför finns det ingen möjlighet att några objekt kan visas i fler än en gruppering. Och om ett objekt alls visas i listan styrs helt av filtret (och om personen som kör rapporten har behörighet att visa det).

**Fråga**

Skulle du rekommendera någon annan rapport för att spåra hastighet? Bara en högnivårekommendation är bra eftersom jag vet att det inte finns tillräckligt med tid att gå igenom detaljerna.

**Svar**

Precis som med andra rapporter måste du först bestämma vad du vill veta. Nästa steg är att komma åt informationen, vilket i vissa fall innebär att du måste börja spåra den.

En anledning till att jag valde att jämföra den faktiska varaktigheten med två typer av planerad varaktighet var att jag tyckte att den gav intressanta insikter om hastigheten. Informationen fanns också tillgänglig, så jag behövde inte börja spåra den. Med några beräkningar kan jag extrahera data i ett formulär som jag kan rapportera om.

Men du kan lika gärna hålla reda på annan information om uppgifter eller projekt som ska rapporteras.

Workfront har inga inbyggda snabbhetsrapporter, så jag rekommenderar dig och ditt team att brainstorm på det ni vill veta för att avgöra snabbheten och sedan se vad ni behöver spåra.

**Fråga**

Kan du beräkna något på COLUMN-nivå? Istället för att anropa ett beräknat FÄLT från ett anpassat formulär?

**Svar**

Det skulle ha varit möjligt att använda ett värdeuttryck i textläge för att utföra dessa beräkningar. Vi kunde inte ha gjort First Duration eller First Commit Date, men vi behövde fånga dem där de inte skulle ändras.

När det gäller förhållandet mellan arbete och implementering och den justerade hastighetsstatusen behövde dessa fält vara anpassade så att vi kunde använda dem på fliken Diagram. Fliken Diagram känner inte igen grupperingar i textläge, de måste vara anpassade fält. Och eftersom vi behövde Work-to-Commit Ratio och Adjustment Velocity för att beräkna dessa statusvärden behövde vi även dessa anpassade fält. I det här fallet behövde de alla vara anpassade fält, men det är alltid bra att fundera över båda sätten och välja vad som skulle fungera bäst. Tack för frågan.

**Fråga**

Våra projekt förändras ofta på grund av att kunderna blir försenade eller förändras genomgående. Vår rapport kan visa allt som&quot;fruktansvärt&quot;. Vad är en rekommendation för att spåra orsaker till ändring? Vi funderade på att lägga till ett anpassat formulär på dokumentnivå som rapporterar orsaken till ändringen (antingen intern eller klientändring), men undrar vad som är bäst.

**Svar**

Det bästa sättet är att använda en listruta för att spåra detta. Lägg in så många &quot;anledningar&quot; som du kan tänka dig att börja med och lägg sedan till ett &quot;annat&quot; alternativ för att fånga en anledning som inte finns med i listan. Om den nya anledningen ser ut eller blir vanlig lägger du till den i listrutan. Du kan enkelt rapportera om saker i en nedrullningsbar lista och du kan gruppera det här fältet (du kan inte gruppera i kryssrutor eller i en flervalslistruta).

Bara en kommentar till. Du kanske inte vill inkludera alla projekt i dina Snabbrapporter. Om du ska fixa buggar eller&quot;gå dit ingen har gått tidigare&quot; gör du antagligen inte samma typ av åtagande till ett slutdatum som om du bygger ett hus som du har byggt många gånger tidigare.

Se till att ni lägger in snabba rapporter där det kan hjälpa er att uppnå era mål.

**Fråga**

Om jag ställer in standardbaslinjen för ett projekt till &quot;Original&quot; och sedan tar ut projektet från aktuell och sätter det tillbaka i aktuell version, kommer det då att ändra standardbaslinjen?

**Svar**

Ja. Varje gång du ändrar statusen till Aktuell får du en ny baslinje och den blir den nya standardinställningen. Alla tidigare baslinjer finns dock kvar och du kan manuellt ange den ursprungliga baslinjen som standardbaslinje igen.

**Fråga**

Finns det något sätt att i en rapport ange vilka fält som kan redigeras? Kan jag ange begränsningar för vissa fält?

**Svar**

Du kan begränsa behörighet att visa och redigera fält i ett anpassat formulär. Du måste inkludera fälten i ett avsnitt, och i avsnittsinställningarna kan du välja vilka rättigheter som krävs för att användare ska kunna visa eller redigera fält i avsnittet.

**Fråga**

Kan du skapa en rapport som söker efter ett specifikt namngivet dokument i dokumentbiblioteket?

**Svar**

Ja. Du måste skapa en dokumentrapport. Det låter som om du vill ange ett specifikt dokumentnamn varje gång du kör rapporten. Om så är fallet rekommenderar jag att du går till Rapportalternativ och väljer Rapportfrågor. Lägg till en fråga för Dokument >> Namn.

**Fråga**

Varför är värden tillgängliga som kolumner men inte tillgängliga för markering eller gruppering i rapporter. Exempel: Utgåva Source.

**Svar**

Huvudanledningen till att en kolumn kan visas, men inte är tillgänglig för gruppering, är att den kan innehålla en lista, som en kryssruta för anpassade fält eller uppgiftstilldelningar. Gruppering på en lista är inte tillåten.

**Fråga**

Hur kan jag separera i en rapport (med vilka fält) när hennes inmatning gjordes och när timmarna faktiskt utfördes?

**Svar**

Fältet Ingångsdatum för objektet Timme hänvisar till datumet då timmarna bearbetades. Detta gör att inmatningsdatumet skiljer sig från andra objekt, där det innebär det datum då objektet skapades. Även om det inte finns något datum att skapa för timmar finns det ett &quot;Senast uppdaterat den&quot;, som är det första datumet som skapades och sedan redigerades timmen därefter.

**Fråga**

Hur kommer vi åt baslinjedata ur en rapportsynpunkt? Jag har ett projekt med flera baslinjer. Jag vill se hur enskilda uppgifter planerades i varje baslinje. Finns det något sätt att skriva en rapport som visar projektplanen för varje baslinje?

**Svar**

En rapport visar vilka fält som du vill se för baslinjen som är inställd som standard, så att du kan ändra baslinjen och uppdatera rapporten för att se fält med den nya baslinjen.

Men om du vill se grafisk information om dina uppgifter kan du göra det med funktionen Gantt-schema. Aktivera Gantt i en uppgiftslista (med Gantt-ikonen i det övre högra hörnet bredvid Spara automatiskt), gå till inställningsikonen precis nedanför och till höger och klicka på det. Markera rutan Baslinje så visas alla baslinjer. Du kan markera dessa i taget och se ändringarna i dina uppgifter i Gantt-vyn.

**Fråga**

Så här skapar du en rapport för att hitta statusändringarna för en definierad period, till exempel förra månaden.

**Svar**

Med Analytics-funktionen i Workfront kan du snabbt visa historiska data, inklusive statusändringar.

Men du kan också hämta information om statusändringar med en anteckningsrapport. Du kan filtrera så att du kan se statusändringar för projekt om du spårar fältet Projektstatus.

Gå till Inställningar > Gränssnitt > Uppdatera feeds och kontrollera att Projektstatus är ett av de inbyggda fälten som spåras. Om det inte är det måste du lägga till det.

Skapa nu en anteckningsrapport och gör följande:

På fliken Kolumner (Visa):

* Ersätt kolumnen &quot;Anteckningstext&quot; för &quot;Granskningstext&quot;. Detta visar information om vad statusen ändrades från och till
* Lämna kolumnerna &quot;Projekt: Namn&quot; och &quot;Inmatningsdatum&quot;
* Klicka på kolumnen Ingångsdatum och markera sedan Sortera efter den här kolumnen på panelen Kolumninställningar. Om du vill se de senaste statusändringarna sorterar du dem i fallande ordning.

På fliken Grupperingar:

* Gruppera efter projekt: Namn

Skapa följande filterregler på fliken Filter:

* Obs >> Granskningstyp >> Jämn >> Statusändring
* lägg till ytterligare regler som ska filtreras efter Anteckningens anmälningsdatum. Du kanske vill utelämna detta i Filter och använda en rapportfråga i stället
* Filtrera på projekt, portfölj eller andra data efter behov.

**Fråga**

Som planerare kan du skicka rapporter till andra användare?

**Svar**

Med en plan kan du skapa rapporter och dela dem med andra användare, även med personer som inte är användare. När du visar rapporten går du till Rapportåtgärder > Delning och klickar sedan på kugghjulsikonen i det övre högra hörnet av rutan Rapportåtkomst. Välj&quot;Gör detta offentligt för externa användare&quot;. alternativ. Du kan kopiera länken och skicka den till vem som helst. De kommer att se rapporten i realtid i sin webbläsare.
