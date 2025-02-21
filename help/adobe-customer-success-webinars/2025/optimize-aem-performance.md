---
title: Optimera AEM prestanda - Cachelagra strategier och tekniker
description: Sessionen omfattade strategier och tekniker för cachelagring, mekanismer och nivåer för cachelagring, hantering av dynamiskt innehåll, problem med felsökning och synkronisering av cachedvalidering mellan dispatchern och CDN.
topic: Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3764
last-substantial-update: 2025-02-21T00:00:00Z
jira: KT-17373
source-git-commit: e7bf8b79ad4920b303fc3afbdfb4adee60614c88
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Optimera AEM prestanda: Cachelagra strategier och tekniker

Under den här sessionen utforskar vi olika mekanismer för cachelagring - som cachning av sidor, resurser och dispatcher - samt hur vi implementerar cachning på CDN-nivå för att optimera innehållsleveransen och minska inläsningstiden. Diskussionen handlar om de effektivaste strategierna för varje cachelagringslager, felsökning av vanliga problem och hur man utnyttjar CDN-funktionerna för maximal effektivitet.

## Viktiga diskussionspunkter

* Introduktion till cachning
* Olika typer av cachning, bästa praxis för cachning, ogiltigförklaring och uppdatering av cacheminnet
* Felsökning

>[!VIDEO](https://video.tv.adobe.com/v/3444452/?learn=on&enablevpops)

## Viktiga uppgifter

* **Cachelagringsstrategier och -tekniker** Sessionen fokuserade på olika cachelagringsstrategier och -tekniker för att optimera prestanda, inklusive cachelagring i olika lager som webbläsare, CDN och dispatcher.

* **Cachelagringsmekanismer och nivåer** Diskussionen behandlade olika cachningsmekanismer och -nivåer, inklusive webbläsarcachning, CDN-cachning och dispatcher-cachning samt hur de kan konfigureras och hanteras.

* **Hantering av dynamiskt innehåll** Tekniker för hantering av dynamiskt innehåll på en sida diskuterades, inklusive användningen av SDI (Sling Dynamic Include) och ESI (Edge Side Includes) för att säkerställa att dynamiskt innehåll inte cachelagras medan statiskt innehåll lagras.

* **Felsökning av cachelagringsproblem** Flera tekniker för att felsöka cachelagringsproblem på olika nivåer (webbläsare, CDN, dispatcher) har förklarats, bland annat användningen av rubriker, loggar och särskilda konfigurationer för att identifiera och lösa cachelagringsproblem.

* **Synkronisering av cache-invalidering** Sessionen åtgärdade ett problem med synkronisering av cachedvalidering mellan dispatchern och CDN, och rekommenderade att kortare max-age-värden och CDN-rensnings-API:er skulle användas för att se till att båda cacherna ogiltigförklaras samtidigt när sidan aktiveras.