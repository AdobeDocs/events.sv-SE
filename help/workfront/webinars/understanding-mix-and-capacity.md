---
title: Fråga experten - Förstå blandning och kapacitet
description: Lär dig att mäta blandning och kapacitet inom företaget. Det här webbinariet spelades in den 2 oktober 2019.
doc-type: feature video
team: Technical Marketing
kt: 9913
exl-id: 49cce53f-457b-4973-a0d9-1b5ce2272884
duration: 4239
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '2230'
ht-degree: 0%

---

# Fråga experten - Förstå blandning och kapacitet

Lär dig att mäta blandning och kapacitet inom företaget. Det här webbinariet spelades in den 2 oktober 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341119/?quality=12)

## Frågor och svar

**Fråga**

Hur placerar du %s i ett kolumndiagram?

**Svar**

De procentvärden som anges i Mix-rapporten fanns där eftersom vi på fliken Diagram valde Gruppera kolumner och Staplade till 100 %. Om vi väljer Staplad visas de planerade timsummorna och inte procenten.

**Fråga**

Om din arbetsinsats är en blandning av projekt/uppgifter och ärenden/förfrågningar, hur rekommenderar vi att du får en högnivågranskning (i en Workfront-rapport) av en WPI.

**Svar**

Projekt, uppgifter och ärenden måste ha sina egna rapporter med sina egna anpassade formulär. De kan dock använda samma arbetstypfält. Du kanske vill visa de tre rapporterna på en kontrollpanel.

**Fråga**

Måste vi gruppredigera uppgifter för att göra dem operativa eller strategiska?

**Svar**

Tekniken vi föreslår är att skapa en rapport som gör det möjligt att få en lista över åtgärder som är operativa. När du har markerat alla uppgifter samtidigt kan du redigera dem gruppvis och sedan bifoga det anpassade formuläret med arbetstypen Arbetstyp och ange arbetstypen till Använd för alla uppgifter samtidigt. Du följer samma procedur för att samla in en lista över strategiska uppgifter, redigera dem gruppvis och lägga till det anpassade formuläret, osv.

Det finns några idéer i webbinariet om anpassade uppmaningar som kan hjälpa dig att få en lista, som att kontrollera om det finns vissa ord i uppgiftsnamnet, projektägaren, portföljen eller tilldelade användare. Det här är bara idéer. Ni bör ta fram en rapport som fungerar bäst i er situation.

**Fråga**

Om jag har fyra kategorier i min mix, kan jag skapa ett mål för varje och sedan rapportera om deltavärden mellan prognos och plan jämfört med faktisk? (fyra kategorier: Campaign, Business Unit, Web och Product). Vi har kategorierna på projektnivå i anpassade formulär/fält. Målet skulle vara att skapa en kvartalsprognos (budget/prognos) och sedan följa upp planerade timmar i den riktningen och slutligen faktiska.

**Svar**

Om du har alla kategorier i ett anpassat fält (vi kallar det Arbetstyp för tillfället) skapar du bara en projektrapportgruppering på Planerade timmar först och Arbetstyp sedan. Filtrera projektrapporten så att projekt i Planning visas inom önskade datumintervall. Använd ett diagram med grupperade staplar eller staplar som är staplade på 100 % om du vill se procentandelar. Det här kan vara din prognosrapport.

Du kan kopiera rapporten och redigera den för att skapa en rapport baserad på aktuella projekt, och ändå visa blandningen baserat på planerade timmar.

Du kan kopiera rapporten igen, ändra den till att gruppera efter faktiska timmar i stället för efter planerade timmar och endast visa slutförda projekt inom önskade datumintervall. Då visas procentmixen baserat på faktiska timmar.

**Fråga**

Fungerar detta om du har flera kategori-ID:n för ett projekt eller en uppgift?

**Svar**

Ja, om du har flera ID:n måste de separeras med en flik, enligt följande:

```
EXISTS:1:$$EXISTSMOD=NOTEXISTS
EXISTS:1:$$OBJCODE=OBJCAT
EXISTS:1:categoryID=5d76d82600e7926bb51eeb1e0886810e 5d54288d01034619f2eb2c74f6472f18
EXISTS:1:objID=FIELD:ID
```

Det bästa sättet att separera dem med ett tabbtecken är att först skapa en lista med kategorier i verktyget. Om du lägger in flera anpassade formulärnamn och växlar till textläge visas de som ID:n som avgränsas med tabbar.

Flera ID:n behandlas som ELLER:n, så om någon av dem är kopplad till uppgiften visas den inte i rapporten.

**Fråga**

Frågar rapporten&quot;ANDed&quot; eller&quot;ORed&quot;?

**Svar**

De enskilda anpassade prompterna är&quot;ANDed&quot;. Om du anger Pam som projektägare och Faktura som tilldelad till uppgiften, kommer du bara att se uppgifter som tilldelats Faktura i projekt där Pam är projektägare.

**Fråga**

Varför kan du bara sortera efter vissa kolumner? Du kan alltså inte sortera efter uppdrag.

**Svar**

