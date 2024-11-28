---
title: Tales from 200 Trenches
description: Se till att webbprojekten blir framgångsrika genom att prioritera prestanda, använda Google PageSpeed Insights, optimera nyckeltal som LCP och TBT, hantera resurser effektivt och följa bästa praxis för utveckling och bildoptimering.
solution: Experience Manager, Experience Manager Sites
feature: Edge Delivery Services
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1321
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16541
source-git-commit: 07d4174b0d89ba2c417866e76ae72f015b91b03a
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Tales from 200 Trenches

Kiran Murugulla, Senior Engineer på Adobe och Varun Mitra, Architect for Adobe Experience Manager Cloud, delar med sig av sina över 200 Edge Delivery Services projekt. Upptäck hemligheterna bakom att leverera snabba, högpresterande upplevelser med enastående Core Web Vitals.


>[!VIDEO](https://video.tv.adobe.com/v/3439424/?learn=on&enablevpops)

## Community-diskussion

Fortsätt konversationen i [diskussionen](https://adobe.ly/4fwWvvi) i Adobe Developers Live Community.

## Viktiga uppgifter

* **Prestanda är av yttersta vikt**, särskilt webbsidornas hastighet, framhävs som en nyckelfaktor för framgångsrika webbprojekt. Ett av de viktigaste målen är att se till att resultatet blir 100.
* **Utvecklingspraxis**
   * Använd Google PageSpeed Insights för kontinuerlig testning under utvecklingen.
   * Starta projekt med standardkod som redan har 100 poäng för att behålla höga prestanda.
   * Se till att pull-förfrågningar uppfyller prestandastandarderna innan de sammanfogas.
* **Nyckelmått** Fokuserar på optimering av LCP (Störst Contentful Paint) och TBT (Total Blocking Time) eftersom de påverkar prestandan avsevärt.
* **Resurshantering**
   * Inkludera nödvändiga resurser som teckensnitt och skript från tredje part i projektkällan.
   * Använd reservteckensnitt för att förbättra inläsningstiden.
   * Fördröj inläsningen av icke nödvändiga skript för att förbättra den inledande inläsningsprestanda.
* **Bildoptimering** Prioritera inläsning av bilder som är lika stora som tidigare och använd högprioriterade hämtningsinställningar för viktiga bilder.
* **Fallstudier**
   * ***CNN.com*** Optimerade frågeindex och fördröjd inläsning av Google-annonser för att förbättra prestandan.
   * ***Herbert Homes*** Använde observations-API:t för skärningspunkt för att läsa in data när användare rullar, vilket förbättrar prestanda och användarupplevelse.
* **God praxis**
   * Börja med mallkod och använd välstrukturerad kod.
   * Använd avancerade CSS-väljare och minimera manipuleringen av JavaScript.
   * Fokusera på mobilutveckling först.
   * Säkerställ att innehållsstruktureringen är intuitiv för skribenterna.
* **Verktyg** Använd verktyg som Google Sheets och DSA för att följa upp webbplatsens prestanda över tid.

