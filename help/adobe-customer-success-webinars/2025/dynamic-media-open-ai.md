---
title: Mastering Dynamic Media with Open API
description: Förstå de viktigaste skillnaderna mellan traditionell Dynamic Media och Open API-modellen och lär dig hur ni lyckas med övergången och implementeringen av Dynamic Media Ultimate med Open API.
solution: Experience Manager as a Cloud Service, Experience Manager Assets
feature-set: Experience Manager Assets
feature: SDK/API
topic: Development, Content Management
role: Admin, Developer, User
level: Beginner, Intermediate
doc-type: Event
duration: 2757
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18702
source-git-commit: ef1eacd73c5a4fb9cdfee730d40606ec65bab2a7
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 1%

---


# Mastering Dynamic Media with Open API

Det här webbinariet är utformat för proffs som är bekanta med traditionella dynamiska media och som vill förstå och implementera [Dynamic Media Ultimate](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dm-prime-ultimate) med Open API.  Vi kommer att utforska Dynamic Media Ultimate och jämföra det med traditionell Dynamic Media. Vårt mål är att ge en heltäckande bild av skillnaderna mellan dessa två metoder, så att deltagare som är bekanta med Dynamic Media enkelt kan anpassa sig till den öppna API-modellen.

>[!VIDEO](https://video.tv.adobe.com/v/3470620/?learn=on&enablevpops)

## Jämförelse av nyckelfunktioner

| Funktion | Dynamiska medier | Dynamiska medier med OpenAPI |
|-----------------------------|------------------------|----------------------------|
| *Tillgänglighet* | Lokalt, AMS, Cloud | Endast molnet |
| *Modifierare* | Det finns många tillgängliga | Begränsad men växande |
| *Åtkomstkontroll* | Öppna för alla användare | Begränsat av roller |
| *CDN TTL* | ~10 timmar | ~10 minuter |
| *Kräv godkännande* | Automatiskt publicerad | Kräver godkännande |
| *Egen SEO* | Ja | Ja |

## Integreringsscenarier

Dessa integreringsscenarier visar på flexibiliteten och skalbarheten hos Dynamic Media med OpenAPI för olika företagsbehov.

* **AEM Sites-integrering** Dynamic Media med OpenAPI har stöd för sömlös integrering med AEM Sites, vilket gör att resurser kan hämtas direkt från leveransnivån utan duplicering.
* **Tredjepartsprogram** Aktiverar integrering med plattformar som Salesforce och Drupal med API:er eller mikrofront-end-program.
* **API-styrd åtkomst** innehåller API:er för sökning, hämtning och leverans av optimerade återgivningar av resurser.
* **Leveransnivåoptimering** Assets levereras via Snabbt, vilket ger snabbare och effektivare leverans.