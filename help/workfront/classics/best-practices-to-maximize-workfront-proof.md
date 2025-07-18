---
title: Fråga experten om bästa praxis för att maximera Workfront Proof
description: Lär dig hur du konfigurerar inställningar, aktiverar bra rapporter och undviker vanliga fel i korrektur. Det här webbinariet spelades in den 26 februari 2020.
doc-type: feature video
team: Technical Marketing
kt: 9916
exl-id: 7d3e437d-4a6e-44b8-9eff-eabb8284c391
duration: 5182
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '5572'
ht-degree: 0%

---

# Fråga experten om bästa praxis för att maximera Workfront Proof

Lär dig hur du konfigurerar inställningar för att lyckas, får åtkomst till vyer (och andra knep) för att skapa bra rapporter och hur du undviker vanliga fallgropar i korrektur. Det här webbinariet spelades in den 26 februari 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341122/?quality=12)

## Frågor och svar

**Fråga**

För att ge en mottagare möjlighet att dela ett korrektur som delats med honom eller henne måste du för närvarande markera rutan &quot;prenumeration&quot; under korrekturinställningar. Finns det några planer på att göra den här kryssrutan till automatisk kontroll som standard?

**Svar**

Detta kan aktiveras/inaktiveras som standard för enskilda användare av en administratör genom att följa den här sökvägen: PHQ-inloggning > Kontoinställningar > Användare > Klicka på användarens namn > Standardkorrekturinställningar.

**Fråga**

Om du inte väljer Nytt korrektur och du överför ett dokument och användaren är inställd på att automatiskt generera korrektur. Kan du ändra dessa inställningar efter att filerna redan har överförts?

**Svar**

Ja. Du kan justera alla korrekturinställningar genom att markera korrekturet på fliken Dokument och sedan klicka på Korrekturinformation.

**Fråga**

Gäller denna presentation fristående verktyg?

**Svar**

Rekommendationer om korrekturroller, e-postaviseringar, beslutsalternativ, vidarebefordrande e-postmeddelanden och gruppering/delning/inställningar av arbetsflödesmallar är alla relevanta för fristående korrektur.

**Fråga**

Vad använder du en korrekturmall för?

**Svar**

Om din organisations innehållsgranskningsprocess ofta upprepas eller om innehållet ofta granskas av samma personer, kan du skapa arbetsflödesmallar som innehåller dessa granskare med korrekturroller och aviseringsinställningar som du anger.

**Fråga**

Vad är en korrekturarbetsflödesmall?

**Svar**

En mall för korrekturarbetsflöde är en mall med ett fördefinierat arbetsflöde för korrekturläsning som kan användas på korrektur. Med dem kan ni både standardisera och automatisera processer för godkännande av korrektur.

**Fråga**

Hur skapar man en korrekturmall?

**Svar**

Som administratör vill du följa den här sökvägen: PHQ-inloggning > Arbetsflöden > Ny > Ny mall.

**Fråga**

Kan malldelning användas för delning med grupper och team eller bara enskilda användare?

**Svar**

För närvarande kan du inte dela arbetsflödesmallar med Workfront Groups, Teams, Job Roles eller Companies. Du kan dock dela dem med enskilda personer och dela dem med korrekturgrupper. Om du vill skapa en korrekturgrupp följer du den här sökvägen: PHQ-inloggning > Grupper > Ny grupp.

**Fråga**

När du skickar in ett bevis - under Organisation - finns det då plats för att rensa bort de mappar som varje användare ser så att de bara ser de mappar som är tillämpliga på dem? Istället för alla mappar som har gjorts i företagskontot?

**Svar**

Frågan gäller fristående Workfront Proof. I fristående Workfront Proof kan du använda privata mappar för att dölja mappar för specifika användare. På så sätt får du en smidigare lista över mappar att välja mellan. Observera att du även kan använda type-ahead-logik för att hitta mappen som du vill lägga till ett korrektur till.

**Fråga**

Har granskare och godkännare möjlighet att ändra de här meddelandeinställningarna?

**Svar**

Administratörer i Workfront kan ändra standardinställningarna för e-postavisering för användare och kontakter. Den som skapar korrektur kan sedan ändra meddelandeinställningen när han eller hon skapar ett korrektur och på sitt befintliga korrektur.

Mottagare på korrektur kan alltid ändra sin e-postavisering för specifika korrektur på korrekturnivå i verktyget för korrekturläsare genom att välja inställningsikonen på den vänstra menyn.

