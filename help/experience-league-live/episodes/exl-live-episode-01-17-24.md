---
title: Lägg in data och analyser från Adobe Analytics i Customer Journey Analytics
description: Se hur nya automatiserade processer kan hjälpa er att flytta analyser och data från Adobe Analytics till Adobe Customer Journey Analytics.
jira: KT-14746
thumbnail: https://video.tv.adobe.com/v/3426778?format=jpeg
event-cta-url-live: https://www.youtube.com/watch?v=BkAjaMPgpgE
event-cta-url-reg: https://engage.adobe.com/ExpLeagueLive-240117.html
event-start-time: 2024-01-17 10:00-7
event-guests: Doug Moore,Eric Matisoff,Bryan Skelton
exl-id: 2c2136a9-0b40-4a0a-907d-5af181568073
duration: 3655
source-git-commit: 604f85ddc402ed248678782412efe4f2e5988ab4
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Lägg in data och analyser från Adobe Analytics i Customer Journey Analytics

Delta i Bryan, Eric och Doug när de diskuterar hur ni snabbt ska komma igång med Customer Journey Analytics (CJA). Du får lära dig mer om hur du använder automatiserade processer för att flytta data och analyser från Adobe Analytics till CJA, samt hur mycket du ska tänka på under processen. Och de kommer förstås att ha en bra dos roliga tips och tricks på vägen.

>[!VIDEO](https://video.tv.adobe.com/v/3426778/?quality=12&learn=on)

>[!BEGINSHADEBOX Har du frågor?&quot;]

Fortsätt diskussionen om [Experience League användarforum](https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/experience-league-live-post-session-discussion-bringing-your/m-p/646093#M3582).

>[!ENDSHADEBOX]

## Viktiga uppgifter

* Det finns två sätt att hämta data från Adobe Analytics till Customer Journey Analytics: Analytics Data Connector (ADC) och Web SDK.
* ADC tillåter att data från en rapportsserie kopieras till Adobe Experience Platform för analys medan Web SDK skickar data direkt till Adobe Experience Platform.
* Med datavyer i Customer Journey Analytics kan du anpassa och analysera data som hämtas till plattformen.
* Datavyer har kraftfulla funktioner som retroaktiva ändringar, härledda fält för anpassning och möjlighet att filtrera och analysera data på detaljnivå.
* Anslutningar i Customer Journey Analytics gör det möjligt att kombinera olika datauppsättningar, vilket möjliggör analys av flera datakällor på ett och samma ställe.
* Datavyer och anslutningar bör användas strategiskt och med försiktighet för att säkerställa en korrekt styrning och kontroll över dataåtkomst och dataanalys.
* Det finns ett nytt verktyg som kallas&quot;komponentmigrering&quot; som gör att Adobe Analytics-administratörer kan migrera projekt till CGA.
* När du migrerar ett projekt flyttas alla komponenter i tabellerna, liksom alla segment eller beräknade värden, till CGA.
* Det finns en mappningsprocess där komponenter som inte finns i CGA kan mappas med&quot;catch-all&quot; eller härledda fält.
* Vi rekommenderar att du skapar en&quot;catch-all&quot; för element som inte finns i CGA och sedan redigerar dem i målprojektet.
* Tidigare trodde man att beräknade värden och segment måste återskapas när man migrerar till CGA, men nu finns det ett alternativ för att migrera dem.
* För att säkerställa att beräknade värden och segment inkluderas i migreringen måste de tillämpas på en tabell eller visualisering i Adobe Analytics.
