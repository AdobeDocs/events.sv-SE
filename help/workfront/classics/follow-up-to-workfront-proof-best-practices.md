---
title: Fråga experten - Följ upp Workfront Proof bästa praxis
description: Lär dig varför du bör använda automatiska arbetsflödesmallar, hur du skapar dem och hur du justerar korrekturinställningar för att säkerställa sekretess. Det här webbinariet spelades in den 4 mars 2020.
doc-type: feature video
team: Technical Marketing
kt: 9917
exl-id: 2b2f6522-2fd9-4d5e-9bc3-903c1d5e4e3b
duration: 4083
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 0%

---

# Fråga experten - Följ upp Workfront Proof bästa praxis

Lär dig varför du bör använda automatiska arbetsflödesmallar, hur du skapar dem och hur du justerar korrekturinställningar för att säkerställa sekretess. Det här webbinariet spelades in den 4 mars 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341123/?quality=12)

## Frågor och svar

**Fråga**

Det verkar som om vår instans automatiskt genererar korrektur när dokument överförs. Finns det något sätt att aktivera/inaktivera den här funktionen?

**Svar**

Ja, den här inställningen kan inaktiveras i din personliga profil. Om du klickar i Mina inställningar > Inställningar finns det en kryssruta för&quot;Generera korrektur automatiskt när du överför dokument&quot; som kan markeras eller avmarkeras.

**Fråga**

Kan du skapa ett arbetsflöde som har tomma faser så att du kan fylla i personer efter att ha bifogat det för att tillåta flera team att använda ett flöde?

**Svar**

Ja, automatiserade arbetsflödesmallar kan ha tomma steg så att olika användare kan läggas till beroende på vilket team som använder dem.

**Fråga**

I det här fallet överför designern dokumentet, men kontohanteraren genererar korrekturet och ställer in godkännandeflödet. När en ny version behövs lägger designern till versionen som ett dokument och processen börjar om. Finns det fortfarande ett sätt att låta kontohanteraren hantera korrekturflödet och designern hantera versionshanteringen utan att behöva skapa flödet varje gång du genererar det nya korrekturet?

**Svar**

Om du konfigurerar Designer med en åtkomstnivå för arbete eller plan i Workfront får de en korrekturlicens. Om korrekturlicensen är inställd på Administratör eller Administratör kan de skapa nya versioner av korrektur utan att behöva ta det manuella steget att låta Kontohanteraren konvertera den nya versionen och använda ett arbetsflöde. Den nya versionen kommer bara att anta arbetsflödet från den tidigare versionen (och kan även ändras nu).

**Fråga**

Vad rekommenderas för&quot;E-postaviseringar&quot;? beslut eller alla aviseringar?

**Svar**

Jag rekommenderar att Korrekturens skapare/ägare är inställd på &quot;Beslut&quot; för deras e-postavisering. Jag rekommenderar att alla andra korrekturmottagare är inställda på Inaktiverad för sin e-postavisering (även om e-postaviseringen är inaktiverad kommer de fortfarande att få meddelandena Nytt korrektur, Ny version, Senaste korrektur och @Mention e-post). Med den här inställningen kan du vara säker på att e-postvarningarna är riktade och att e-postmeddelanden hålls så få som möjligt.

**Fråga**

Kan du ändra ägaren till det bevis som meddelas när beslut fattas? Vi försökte använda korrekturverktyget, men det gick inte att ändra dokumentägaren från den person som överförde det ursprungliga dokumentet. Exempel: En marknadschef överförde originaldokumentet men det var en marknadsföringsspecialist som i slutändan ansvarade för att fatta beslut och göra ändringar.

**Svar**

Om du vill ändra ägare för korrekturläsaren följer du den här sökvägen: Dokument > Välj Korrektur > Klicka på &quot;Korrekturinformation&quot; > I fönstret med korrekturinformation, letar du reda på mottagaren som du vill göra ägare av korrekturläsaren > Klicka på knappen för Elips för den mottagaren och väljer &quot;Gör ägare&quot;.

**Fråga**

Finns det någon uppföljning av antalet granskningsrundor?

**Svar**

Vanligtvis matchar granskningsrundorna antalet korrekturversioner.

**Fråga**

Kan en person befinna sig i mer än ett stadium? Med andra ord, om vi har en chefer i en tidig granskningsrunda som har en slutgiltig granskning i ett senare skede, hur skulle vi då göra det?

**Svar**

Du kan inte lägga till en korrekturmottagare i mer än ett steg i en granskning av ett korrektur, men när granskningsfasen är aktiverad visas korrekturet i de återstående stegen för den versionen. Detta gör att de kan fortsätta att kommentera och svara på kommentarer även om andra steg har startats. Nyckeln till att se till att det här fungerar är att se till att du inte har faser låsta när den nya scenen startar.

**Fråga**

Kan du redigera befintliga arbetsflöden?

**Svar**

Ja, du vill navigera till Workfront Proof och sedan välja Arbetsflöden från den vänstra menyn. Där kan du redigera faser, lägga till användare, ta bort användare, lägga till faser osv.

**Fråga**

Finns det någon specifik fördel med att ha arbetsflödet för godkännande av ett dokument på korrekturet i stället för uppgiften? Vi har konfigurerat den för att ingå i dokumentet-/konstutvecklingsaktiviteten, så om bilden refuseras i något skede av godkännandeprocessen, aktiveras uppgiften igen så att den tilldelade designern kan revidera den. På så sätt behöver vi inte jobba på två ställen. Men jag kanske saknar nåt viktigt med att gå den här vägen.