**Fråga**

Åsidosätter e-postvarningarna de globala meddelandena?

**Svar**

Korrektur för e-postaviseringar är helt oberoende av de globala meddelandeinställningarna.

**Fråga**

Om granskarna är inställda på&quot;inaktiverad&quot;, hur vet de om det finns ett nytt bevis som de kan granska om de har avvisat en tidigare version?

**Svar**

E-postaviseringar är oberoende av e-postmeddelandet för nytt korrektur, ny version, e-post för risk, sen e-post och @Mentions-e-post. Om du väljer&quot;Inaktiverad&quot; som e-postavisering kommer du bara att inaktivera meddelanden om aktiviteter som kommentarer, svar och beslut på korrekturet (med undantag för @Mention e-post från kommentarer).

**Fråga**

Inaktiverar e-postinaktiveringen Enterprise wide? eller av Portfolio?

**Svar**

Inställningen som finns i Inställningar > E-post > Granska och godkänn som gör att e-postmeddelanden kan skickas när korrekturmottagare gör kommentarer är Enterprise Wide (det är en global inställning).

**Fråga**

Jag har en gästanvändare som har lagts till i korrekturet och som inte kan granska beviset. Och användaren har inte åtkomst i Workfront.

**Svar**

Om gästen har åtkomst till beviset, men inte kan göra några kommentarer eller beslut, kontrollerar du att deras korrekturroll finns i korrekturfilen. I det här fallet kan de ha lagts till i korrekturläsningen med rollen&quot;Skrivskyddad&quot;. Om de är konfigurerade som granskare eller granskare och godkännare på korrekturet och fortfarande inte kan göra kommentarer/markeringar/beslut, skickar du en supportanmälan.

**Fråga**

Kräver gästanvändare en licens?

**Svar**

Gästanvändare behöver ingen licens.

**Fråga**

Ser jag inte bevislådan?

**Svar**

Om du inte ser rutan för korrekturbeslut på ett korrektur kan du ställa in dig på korrekturet med rollen Skrivskyddad eller Granskare, eller så har den scen som du befinner dig i på korrekturet ännu inte startats.

**Fråga**

Kan du förtydliga inställningen i WF>Konfigurera - om du har möjlighet att skicka e-post för varje kommentar - skickas dessa även om e-postmeddelandet i PHQ är inaktiverat? och vem får mejlen?

**Svar**

Alternativet Workfront-inställningar > E-post > Granska och godkänn-meddelande är oberoende av alternativen för e-postavisering på korrekturnivån. Om detta är aktiverat får alla på varje korrektur ett e-postmeddelande varje gång någon på korrekturet som de är på gör en kommentar.

**Fråga**

Tidigare rekommenderade du&quot;inaktiverad&quot; för e-postaviseringar utanför korrekturägaren. Får mottagarna fortfarande ett e-postmeddelande om att de har tilldelats ett bevis i så fall?

**Svar**

Ja. E-postaviseringar (som kan ställas in på All Activity (Alla aktiviteter), Disabled (Inaktiverade), Decision etc) är oberoende av e-postmeddelanden med korrektur av meddelanden (Nytt korrektur, Ny version, Riskkorrektur, Sent Korrektur, @Mentions).

**Fråga**

Vad händer om du har en instans där någon läggs till i ett bevis och de känner att de inte borde vara där? Vill du inte ta bort&quot;Inte relevant&quot; och ge dem ett alternativ att välja?

**Svar**

Detta är en bra användning för alternativet Ej relevant beslut. Men om någon inte ska vara på beviset rekommenderar jag att de @Uppge korrekturägaren i en kommentar på beviset och ber om att bli borttagna. Om någon som ska fatta ett beslut om beviset fattar beslutet&quot;Inte relevant&quot; när de ska fatta ett beslut om Godkänt eller Ändringar krävs, kan detta ändra hur det arbetsflöde som tillämpas på det korrekturet fungerar.

**Fråga**

Var kan jag hitta kryssrutan för&quot;obligatorisk inloggning&quot; för gästanvändare?

**Svar**

Detta finns i korrekturinställningarna på sidan Korrekturinställningar när du skapar ett korrektur. Om korrekturet redan har skapats kan du komma åt den här inställningen genom att välja korrekturet på fliken Dokument och klicka på Korrekturinformation > Inställningar. Observera att du bara kan dela nödvändiga inloggningskorrektur med personer som har en språklicens.

**Fråga**

