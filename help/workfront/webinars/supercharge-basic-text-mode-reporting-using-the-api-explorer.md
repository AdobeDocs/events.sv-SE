---
title: Fråga experten - Utnyttja grundläggande textlägesrapportering med API-utforskaren
description: Lär dig mer om API-utforskaren, hur du använder den och hur du förbättrar dina rapporter med hjälp av det grundläggande textläget. Det här webbinariet spelades in den 22 januari 2020.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9918
source-git-commit: edd0bdb28a9b3d065a64a95af6a216b747577c77
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 2%

---

# Fråga experten - Utnyttja grundläggande textlägesrapportering med API-utforskaren

Lär dig mer om API-utforskaren, hur du använder den och hur du förbättrar dina rapporter med hjälp av det grundläggande textläget. Det här webbinariet spelades in den 22 januari 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341124/?quality=12)

## Ytterligare resurser

![Ett diagram med exempel på kodrader i textläge](assets/text-mode-chart.png)


**Slutlig kolumn för alla jobbroller**

```
description="Primary =" indicates the user's primary job role
displayname=All Job Roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("Primary = ",{role}.{name}),{role}.{name})
valueformat=HTML
```

**Textläge för kolumnen&quot;Alla team&quot;**

```
displayname=All Teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

**Textläge för kolumnen&quot;Alla grupper&quot;**

```
displayname=All Groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

**Textläge för kolumnen&quot;Direktrapporter&quot;**

