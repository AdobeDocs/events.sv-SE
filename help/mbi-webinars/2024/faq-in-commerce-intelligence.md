---
title: Frågor och svar i Commerce Intelligence
description: Få svar på några vanliga frågor om Commerce Intelligence som rör självbetjäningskonfigurationer, integreringar, säkerhet, bästa praxis och mycket annat.
solution: Commerce, Commerce Intelligence
feature-set: Commerce Intelligence
role: Admin, User
level: Intermediate
doc-type: Event
duration: 2167
last-substantial-update: 2024-06-07T00:00:00Z
jira: KT-15680
exl-id: ead47498-4526-481c-8910-961377bdb55f
source-git-commit: 4471d715fb226701bdad95ffe2834e763451c7ea
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Frågor och svar i Commerce Intelligence

Få svar på några vanliga frågor om Commerce Intelligence som rör självbetjäningskonfigurationer, integreringar, säkerhet, bästa praxis och mycket annat.

>[!VIDEO](https://video.tv.adobe.com/v/3429617/?learn=on)

## Viktiga uppgifter

**Valutahantering**

* Valutor hanteras baserat på en enda valutainställning.
* Monetära siffror i rapporter föregås av den angivna valutasymbolen.
* Valutainställningarna görs i kontoinställningarna genom att en lämplig valuta väljs för konvertering av valutakurser.

**Metoder för dataimport**

* Dataimport kan göras med API-anslutning, CSP-överföringar och import-API.
* Oraclets DB stöds inte, men CSP-överföring eller import-API kan användas som alternativ.
* Begränsningar av API-användning inkluderar en begäran om förbrukning per månad och ungefär 100 poster, vilket motsvarar cirka 100 000 poster per månad.

**Source-integrering med data**

* Adobe Commerce Intelligence har stöd för flera datakällor som Adobe Commerce, SAS, API:er, databaser m.m.
* Tillåter konvergens av data från olika Adobe Commerce-instanser till en enda Commerce Intelligence-instans.
* Integrationen kan underlättas av Commerce Intelligence och supportteamet så att instansen konfigureras utifrån företagets behov.