Kan någon ta bort sig själv från ett bevis om de har lagts till av någon annan?

**Svar**

Om personen har redigeringsbehörighet för beviset som de har lagts till i kan han eller hon ta bort sig själv. Personer med redigeringsbehörighet är Workfront-användare med en korrekturlicens på administratörs- eller kontrollnivå samt personer som har lagts till i beviset med korrekturroller för författare eller moderator. Alla andra måste tas bort av någon med redigeringsbehörighet.

**Fråga**

Varför skulle jag använda dokumentgodkännande jämfört med korrektur för godkännande eller vice versa?

**Svar**

Dokumentgodkännande kan användas för dokument som inte kräver kommentarer och markeringar i linje med det dokument som godkänns. Jag vill bara att du tittar på det här dokumentet och antingen godkänner eller avvisar det. Korrektur tillåter kommentarer och markeringar i dokumentet i verktyget för korrekturläsare. Du måste till exempel titta på det här beviset, lägga till kommentarer, lägga till markeringar och fatta ett beslut. I framtiden är planen att sammanföra de två funktionerna eftersom de är mycket lika.

**Fråga**

Vi är en marknadsföringsavdelning och vi gör ett internt korrekturgodkännande och måste sedan skicka ut externt till den som gjorde begäran. Vi ger inte våra beställare åtkomst till våra projekt. Vi vill inte heller att de ska se alla våra kommentarer i det interna beviset. Nu gör vi ett nytt rent korrektur och laddar ned det och mejlar det till dem. Vi vill att de ska använda Korrektur för högdagrar, men vet inte hur man gör det utan att det också ger dem tillgång till vårt projekt. Några förslag?

**Svar**

Jag rekommenderar att du använder Automated Workflow Templates så att du kan använda &quot;Private Stages&quot;. Med privata faser kan du dölja kommentarer, markeringar och beslut från gästgranskare i andra faser. På så sätt kan din interna korrekturgranskning döljas helt och hållet för den externa begäraren.

**Fråga**

Vad är det bästa sättet att lägga till sig själv som granskare och godkännare när någon har skapat ett bevis?

**Svar**

Om du är Workfront-användare med behörigheten Korrekturerad administratör eller arbetsledare kan du lägga till dig själv som granskare och godkännare för alla korrektur som du har tillgång till. I annat fall vill du att korrekturägaren (eller någon annan med redigeringsbehörighet för korrekturet) ska lägga till dig.

**Fråga**

Vi har försökt att tagga användare i ett korrektur, men de får inget e-postmeddelande. Finns det något i kontoinställningarna för att säkerställa att ett e-postmeddelande skickas?

**Svar**

Jag rekommenderar att du kontrollerar e-postfilter/skräppostmapp för att se om meddelandena har skickats dit och sedan gör nödvändiga justeringar i e-postprogrammet för att vitlista dessa e-postmeddelanden. Du kan även kontakta vårt supportteam och få hjälp med detta.

**Fråga**

Du kan bara @ någon om de har en korrekturlicens, eller hur? Som i har den här personen aldrig varit i korrekturet och du vill tagga (@) dem.

**Svar**

Om du är gäst eller Workfront-användare och har en korrekturläsningslicens för Manager kan du @Mention för alla som finns på beviset (oavsett om personen har en licens eller inte). Om du är en Workfront-användare med en korrekturläsare eller administratör, eller om du är Korrekturägare, kan du @Uppge vem som helst i din kontaktlista på språkplattformen.

**Fråga**

Det största problemet här: e-postadress %2B (dubblettadresser). Varför och hur händer det och hur kan det repareras?

**Svar**

Det här kan hända om någon lägger till någon i ett korrektur manuellt med fel e-postadress. Om du stöter på detta kan en administratör ta bort den felaktiga e-postadressen från Korrekturkontot genom att följa den här sökvägen: PHQ-inloggning > Kontakter > Välj fel e-postadress/gästinstans > Ta bort. Om du stöter på problem med att användare läggs till med dubbla e-postadresser ber vi dig kontakta vårt supportteam för hjälp.

**Fråga**

När man väl har fattat ett beslut måste man ändra tillbaka beviset till produktion. Vilken typ av åtkomst behöver du ge produktionsteamet så att de kan använda kommentarens åtgärd om korrekturet är låst?

**Svar**

Om ett korrektur är låst måste du låsa upp korrekturet för att någon ska kunna göra kommentarer eller svara på kommentarer. Personer med följande behörigheter kan låsa upp korrekturläsaren: Korrekturägaren, Workfront-användare med en korrekturlicensnivå som administratör eller ansvarig.