```
displayname=Direct Reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

## Frågor och svar

**Fråga**

Går det att använda en samling i en rapport i textläge?

**Svar**

Ja, du kan använda vilket objekt som helst i samlingsområdet. Du kommer att vilja utforska och se vad du har tillgång till. Allt har inte åtkomst till både användarobjektet och jobbrollsobjektet som vi såg med användarrollsobjektet i API-utforskaren.

**Fråga**

Kan du diskutera villkorlig användning av olika samlingar i samma kolumn (projektuppdateringar eller aktivitetsuppdateringar)?

**Svar**

När du är i iterationsområdet och ser värdefältet eller värdeuttrycket där, används ett av objekten i samlingslistan. Med hjälp av värdefältet kan vi hämta namnet på den jobbrollen, till exempel, eller något som finns i det objektet i listan. Om du arbetar med en uppgift kan ett uppgiftsobjekt referera till det projekt som aktiviteten ingår i.

**Fråga**

Kan du diskutera om&quot;insamling av aktivitetsuppdateringar endast är möjlig i en uppgiftsrapport?&quot;

**Svar**

När du skapar en problemrapport kan du se aktivitetsinformation om problemet har rapporterats för aktiviteten, och du kan också se den informationen inifrån samlingen. Förutom i de här fallen måste du vara i en uppgiftsrapport för att kunna se data för uppgiftsinsamling.

**Fråga**

Kan du dela textformat ([!DNL CSS])?

**Svar**

Workfront stöder inte [!DNL CSS] i textläge.

**Fråga**

Vilket är det bästa och snabbaste sättet att hitta ett eget fältnamn - för textlägesrapportering? Jag har använt redigeringsalternativet HTML i webbläsaren ELLER genom att lägga till ett fält i en rapport och växla till textläge för att ta tag i det MEN.. nyfiken hur andra gör detta

**Svar**

Jag hittar det snabbaste sättet att markera fältet i användargränssnittet, växla till textläge och kopiera fältnamnet. Detta garanterar att jag får rätt stavning för fältet.

**Fråga**

Hur kan jag använda textläge för att identifiera medlemmar i ett team i en rapport? Vi använder för närvarande grupptilldelningar i arbetsflöden för godkännande av uppgifter och vill lista gruppmedlemmarna i den aktuella godkännandefasen i en kolumn som liknar hur fältet Godkännare och status fungerar.

**Svar**

För att kunna referera till de teammedlemmar som är kopplade till det aktuella godkännandesteget måste du referera till en samling med en refererad samling, vilket för närvarande inte är möjligt med Workfront textlägesfunktioner. Den kolumn som din organisation använder för närvarande visar vilket team som är kopplat till godkännandet som är ditt bästa alternativ.

**Fråga**

Måste fältet och objektnamnet vara i rätt skiftläge (t.ex. roll jämfört med roll)?

**Svar**

När du refererar till objekt i textläge måste du skriva det exakt som den högra kolumnen i API-utforskaren visar. Om du till exempel vill referera till ett projektnamn från en aktivitetsrapport ser värdefältet ut så här:

```
valuefield=project:name
```

När det gäller problem kallas de dock opTasks i API Explorer. Om du kör en timrapport och vill lägga till en kolumn för Issue name ser värdefältet ut så här:

```
valuefield=opTask:name
```

**Fråga**

Jag vill skapa en rapport som för varje projekt visar vilka aktiva uppgifter som bearbetas. Hur skulle jag bäst göra det? Jag antar att det skulle vara en uppgiftsrapport som även innehåller kolumner med projektinformation tillagda?

**Svar**

Det stämmer. En uppgiftsrapport är bäst för detta. Du måste definiera&quot;Aktiva uppgifter&quot;. Om du använder föregångare är detta en uppgift som är klar. Du kan alltså filtrera med Ready = True. Då kommer alla uppgifter som är klara att börja att utföras. Sedan rekommenderar jag att du grupperar efter projektnamn så att alla dina uppgifter grupperas tillsammans och du ser snabbt vilka uppgifter som tillhör vilket projekt.

**Fråga**

Finns det något sätt att skapa rapporter som beräknar data, till exempel procent av projekt som uppfyller vissa kriterier?

**Svar**

Det bästa sättet att skapa en rapport för att presentera eller beräkna data (% till exempel) är att använda grupperingar i rapporten och sedan använda ett diagram. Om du vill lägga till ett cirkeldiagram i rapporten kan du välja att cirkelsegmenten ska vara i värden eller i procent.

**Fråga**

Kan du använda textläge för att identifiera medlemmar i ett team som har tilldelats till den aktuella fasen för godkännande av uppgifter som liknar kolumnen Godkännare och Status?

**Svar**

Du måste lägga till en samlingskolumn i textläge i aktivitetsrapporten med följande:

```
displayname=Current Approval Stage Approvers 
listdelimiter=<p> 
listmethod=nested(currentApprovalStep.stepApprovers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

**Fråga**

Kan du filtrera där alla grupper innehåller en viss grupp?

**Svar**

Om du vill filtrera objekten i rapporten gör du det på rapportens filterflik. Om du bara vill se användare där en av grupperna var Redovisning, lägger du till en filterregel som säger:

```
Other Groups>ID>Equal>Accounting
```

**Fråga**

Finns det något sätt att skapa en rapport som avgör den faktiska varaktigheten för en kombination av uppgifter?

**Svar**

Du måste filtrera rapporten så att den bara innehåller den kombination av uppgifter som du vill ha. Sedan måste du placera en kolumn för faktisk varaktighet i vyn och sammanfatta den med Summa i kolumninställningarna, och slutligen måste du gruppera rapporten på något sätt. När du kör rapporten visar grupperingsfältet summan av de faktiska varaktigheterna i de rader som grupperas.

**Fråga**

Finns det något sätt att ta bort uppgifter som faller under en överordnad för att bestämma varaktigheten för resten av uppgifterna under en överordnad?

**Svar**

Längden på en överordnad aktivitet beräknas genom att subtrahera startdatumet för den tidigaste startuppgiften från slutdatumet för den senaste slutuppgiften under den överordnade aktiviteten. I en rapport vet du bara om varje enskild uppgift som är under övervägande, vare sig den ska visas eller inte. Rapportmotorn kan inte längre låsa sig till information från en uppgift och använda den när du tittar på en annan uppgift. Det enda sättet att uppnå det du vill är att ta bort en uppgift från att vara under en viss överordnad i projektuppgiftslistan och observera hur varaktigheten för den överordnade aktiviteten beräknas om.

**Fråga**

För villkorsstyrda grupperingar är en anpassad form (tänk&quot;Västerstater&quot;,&quot;Centralstater&quot;,&quot;Östra stater&quot;) för att avkoda de enskilda grupperna en vanlig teknik som fungerar bra med den anteckningen, när rekommenderar du att använda beräknade grupperingar eller beräknade parametrar?

**Svar**

Beräknade grupperingar (även kallade värdeuttryck i en gruppering) är ett bekvämt sätt att få resultat att visa i grupperingsfältet. Detta kan även göras med ett beräknat anpassat fält. Det finns fördelar och nackdelar för varje tillvägagångssätt, som är:

* Värdeuttryck beräknas varje gång webbläsarsidan uppdateras. Det här kan vara bättre än beräknade anpassade fält som beräknas om när objektet de är kopplade till redigeras, när beräkningsfälten beräknas om i en gruppredigering eller när det anpassade formuläret redigeras och alternativet Uppdatera tidigare beräkningar är markerat.
* Värdeuttryck kan dock inte användas i diagram, villkorsstyrd formatering eller filter. Du måste använda beräknade anpassade fält för dessa.

**Fråga**

Finns det inget sätt att ändra grupperingens visningsnamn från &quot;Inget värde&quot; till något annat som vi väljer att anropa för rapportering? d.v.s. alltid &quot;Inget värde&quot;?

**Svar**

Det finns ett sätt att ersätta&quot;Inget värde&quot; med något annat. Anta att du har en projektrapport grupperad efter Portfolio-namn. Alla projekt som inte är tilldelade till en portfölj hamnar i en gruppering med titeln:

```
Portfolio: Name: No Value
```

Om du vill ändra detta redigerar du grupperingen i textläge och ersätter den här raden:

```
group.0.valuefield=portfolio:name
```

med den här raden:

```
group.0.valueexpression=IF(ISBLANK({portfolio}.{name}),"Not in any Portfolio",{portfolio}.{name})
```

Grupperingen kommer nu att ha följande namn:

```
Portfolio: Name: Not in any Portfolio
```

**Fråga**

Finns det någon parameter för att spåra ofullständiga tilldelningar, t.ex.:

1. Aktiviteter med ett enstaka uppdrag som inte tilldelats en person, eller
1. Uppgifter med flera tilldelningar som har minst en ej tilldelad person för de begärda rollerna

**Svar**

Detta kan åstadkommas med hjälp av en uppdragsrapport och filtrering för

```
Assigned To ID > Is Blank and Role ID > Is Not Blank
```

Detta kommer att leda till alla uppgifter eller problem som har tilldelats en roll, men inte nödvändigtvis en viss användare. Du måste lägga till kolumnerna för Uppgift och Utgåva för att se vilket objekt uppdraget tillhör, och om det grupperas efter Projektnamn bör det hjälpa till att hålla ordning på det.

**Fråga**

Chuck, jag glömmer, men minns du egenskapen i textläge som sedan återges som en verktygstips när du hovrar?

**Svar**

description= gör att du kan visa ett verktygstips när du hovrar över kolumnrubriken.

**Fråga**

Kan jag rapportera i ett kryssrutefält som tillåter flera val, men bara dra det första urvalet till rapporten?

**Svar**

Ja. De valda alternativen i kryssrutefältet finns alla i en sträng där varje markering avgränsas med kommatecken. Du använder SEARCH-uttrycket för att hitta positionen för det första kommatecknet i kryssrutefältet och sedan använda indexet med LEFT-uttrycket för att visa så många tecken från början av listan. Här är koden:

```
valueexpression=IF(SEARCH(",",{DE:Checkbox Field},0)>0,LEFT({DE:Checkbox Field},SEARCH(",",{DE:Checkbox Field},0)),{DE:Checkbox Field})
```

Om du använder kommatecken i ett markeringsnamn i kryssrutefältet visas bara den delen av markeringen upp till det första kommatecknet.
