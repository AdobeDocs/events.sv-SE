---
title: Adobe Experience Manager Rapid Development Environment
description: Underlätta snabb utveckling och driftsättning i molnmiljöer med nya Adobe SDK, vilket minskar driftsättningstiden avsevärt och stöder snabba uppdateringar, livedoggar och avancerade konfigurationsalternativ, vilket diskuterades i DevOps Life 2024.
feature: Developer Tools
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2427
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16570
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Adobe Experience Manager Rapid Development Environment

Upptäck de bästa metoderna för snabba utvecklingsmiljöer och den uppdaterade utvecklarkonsolen. Natalia Angulo Herera, Software Development Engineer på Adobe, och Remo Liechti, Software Development Engineer på Adobe, täcker migreringsproblem, AIO CLI-installation, driftsättning, testning, loggning och konfigurationshantering för ett smidigare Adobe Experience Manager-arbetsflöde.

>[!VIDEO](https://video.tv.adobe.com/v/3440397/?learn=on&enablevpops)


## Community-diskussion

Fortsätt konversationen i [diskussionen](https://adobe.ly/3UJluDo) i Adobe Developers Live Community.

## Viktiga uppgifter

* **Introduktion till DevOps Life 2024** Mötet anordnas av Natalia och Remo från Adobe, med fokus på snabba utvecklingsmiljöer.
* **Problemsats** Utmaningen med lokala utvecklingsmiljöer som fungerar bra lokalt men som inte fungerar när de distribueras till molnet.
* **Lösning** Skapar en ny SDK i molnet för att underlätta snabb utveckling och distribution, vilket minskar tiden från 30 minuter till sekunder eller några minuter.
* **Distributionsprocess** I den nya miljön kan du snabbt uppdatera och validera via ett nytt API- och CLI-plugin-program, vilket ger snabbare feedback och driftsättning.
* **Infrastrukturskillnader** Molnmiljön använder en enda författare och publiceringsinstans utan hög tillgänglighet och använder inte MongoDB.
* **Installation och användning** Utvecklare kan konfigurera en snabb utvecklingsmiljö via molngränssnittet med hjälp av CLI för npm och Adobe IO för installation och konfiguration.
* **Grundläggande kommandon** Nyckelkommandon omfattar io amd —help, io login, io status, io install, io history, io delete och io reset.
* **Loggning och felsökning** Den nya miljön har stöd för live-loggar och byte av loggnivåer utan omdistribution med kommandon som io am eller d-loggar.
* **Avancerade ämnen** Stöd för frontendpaket och konfigurationspipelines, vilket möjliggör snabb distribution och upprepning.
* **Kommande funktioner** planerar att införa funktioner för ögonblicksbilder för enklare miljöåterställningar och automatiska uppdateringar utan innehållsförlust.
* **Frågor och svar och feedback** Sessionen uppmuntrar deltagare att gå med i Discord-kanalen för live-interaktion och feedback med utvecklingsteamet.