&quot;Uppdrag&quot; är en lista och du kan inte sortera eller gruppera objekt i en lista. Du kan bara sortera eller gruppera ett enskilt objekt.

För att illustrera poängen kan du föreställa dig en lista med uppdrag som detta för en uppgift:

```
Jane
Bill
Dan
```

Och en lista över tilldelningar som detta för en annan uppgift:

```
Bill
Jane
Helen
```

Vilken uppgift ska visas först i en sortering? Du kan säga &quot;sortera efter förnamnet i listan&quot;, men det är inte nödvändigt eftersom du inte kan styra ordningen. Workfront undviker problemet genom att inte tillåta dig att sortera efter listor.

Gruppera efter lista, då? Om vi kunde gruppera efter en lista med namn, skulle du hitta alla uppgifter som tilldelats Jane, Bill, Dan grupperade tillsammans och alla uppgifter som tilldelats Jane, Dan, Bill (samma lista, men i en annan ordning) i en annan gruppering. Workfront undviker problemet genom att inte tillåta gruppering efter listor.

**Fråga**

Används planerade timmar för strategiska uppgifter och faktiska timmar för drift?

**Svar**

Nej. I vårt exempel använder vi Planerade timmar för att visa den planerade ansträngningsnivån för både strategiska och operativa uppgifter. På så sätt kan vi enkelt jämföra dem, oavsett om de har förekommit tidigare, idag eller i framtiden. Du kan också använda faktiska timmar för att jämföra strategiska och operativa uppgifter, men bara för uppgifter tidigare eftersom faktiska timmar är de timmar som användarna har rapporterat som den tid de faktiskt arbetade med uppgifterna.

**Fråga**

Hur redogör vi i resursplaneraren för aktiviteter som planerats tidigare men inte slutförts? De planerade timmarna verkar inte gå framåt och visas därför inte i kommande veckor som aktiviteter/timmar som behöver resurser.

**Svar**

Det finns ingen &quot;automatisk&quot; övergång till ej slutfört arbete. Du måste planera om projektet när det händer. Resurserna som du ursprungligen tilldelat en viss uppgift kanske inte är tillgängliga inom den nya tidsramen, så projektledaren måste titta på detta och bestämma det bästa sättet att planera om. Detta kan innebära att intressenter måste delta och att de kan godkänna ändringarna i planen.

**Fråga**

I stället för att ange 2 timmar/dag för att kontrollera e-post, brytningar, rekommenderar du att du justerar deras heltidsanställda?

**Svar**

Ja, om du ställer in FTE på 0,75, som visar att användaren är tillgänglig 6 timmar per dag i Resursplaneraren. Det här blir deras tillgänglighet varje dag. Om du vill visa dem som otillgängliga för olika perioder beroende på datumet, t.ex. inte tillgänglig den sista dagen i varje kvartal, är ett kostnadsfritt projekt ett sätt att göra detta.

En del föredrar allmänna projekt eftersom de kan skapa dem själva och ändra dem när de vill, medan de kanske inte har rätt att redigera sina egna heltidsanställda.

**Fråga**

Är data för kontrollpanelen för team-kapacitet tillgängliga för alla som delar rapporten, oavsett vilka behörigheter de har för arbetet?

**Svar**

Om en användare inte har behörighet att visa objektet visas det inte i rapporten/kontrollpanelen. Om du vill att alla ska se samma resultat kan du gå till Rapportåtgärder > Redigera > Rapportinställningar och ange&quot;Kör den här rapporten med åtkomsträttigheter för&quot; i fältet. På så sätt kan de användare som är delade i den här rapporten se exakt vilka resultat du ser. De får inte ytterligare åtkomst till själva resultatet, så vissa resultat kan vara klickbara eller inte klickbara.

**Fråga**

Hur skapar vi en rapport som visar all personal som är tilldelad ett projekt totalt (inte på aktivitetsnivå)?

**Svar**

Du kan skapa en kolumn i en projektrapport som visar alla användare som listas som en del av personalfliken (Projektgrupp). Du vill använda följande textläge:

```
displayname=Project Team
listdelimiter=<p>
listmethod=nested(projectUsers).lists
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

**Fråga**

Jag skulle vilja ha en rapport/kontrollpanel som innehåller hur mitt team fungerar. Särskilt följande scenarier: - Projekt jag äger / Projekt skapade för mig / Uppgifter tilldelade till andra / Uppgifter tilldelade mig

**Svar**

Projekt jag äger

Det finns en inbyggd rapport med namnet&quot;Aktuella projekt&quot; som visar alla aktuella projekt. Du kan redigera det här projektet och lägga till en filterregel: Projekt > Ägar-ID > Lika > $$USER.IDTpara sedan rapporten och döp om den till&quot;Projekt jag äger&quot;.

Projekt skapade för mig

Det finns en inbyggd rapport med namnet&quot;Mina projekt&quot; som visar alla aktuella projekt som du är i projektteamet (vilket innebär att du är ägare, sponsor eller tilldelad till uppgift). Du vet inte om det är det du frågar efter, men det finns inga andra sätt att veta om någon har skapat ett projekt åt dig förutom att du har blivit projektägare, sponsor eller tilldelat dig en uppgift.

Uppgifter som jag har tilldelat andra

Skapa en aktivitetsrapport med de filter du vill ha, gå sedan till fliken Filter och klicka på Växla till textläge. Lägg till den här koden i det som redan finns:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Då visas alla uppgifter där den inloggade användaren har tilldelat minst en av de aktuella tilldelningarna. Om flera personer har tilldelat tilldelningar visas endast namnet på den första personen som tilldelade någon som&quot;Begärd av&quot; på startsidan för uppgiften. Om du vill se alla personer som har tilldelats och som har tilldelat var och en av dem, kan du lägga till en kolumn i vyn, växla till textläge och ersätta det som finns där med det här:

```
displayname=All Assignees and Requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