**Fråga**

Vilken är den bästa lösningen för team att känna till korrektur som redan finns i en personkö?

**Svar**

Du kan skapa en korrekturgodkännanderapport inifrån Workfront. Du kan sedan använda filter som bara visar korrektur för vissa användare som fortfarande behöver ett beslut.

**Fråga**

Finns det något sätt att ladda ned korrektur med tillhörande godkännanden i en mapp?

**Svar**

Du kan öppna och ladda ned en Skriv ut sammanfattningsrapport för dina korrektur som innehåller alla kommentarer, svar, markeringar, åtgärder och beslut för alla versioner.

**Fråga**

När användare som begär åtkomst till rapportering får även detta åtkomst till avsnittet till vänster (dvs. arbetsflöden, kontakter, kontoinställningar osv.)?

**Svar**

Detta beror på deras korrekturlicensnivå. Om de är konfigurerade med chefs- eller tillsynslicensen kan de komma åt Kontakter, men de kommer inte att kunna komma åt Kontoinställningar och Arbetsflöden. Om de är konfigurerade med administratörslicensen har de åtkomst till kontoinställningar och arbetsflöden.

**Fråga**

I min organisation skickar projektledaren en begäran om godkännande till intressenter för granskning/kommentarer. Du nämnde att vi inte ska lägga till namn i godkännandefälten, hur delar du som PM-ledaren det kreativa beviset till intressenter?

**Svar**

Godkännandefältet är för dokumentgodkännanden, vilket är bra att använda om du bara behöver ett enkelt dokumentgodkännande. Om du vill ha ett korrekturgodkännande (med kommentarer, markeringar och ett korrekturbeslut) vill du lägga till intressenter i beviset med rollen som korrekturläsare och godkännare.

**Fråga**

Hur lägger du till personer som nya roller i ett redan skapat bevis?

**Svar**

Om du vill lägga till korrekturmottagare och välja deras korrekturroll på ett befintligt korrektur, ska du följa den här sökvägen: Välj korrekturet på dokumentfliken > och klicka sedan på Korrekturinformation. När fönstret med korrekturinformation öppnas klickar du på knappen för att visa information i det övre högra hörnet på scenen och väljer sedan &quot;Dela&quot;. Du kan sedan lägga till mottagarna och välja deras korrekturroll och e-postavisering.

**Fråga**

Om vi ger korrekturläsare/-skapare åtkomst till korrekturfrågor, kan vi då blockera administrationsområden som arbetsflöden, grupper osv.?

**Svar**

Ja, detta avgörs av behörigheten för användarkorrektur. Användare med behörigheten Korrektur för chef eller ansvarig har inte åtkomst till kontoinställningar och arbetsflödesmallar. Användare med behörigheten Korrekturadministratör får tillgång till kontoinställningar och arbetsflödesmallar. Alla användare med åtkomst kan komma åt gruppområdet.

**Fråga**

Hur kan användare se alla korrektur de har tilldelats utan att vara korrekturhanterare?

**Svar**

Om en användare vill se alla korrektur som de fortfarande behöver fatta ett beslut om, kan de använda området Hem eller Mina uppdateringar i Workfront (beroende på åtkomstnivå). Du kan också skapa en korrekturgranskningsrapport och använda filter för att endast visa korrektur som den inloggade användaren är granskare och godkännare för.

**Fråga**

Hallå, kan du gå igenom automatiserade korrekturarbetsflöden, för situationer där det finns tre olika utkast och feedback, och hur du får plats med när feedback kommer ut sent, och hur kan du bäst knyta detta till uppgifter i WF för varje runda (feedback från design- och projektledare)?

**Svar**

Du kan göra många olika saker för att se hur du använder uppgifter tillsammans med Granska och godkänn. En metod jag gillar är att ha en uppgift för Korrekturutskick och jag använder korrekturarbetsflödet för att hantera meddelanden till mottagare (i stället för att tilldela dem en uppgift). Du kan sedan skapa en uppgift för&quot;Korrektur för cirkulationsrundor 2&quot; och&quot;Korrektur för cirkulationsrundor 3&quot; som hjälper dig att hålla reda på hur många rundor som har gått runt. Du kan också hålla reda på förloppet för korrektur med hjälp av Inloggningsfunktionen för korrektur (PHQ > Instrumentpanel > Korrektur att hantera). I den här vyn visas antalet försenade korrektur (samt vid riskkorrektur) som du hanterar.

