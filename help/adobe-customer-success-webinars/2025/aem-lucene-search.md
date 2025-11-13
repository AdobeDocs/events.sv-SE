---
title: Essential Tips and Best Practices for AEM Lucene Search
description: Öka det digitala engagemanget med avancerade sökverktyg från AEM som filter, ansikten, autoföreslå, NGram och stavningskontroll. Lär dig av verkliga demos.
solution: Experience Manager
feature: Search
role: Admin, Developer
level: Intermediate, Experienced
doc-type: Event
duration: 3630
last-substantial-update: 2025-11-13T00:00:00Z
jira: KT-19550
source-git-commit: 84c9a126769fa94b0197d12ca594137e13edc510
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# Essential Tips and Best Practices for AEM Lucene Search

Upptäck hur ni kan förbättra er digitala närvaro och kundengagemang med de senaste sökfunktionerna, som filter, ansikten, automatiska förslag, NGram och stavningskontroll. Lär dig av verkliga demos och få insikter i hur du optimerar sökfunktionerna med AEM och Lucene. Det här webbinariet ger dig möjlighet att lyfta fram din sökupplevelse och ligga steget före i det digitala landskapet.

>[!VIDEO](https://video.tv.adobe.com/v/3476410/?learn=on&enablevpops)

## Låsa upp kraftfulla sökfunktioner i Adobe Experience Manager

Adobe Experience Manager (AEM) utnyttjar Lucene-sökningen för att leverera snabba, relevanta resultat för innehåll, resurser och metadata. Under den här sessionen behandlas hur Lucene-index fungerar, hur de konfigureras och de bästa sätten att maximera sökningsprestanda.

* **Lucene Search är Everywhere** Kraftfulla sökfunktioner i AEM författare, utgivare och portaler, som hanterar automatiska förslag, filter, facets och sidnumrering.
* **Indexdefinitioner Drivprestanda** Att anpassa Oak-indexdefinitioner är avgörande för en effektiv, riktad sökning.
* **Bästa praxis** Kopiera befintliga indexdefinitioner, begränsa indexerade egenskaper och använd rätt flaggor för fulltext- och egenskapssökningar.
* **Avancerade funktioner Förbättra UX**-ansikten, autoföreslå, stavningskontrollera, förbättra och ordna kan aktiveras för mer omfattande sökupplevelser.

Genom att förstå dessa principer kan du säkerställa stabila, värdefulla sökfunktioner i AEM, som stöder både tekniska och affärsmässiga mål.

## Byggblock för Lucene-index

Indexdefinitioner för AEM Lucene är grunden till sökningsprestanda och exakthet. Bland huvudkomponenterna finns:

* **Typ** Anger indextyp (Lucene, property, etc.).
* **Nodtypsbegränsning** Målar specifika innehållstyper (t.ex. dam:Asset, cq:Page).
* **Sökvägsbegränsning** Begränsar indexering till definierade databassökvägar för ökad effektivitet.
* **Sammanställningsregler** Styr djupet och omfånget för indexerat innehåll och ser till att relevanta egenskaper är sökbara.
* **Huvudkonfiguration för indexregler**; anger flaggor som nodeScopeIndex (bred textsökning) och analyserad (tokenisering/normalisering).

Med noggrann konfiguration av dessa element säkerställs att sökfrågorna är snabba, relevanta och resurseffektiva.

## Optimera sökprestanda

Effektiv sökoptimering i AEM Lucene innefattar strategisk konfiguration och efterlevnad av bästa praxis:

* **Börja med befintliga index** Kopiera och ändra alltid färdiga definitioner, skapa aldrig från grunden.
* **Begränsa indexerade egenskaper** Ta endast med nödvändiga egenskaper för att hålla indexen slimmade och presterande.
* **Använd flaggor på ett smart sätt:
   * **nodeScopeIndex** true för bred textsökning
   * **analyserad** true för tokenisering på egenskapsnivå
   * **evaluatePathRestriction** true för sökvägsbaserade frågor
* **Egenskapsindexering** Föredrar att egenskapsbegränsningar söker efter bästa prestanda. Använd bara fulltext när det behövs.
* **Sortering och ansikten** Aktivera propertyIndex och sorteringsordning. Ange facet** true för räkningsbaserad filtrering.

Om du tillämpar dessa strategier kan du få snabbare frågor, minskad resursanvändning och mer relevanta resultat.

