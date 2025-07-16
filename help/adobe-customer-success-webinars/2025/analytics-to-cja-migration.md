---
title: Bästa tillvägagångssätt vid migrering till Adobe Customer Journey Analytics från Adobe Analytics
description: Lär dig de viktigaste stegen och de bästa sätten att migrera från Adobe Analytics till Customer Journey Analytics (CJA), inklusive XDM-schemadesign, datamappning och datavykonfiguration.
solution: Analytics, Customer Journey Analytics
topic: Migration
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 3654
last-substantial-update: 2025-07-16T00:00:00Z
jira: KT-18535
source-git-commit: 90eb4a9d2cf445c58fde776092fb047f820fa207
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Bästa tillvägagångssätt vid migrering till Adobe Customer Journey Analytics från Adobe Analytics

Läs mer om migreringen från Adobe Analytics till Customer Journey Analytics (CJA). Mötet leds av Nicolina Picone och Maurizio Corlio från Adobe Ultimate Success-team och ger en djupgående översikt över CJA, dess funktioner och bästa metoder för migration.

## Viktiga ämnen som diskuteras

* skillnader mellan Analytics och CJA
* vikten av starka identitetsidentifierare, att anpassa datastrukturer och att skapa anpassningsbara datavyer
* täcker strategier för import av historiska data, hantering av attribuering av marknadsföringskanaler och användning av CJA flexibilitet för skräddarsydd rapportering

>[!VIDEO](https://video.tv.adobe.com/v/3464911/?learn=on&enablevpops)

## Viktiga åtgärder

* **Customer Journey Analytics (CJA) Översikt** CJA är en utveckling av Adobe Analytics som fokuserar på hela kundresan över flera kontaktytor (t.ex. mobiler, webben, CRM, callcenters) i stället för enspårsaktiviteter. Det möjliggör databehandling och -hantering i realtid.

* **Migreringsberedskap** Viktiga steg för migrering från Adobe Analytics till CJA är att kontrollera en stark identitetsbeteckning (t.ex. person-ID), justera variabler och dimensioner samt mappa data till XDM-schemat. Historiska data kan importeras med valideringssteg.

* **Datavyer och flexibilitet** Med CJA kan du skapa anpassningsbara datavyer med justerbar sessionstid, segmenteringsfilter och attribueringsinställningar. Denna flexibilitet möjliggör skräddarsydd rapportering och analys.

* **Bästa praxis för historik datamigrering** Validera CJA-data genom att jämföra dem med Adobe Analytics-data inom ett tillåtet intervall (t.ex. 10 % skillnad). Börja med ett kort fönster för bakåtfyllnad (t.ex. en månad) och skala upp gradvis.

* **Attribution för marknadsföringskanal** CJA erbjuder förbättrade funktioner för attribuering av marknadsföringskanaler, vilket eliminerar begränsningar som den första besökssidan och möjliggör mer dynamiska sessionskonfigurationer.