Uppgifter som tilldelats mig

Det finns en inbyggd rapport med namnet&quot;Mina uppgifter&quot; som visar alla ofullständiga uppgifter i Aktuella projekt där du är aktivitetsägare. Jag föreslår att du ändrar filtret så att du kan se alla uppgifter där du är en av de många användare som har tilldelats, inte bara aktivitetsägaren. Det gör du genom att ta bort filterregeln

```
Task > Assigned To ID > Equal > $$USER.ID 
```

och ersätta den med

```
Assignment Users > ID > Equal > $$USER.ID
```

**Fråga**

Finns det något sätt att anpassa etiketter i diagram? Jag har upptäckt att när jag skapar ett diagram som återspeglar projektstatus så inkluderas hemgruppens namn i etiketten.

**Svar**

Etiketter i diagram använder fältnamnet för det du grupperar i. Det enda sättet att ändra etiketter är alltså att använda ett beräknat anpassat fält med vilket namn du vill. I beräkningsavsnittet i fältet anger du fältnamnet för det inbyggda fältet som du vill gruppera efter.

**Fråga**

Hur kodar du rapportfälten på Chuck&#39;s Team Assignements? Gammal bakom, röd för sent och grön i tid? Kan du även ändra ordningen så att den blir mer logisk, t.ex. röd/gul/grön eller tvärtom?

**Svar**

Om du vill ändra de färger som används i rapporten för alternativen för statusstatus redigerar du rapporten och klickar på fliken Diagram. Leta efter listrutan Egna färger >. Den visas intill rutan &quot;Vänster (Y) axel&quot; eller rutan &quot;Gruppera data efter&quot;, beroende på om du väljer att gruppera staplar eller stolpar eller inte. I den listrutan kan du välja färger. Om du klickar på siffrorna i det nedre högra hörnet av färgalternativen kan du välja färg från en större palett.

Tyvärr kan du inte ändra ordningen på dessa.

**Fråga**

Kan du skapa ett diagram där det pekar på antalet projekt som en arbetare har tilldelats en uppgift inom?

**Svar**

Ja, så här:

* Skapa en projektrapport
* Om användaren i fråga är inloggad användare ska filtret innehålla följande rad:

```
   Project Users > ID > Equal >$$USER.ID 
```

* Om inte, placerar du användarnamnet i stället för [!DNL $$USER.ID]. Detta visar alla projekt där den här personen har tilldelats en uppgift eller är ägare eller sponsor. Om du bara vill se projekt där de har tilldelats uppgifter ska du lägga till följande två filterregler:

```
   Project > Owner ID > Not Equal > $$USERID
   Project > Sponsor ID > Not Equal > $$USERID
```

* Skapa minst en gruppering så att du kan skapa ett diagram. Gruppera på vad som helst, som företag. Klicka sedan på fliken Diagram och välj ett diagram. &quot;Antal poster&quot; används som standard för en axel. Detta är antalet projekt som användaren har ett uppdrag i.

När en användare tilldelas ett uppdrag i ett projekt (som tilldelats en aktivitet eller projektägare eller projektsponsor) läggs den personen till i projektteamet och kan visas på fliken Anställning under underfliken Personer. Om en användare tas bort från att vara projektägare, sponsor eller ha några aktivitetstilldelningar är hans/hennes namn fortfarande kvar i projektteamet. Den måste tas bort manuellt om du vill ta bort den. Tänk på att detta kan påverka rapportresultatens exakthet. Om du vill ta bort någon från projektteamet går du till Anställning > Personer, markerar personen eller personerna och klickar sedan på knappen Ta bort som visas ovanför listan.

**Fråga**

Hur kan du ändra den fallande ordningen för en kolumn i textläge (i en gruppering)?

**Svar**

Du kan välja att sortera de flesta kolumner på fliken Kolumner (Visa) när du skapar en rapport. Då sorteras hela listrapporten om du inte har några grupperingar. Om du har grupperingar sorteras de efter det valet inom varje gruppering.

**Fråga**

Hur skapar jag en kolumn som identifierar gruppmedlemmar som tilldelats en godkännandefas?

**Svar**

Om du kör en uppgifts- eller ärende-/begäranderapport finns det en kolumn i Report Builder som heter &quot;Godkännare och status&quot; som hämtar den här informationen.