**Fråga**

När ett korrektur tas bort, finns det en kopia av det beviset kvar på dina servrar?

**Svar**

Ja. Om du tar bort ett korrektur som det finns i papperskorgen för det associerade korrekturkontot kan det återställas därifrån om det behövs och kommer att finnas kvar där tills och om inte papperskorgen töms.

**Fråga**

Finns det något sätt att få ett nytt beslut att utlösas om en annan användare avvisar eller godkänner ändringarna. t. ex. Korrekturpanelen ser något, projektledaren måste fatta ett nytt beslut även om de redan har granskat det och godkänt det. (försöker du inte få proj-hanteraren att inte behöva vänta på korrekturläsningssidan för att kunna utföra granskningen)?

**Svar**

Detta kan inte automatiseras, men du kan ange e-postavisering om beslut till projektledaren. När korrekturläsningsavdelningen fattar sitt beslut meddelas projektledaren om vilket beslut som fattats och kan sedan gå tillbaka till korrekturet, granska kommentarerna från korrekturläsningsavdelningen och ändra deras beslut vid behov.

**Fråga**

Varför när jag markerar&quot;Fråga efter godkännande&quot; när jag skickar en uppdatering i avsnittet Korrekturinformation, ser jag bara statusen SOC och inte SOCD. Ska vi undvika att använda den här kryssrutan? Vad är bästa sättet att skicka en uppdatering för ett korrektur?

**Svar**

När du använder funktionen&quot;Fråga efter godkännande&quot; arbetar du med funktionen Dokumentgodkännande som är oberoende av korrektur och SOCD-förloppsindikatorn. Om du behöver uppdatera korrekturrollen för en korrekturmottagare ska du följa den här sökvägen: Välj korrektur på fliken Dokument och klicka sedan på Korrekturinformation. När fönstret med korrekturinformation öppnas ser du en lista över mottagare och du kan justera alternativet för korrekturroll (och e-postavisering) efter behov. På så sätt kan du (till exempel) ändra korrekturrollen från Granskare till Granskare och godkännare.

**Fråga**

Är det möjligt att se till att de slutliga godkännarna inte har tillgång till tidigare versioner (och kommentarer) om det finns i samma korrekturdokument? Måste man skapa ett nytt korrekturdokument, eller finns det något sätt att samla alla versioner och kommentarer i ett och samma dokument och ange vilka versioner som ska vara tillgängliga?

**Svar**

I kontoinställningarna i ett korrektur kan du styra åtkomsten till dina korrektur för delning/synlighet. Om du vill uppdatera den här inställningen så att korrekturmottagare bara ser de versioner av korrektur som du anger (i stället för att se alla versioner av korrekturet) vill du följa den här sökvägen: PHQ-inloggning > Kontoinställningar > Inställningar > Delning > Mottagare kan visa alla versioner = inaktiverade.

**Fråga**

Kan du lägga till korrekturpanelen som en extern sida på en WF-instrumentpanel? Ser icke-administratörer instrumentpanelen?

**Svar**

Du kan lägga till kontrollpanelen för korrektur som en extern sida i en kontrollpanel. Observera att detta endast är synligt för användare som har en korrekturlicens.

**Fråga**

Funktionerna Dashboard och Reporting i ProofHQ är bara tillgängliga för administratörer som har åtkomst till Proof, eller hur? Är det inte allmänna planer som inte har administratörsåtkomst?

**Svar**

Det här är korrekt. Även om du kan skicka in ett supportärende till Workfront för att begära att alla dina användare av språklicens har tillgång till systemet för korrektur.

**Fråga**

Hej, en fråga om korrekturägarskapsflexibilitet: Om en ny version av korrektur krävs utan den ursprungliga ägaren, är det bäst att de lägger till en kollega i arbetsflödet som författare och sedan bestämmer de&quot;Inte relevant&quot;? (Att delegera ägarskap verkar bara fungera för en enda version).

**Svar**

Det här användningsexemplet och arbetsflödet skulle absolut fungera. En annan sak du kan tänka dig är att användare som kanske behöver överföra nya versioner till korrektur som de inte är ägare till ska konfigureras med behörigheten Korrekturnivå för övervakare eller administratör. Med den här behörighetsnivån kan de överföra nya versioner till korrektur som de inte är ägare av utan att behöva lägga till dem i beviset som författare eller moderator (vilket båda kräver ett beslut).