**Svar**

När det gäller korrektur hanterar du godkännandeprocessen med korrekturarbetsflödesmotorn. Detta gör att du kan använda verktyget för korrekturgranskning för att samla in feedback, kommentarer, markeringar, beslut och faser. Du kan använda flera arbetsflödesutlösare för att dirigera korrekturet och kan använda inställningar som är unika för korrekturstadier, till exempel Låsning, Privata faser och Primära beslutsfattare. Du kan också tilldela unika korrekturroller och unika e-postmeddelanden om korrektur. Dessutom kan du granska innehåll som varierat som statiskt, video och interaktiva korrektur (ungefär 150 olika filtyper).

**Fråga**

Vem kan ställa in scenen på en privat scen? Endast administratörer?

**Svar**

Det är administratörsansvaret att skapa mallen, men alla användare som kan skapa ett korrektur kan göra scenen privat.

**Fråga**

Ingår deadline i e-postmeddelandet?

**Svar**

Ja, om du tillämpar en deadline på ett korrektur, visas det i e-postmeddelandet.

**Fråga**

Kan du dela en mall med en korrekturgrupp?

**Svar**

Observera dock att det bara delas med medlemmar i gruppen som har korrekturlicenser. Du kan inte dela mallar med Workfront-användare eller gäster som inte har några korrekturlicenser.

**Fråga**

Hur omdirigeras ett bevis till en intygsägare om det avvisas?

**Svar**

Korrekturägaren finns kvar på beviset under alla korrekturfaser. Om beviset inte godkänns behöver inte själva beviset skickas tillbaka till ägaren. I stället meddelas korrekturägaren via e-post om det beslut som fattats, granskar kommentarerna och kommer igång med en ny version.

**Fråga**

Hur stänger jag av/döljer &#39;Ladda ned&#39;-dokument i korrektur?

**Svar**

När du lägger till ett nytt korrektur ska du rulla längst ned tills du kommer till Korrekturinställningar. Här visas en kryssruta för&quot;Hämta originalfil&quot; som du kan välja eller avmarkera?

**Fråga**

Hur påverkar den här sekretessinställningen i Kontoinställningar korrekturläsare som använder den automatiska jämförelsen (sida vid sida med automatisk jämförelse) - Hindrar en inställning som är standard till DISabled granskaren från att jämföra två versioner?

**Svar**

För delningsinställningen för&quot;Mottagare kan visa alla versioner&quot; - om den är inställd på&quot;Inaktiverad&quot;, om mottagaren inte är i version 1 men har version 2, kan de inte jämföra version 1 och 2. Observera att Workfront-användare med behörigheten Korrekturansvarig eller Administratör kan se alla versioner oavsett inställning.

**Fråga**

Kan flera personer ladda upp en ny version? till exempel skickar en copywriter version 1 och sedan har vi korrekturet i steg 1. De ser en förändring som behöver göras, eller hur?

**Svar**

Du kan låta korrekturmottagare skapa nya versioner av korrektur om de uppfyller följande villkor: 1) De är ägare av beviset - eller 2) De är inställda med korrekturrollen Författare eller Moderator på beviset - eller 3) De är konfigurerade med behörighetsnivån Korrektur för övervakare eller administratör.

**Fråga**

Hur hanterar man flera korrektur (t.ex. A, B och C) med det automatiserade arbetsflödet. Börjar du igen?

**Svar**

Du kan använda en automatisk arbetsflödesmall för flera korrektur när du skapar den första versionen av korrekturet. Gör så här: Dokument > Lägg till ny > Korrektur. På sidan Nytt korrektur väljer du flera filer som ska överföras, använder mallen för automatiskt arbetsflöde och skapar korrektur.

**Fråga**

Kan ett korrektur exporteras med kommentarer till en PDF?

**Svar**

Du kan exportera en utskriftssammanfattning för ett korrektur till en PDF-fil. Detta kommer att innehålla alla kommentarer, markeringar, svar och beslut.

**Fråga**

Var kan jag se korrekturinställningarna?

**Svar**

Om du vill visa korrekturinställningarna för ett befintligt korrektur följer du den här sökvägen: Fliken Dokument > Välj Korrektur > Klicka på Korrekturinformation > Från i fönstret Korrekturinformation som öppnas, du vill expandera området Inställningar.

**Fråga**

Kan du tagga någon på den privata scenen?

**Svar**

Om du är en korrekturmottagare på den privata scenen kan du tagga vem som helst på den privata scenen. Om du inte befinner dig på den privata scenen kan du inte tagga någon från den privata scenen.

**Fråga**

När du har aktiverat en scen, kan du inaktivera den?

**Svar**

Du kommer inte att kunna inaktivera en aktiv fas, men du kan låsa scenen, vilket förhindrar att personer på scenen kan göra kommentarer och fatta beslut.

**Fråga**

Vad händer bakom kulisserna när en eller flera granskare i en scen säger att ändringar krävs? Vem meddelas om att ladda upp en ny version?

**Svar**

Detta beror på korrekturläsarens och/eller korrekturläsarens inställning &quot;E-postavisering&quot; på korrekturet. Jag rekommenderar att korrekturförfattare/ägare får e-postavisering om &quot;beslut&quot; så att de meddelas via e-post när som helst när ett beslut fattas om beviset.
