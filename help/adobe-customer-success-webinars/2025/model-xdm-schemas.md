---
title: Best Practices and Insights for Modeling XDM Schemas
description: Använd AEP som huvuddatamodellering med XDM-scheman, identitetshantering och bästa praxis för skalbar personalisering och segmentering i realtid.
topic: Personalization
role: Developer
level: Intermediate
doc-type: Event
duration: 3488
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18019
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Best Practices and Insights for Modeling XDM Schemas

Under den här sessionen får du lära dig viktiga arbetsmetoder och genvägar för att skapa skalbara, högkvalitativa Adobe Experience Data Models (XDM) som är anpassade efter Adobe Experience Platform standarder. Få insikter i hur ni effektivt kan mappa kundupplevelsen och använda falldata till XDM för smidig integrering mellan Adobe och externa verktyg.

## Diskussionspunkter

* Definiera och organisera XDM-komponenter för att säkerställa skalbara och flexibla datamodeller
* Vanliga utmaningar inom XDM-design, -utveckling och -underhåll

>[!VIDEO](https://video.tv.adobe.com/v/3458042/?learn=on&enablevpops)

## Viktiga uppgifter

**Datamodellering i Adobe Experience Platform (AEP)**

XDM-schemat är grunden för datamodellering i AEP, vilket möjliggör integrering och delning av data mellan olika system. Den definierar datastrukturen och datatypen, t.ex. profilattribut och händelsebaserade åtgärder.

**Identity Management**

Korrekt identitetshantering är avgörande för att undvika problem som till exempel komprimering av profiler. Genom att hash-koda känsliga data som e-post och använda unika identifierare kan dataintegriteten bevaras. Identitetskartor rekommenderas för segmentering och personalisering i realtid.

**Bästa praxis för schemadesign**

Använd scheman enkelt och fokuserat på användningsfall för marknadsföring. Undvik att överbelasta scheman med onödiga attribut. Använd standardiserade fältgrupper och minimera anpassningar för skalbarhet och framtida korrektur.

**Händelse kontra profilattribut**

Bestäm om data ska modelleras som profilattribut eller händelser utifrån marknadsföringsmålen. Profilattribut lämpar sig för målgruppsanpassning i realtid, medan händelser ger historiska insikter för tidsbaserad segmentering.

**Hantera komprimerade profiler och skalbarhet**

Komprimerade profiler kan bara korrigeras med Adobe-stöd, men regler för identitetsdiagram kan förhindra framtida komprimeringar. För omstrukturering av befintliga scheman rekommenderas att man extraherar nödvändiga data och börjar om med ett rent schema.