**Fråga**

Som jag förstår det kan du inte lägga till samma användare i efterföljande faser i ett automatiserat arbetsflöde, vilket är problematiskt för oss. Är detta något du kan ändra för att tillåta att samma användare befinner sig i flera faser?

**Svar**

Du kan inte lägga till en korrekturmottagare i mer än ett steg i en granskning av ett korrektur, men när granskningsfasen är aktiverad visas korrekturet i de återstående stegen för den versionen. Detta gör att de kan fortsätta att kommentera och svara på kommentarer även om andra steg har startats. Nyckeln till att kontrollera att det här fungerar är att se till att du inte har faser låsta när nya faser startar.

**Fråga**

Kan du förklara hur korrektur slingrar sig mellan faser? Hur stänger man en och flyttar till nästa scen?

**Svar**

Det finns ett antal alternativ i automatiserade arbetsflödesmallar som gör att användaren kan gå från en fas till nästa. Alternativ som du kan använda är&quot;Vid skapande av bevis&quot;,&quot;När alla beslut har godkänts i ett överordnat skede&quot;&quot;När alla beslut har godkänts eller godkänts med ändringar i ett överordnat steg&quot;,&quot;När alla beslut har fattats i ett överordnat skede&quot; samt några andra alternativ.

**Fråga**

Kan du ta bort ett korrektur från ett dokument som har genererats automatiskt, men inte vill att det ska vara ett korrektur?

**Svar**

Om du har aktiverat inställningen &quot;Generera korrektur automatiskt när du överför dokument&quot; kan du inte ta bort ett korrektur från ett dokument. I stället vill du ladda upp det igen med knappen Lägg till nytt > Dokument.

**Fråga**

Kan en användare säga på steg 3 i korrekturflödet att en annan person läggs till som gransknings- och godkännare?

**Svar**

Om användaren har redigeringsbehörighet för det bevis som han/hon kan. Personer med redigeringsbehörighet: Korrekturägare, Korrekturmottagare läggs till i beviset med rollen Korrekturansvarig eller moderator, Bevislicensanvändare med behörigheten Korrekturansvarig eller Administratör.

**Fråga**

Om en användare har utsetts till författare, kan han/hon ladda upp en ny version av korrekturet? Det här är någon annan än den som beställt beviset.

**Svar**

Korrekturmottagare med korrekturrollen författare och moderator kan lägga till nya versioner till korrekturet som de är på med den korrekturrollen.

**Fråga**

Externa användare får ett mejl per korrektur för granskning. Detta kan vara en utmaning för dem att spåra statusen för alla korrektur som de har i spel. Finns det några kontrollpaneler eller e-poststatuslistalternativ eller kommande funktioner som externa användare kan använda för att spåra sin status på flera korrektur?

**Svar**

Jag rekommenderar att du lägger till dessa externa användare i Workfront med en kostnadsfri licens för Reviewer. Detta ger dem tillgång till sidan Mina uppdateringar, som innehåller en lista över alla utestående korrektur som de behöver fatta beslut om.

**Fråga**

Kan du förklara mer om beslutsmeddelandena? Får jag bara meddelanden med korrekturkommentarer från granskare och godkännare eller får jag också kommentarerna från granskarna och när får jag dem?

**Svar**

Meddelanden om e-postavisering för beslut skickas endast när beslut fattas på beviset. De kommer inte att skickas när kommentarer görs. Om du får ett e-postmeddelande om beslut som anger att en mottagare har fattat ett beslut om ändringar som krävs, vet du att det är ett bra tillfälle att granska de kommentarer som han/hon har lagt till (som finns i korrekturet).

**Fråga**

Vad gäller frågan om vidarebefordran av e-post, loggar du faktiskt in som den som äger e-postmeddelandet? Och skulle det ske i låsta miljöer? Skulle det ske i en SSO-miljö?

**Svar**

Då loggas du in i beviset som den person som vidarebefordrade e-postmeddelandet till dig. Om du använder inloggning krävs på korrektur och enkel inloggning (SSO) kommer du inte att få åtkomst till beviset som den person som skickade e-postmeddelandet till dig.

**Fråga**

Var kommer jag åt kontrollpanelen och rapporter när jag korrekturerar?

**Svar**

Om du har en kryssruteikon till höger om sökfältet i Workfront innebär det att du har ett integrerat Workfront- och korrekturkonto. Genom att klicka på den kryssrutan kommer du till Workfront Proof och startskärmen blir kontrollpanelen. Du kan skapa rapporter med alternativet Vyer på den vänstra panelen.

**Fråga**

Under delen Roll finns det två bockar längst ned som anger att någon ska lägga till med en @mention etc. I inställningarna för korrektur kan du ange standardroller för varje person, men det finns inget alternativ för att markera kryssmarkeringarna automatiskt, så du måste göra det varje gång du skapar ett korrektur. Hur kan du göra det till standard för en användare?

**Svar**

Det finns för närvarande inget sätt att göra detta till en standardinställning för korrekturmottagare. Du kan dock spara dessa som standardinställningar för mottagare i Automatiserade arbetsflödesmallar.

**Fråga**

Hur byter du korrekturägare?

**Svar**

Om du vill växla ägare till ett korrektur följer du den här sökvägen: Markera korrekturet på fliken Dokument och klicka på Korrekturinformation. Fliken med korrekturinformation öppnas. Om den person som du vill göra ägare av korrekturet ännu inte finns med på korrekturet, vill du lägga till dem som mottagare genom att klicka på knappen Redigera och välja Dela. När personen har lagts till i korrekturet (eller om de redan finns på korrekturet) väljer du motsvarande Elipses-knapp och väljer&quot;Make Owner&quot;. De blir nu ägare till beviset.

**Fråga**

När det gäller nya versioner av korrektur.. är det enda sättet att göra detta att dra och släppa filen ovanpå den befintliga filen. Är detta det rätta sättet att göra det på?

**Svar**

Jag rekommenderar att du skapar nya versioner på det här sättet: markera korrekturet på fliken Dokument, klicka på knappen Mer och välj Ny version > Korrektur. Du kommer då till sidan Ny version, där du kan fortsätta med arbetsflödet och göra de justeringar du behöver innan du dirigerar den nya versionen.

**Fråga**

Kan du inaktivera kommentarer på korrektur för att dela med en kund så att de inte ser all intern feedback från teamet? Så att du inte behöver generera ett nytt bevis.

**Svar**

Jag rekommenderar att du använder Automated Workflow Templates så att du kan använda &quot;Private Stages&quot;. Med privata faser kan du dölja kommentarer, markeringar och beslut från gästgranskare i andra faser. På så sätt kan din interna korrekturgranskning döljas helt och hållet för den externa begäraren.

**Fråga**

Lägger Workfront Proof-scenen bara till när automatiserade arbetsflöden används och någon som inte har lagts till i arbetsflödet öppnar korrekturet?

**Svar**

Scenen&quot;Workfront Proof&quot; läggs till i korrektur om en icke-mottagare klickar på korrekturet. Den används också om någon konverterar ett grundläggande arbetsflödeskorrektur till en automatiserad Workfront Proof.

**Fråga**

Har vi möjlighet att skapa ett korrekturarbetsflöde där mer än ett beslut kan fattas?

Vi försöker rapportera till vårt interna juridiska team om när utomstående jurister har slutfört granskningar av korrektur (hur många dagar i genomsnitt det tar dem att slutföra granskningen, vem som slutför den, osv.)

Vi började med att lägga till ett nytt beslut i korrekturarbetsflödet som kallas&quot;OC Review Complete&quot; och antog att vi kunde sammanställa en rapport för att spåra dessa.

Problemet är att det bara går att fatta ett beslut om arbetsflödet.

**Svar**

Mer än ett beslut kan fattas om bevis - men det kommer bara att finnas en generell status på ett bevis som kommer från det värsta scenariobeslutet på beviset - eller det beslut som fattats av en primär beslutsfattare.

På grund av dina rapporteringskrav rekommenderar jag att alla som ska granska ska använda samma beslutsalternativ (Godkänd, Godkänd med ändringar, Ändringar krävs) och sedan använda rapportfunktionen i kontrollpanelen för korrektur (PHQ-inloggning > Rapporter) och använda filteralternativet för att filtrera efter mottagare (inkludera mottagare som inte är juridiska rådgivare i filtret). Då kan du se den genomsnittliga omvändningstiden för deras korrektur.

**Fråga**

När en ny version dras och släpps på ett befintligt korrektur, varför ändras ALLA roller eller försvinner specifikt?

**Svar**

När du drar och släpper ett dokument som en ny version är du säker på att arbetsflödet tas bort från den nya versionen. Om du vill behålla arbetsflödet från den tidigare versionen till nästa version markerar du korrekturet på fliken Dokument och klickar sedan på knappen Mer, väljer Ny version > Korrektur. Du kommer då till sidan Ny version, där du kan fortsätta med arbetsflödet och göra de justeringar du behöver innan du dirigerar den nya versionen.

**Fråga**

Scenario - Vidarebefordra korrektur: En extern kund som granskar ett korrektur kan vilja cirkulera internt på sin organisation innan han eller hon godkänner vårt bevis. De andra granskarna behöver inte vara med i systemet, så de verkar inte vara @ i kommentarerna. Hur ska de dela på bästa sätt - skicka e-postmeddelandet och markera för mottagaren att kommentarer inte ska visas som namn?

**Svar**

Du vill använda funktionen för korrektur av prenumerationer. Detta kan aktiveras i inställningarna för korrekturet och gör det möjligt för mottagarna på korrekturet att vidarebefordra en allmän offentlig länk till korrekturet och sedan tillåta mottagarna att prenumerera på korrekturet (lägga till sig själva).

**Fråga**

Vad är bästa sättet att använda mappar i dokument?

**Svar**

Detta beror på projektets karaktär, men något du kan tänka dig är en aktiv korrekturmapp som innehåller alla korrektur/versioner som aktivt dirigeras runt och en Godkänd korrekturmapp som innehåller alla korrektur som är slutförda och godkända. När ett korrektur är helt godkänt flyttar du det från mappen Aktiva korrektur till mappen Godkänt korrektur.

**Fråga**

Om jag har tre personer i en grupp granskningar, kan jag då ange att jag behöver godkännanden från två av dem?

**Svar**

Ja. Du ska lägga till de två personer som du behöver ett beslut från som granskare och godkännare och den tredje personen som granskare.

**Fråga**

Vi vill skicka ett korrektur till en extern kund (icke-Workfront-användare) som kan granska och kommentera. Vi vill skicka ett rent korrektur till dem (med andra ord ett utan interna kommentarer). Vilka steg är de rätta för att få detta att hända för att säkerställa att den externa kunden får beviset (bara beviset, ingen åtkomst till själva projektet) och hur skickar de externa klienterna tillbaka det markerade beviset? Vi använder för närvarande inte korrekturmallar/automatiserade arbetsflöden.

**Svar**

Jag rekommenderar att du använder automatiserade arbetsflödes-/automatiserade arbetsflödesmallar för detta eftersom det gör att du kan använda funktionen &quot;Privat scen&quot;. När du använder funktionen för den privata scenen kan du ha kommentarer/beslut och mottagarna av vissa granskningsfaser dolda för personer i andra faser. Du kan till exempel ha en intern fas som en privat fas och en klientfas. Klienterna kan inte se något med den interna scenen att göra medan du kan se aktiviteten i klientscenen.

**Fråga**

Går det att hålla specifika användare (även profilläsare) i ett tidigt skede utan att behöva använda dem som loopar i senare faser?

**Svar**

När någon har lagts till i en version av ett korrektur på ett stadium, kommer de att finnas kvar på den versionen av korrekturet under de återstående stegen. Du kan låsa scenen när nästa steg börjar (eller manuellt) vilket förhindrar att de kan göra fler kommentarer.

**Fråga**

Var kan vi se en lista över alla som har granskat och/eller godkänt ett bevis, vilken dag och vilken tid? För revision osv. Finns det också en plats där vi kan se alla granskningar och godkännanden för alla versioner av ett korrektur?

**Svar**

Om du vill se en lista över aktiviteter, t.ex. när kommentarer och beslut gjordes, vill du klicka i Aktivitetshistorik i Korrekturinformation. Följ den här sökvägen: Välj Korrektur på fliken Dokument > Klicka på Korrekturinformation > Expandera aktiviteten. Om du vill visa den här informationen på versionsnivå följer du den här sökvägen: Välj Korrektur på fliken Dokument > Klicka på fliken Information > Mot längst ned på skärmen så visas ett versionsavsnitt. Härifrån kan du visa korrekturinformationen på versionsnivå.

**Fråga**

Kan du prata lite om privata steg i korrektur?

**Svar**

När en fas görs privat är kommentarer och beslut inte synliga för personer som inte har lagts till på den här scenen eller inte är tillsynsmyndigheter, administratörer eller faktureringsadministratörer på kontot. Granskare som läggs till på en privat scen kan bara se den fas de läggs till i korrekturet och kommentarerna som görs i den fasen.
