---
title: Streamline-autentisering - migrerar från tjänstkonto (JWT) till OAuth Server-till-server-autentiseringsuppgifter
solution: Experience Manager
feature: Developer Tools, Security
description: Adobe webbinarium, ledd av chefsingenjören Jeff Homequest och Marco Lara, fokuserade på att migrera från tjänstkontot JWT till OAuth server-till-server-autentiseringsuppgifter, och framhäver tidsgränsen i januari 2025, migreringssteg, fördelarna med OAuth och speciella överväganden för AEM, med omfattande stöd och dokumentation för processen.
topic: Integrations, Security, Migration
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3292
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16629
exl-id: 97e2a2de-1cb4-4f2f-8c9b-47ee40227625
source-git-commit: 460acb3fd1e9b29075cefa07e8d6947d2a61a314
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Streamline-autentisering: Migrerar från tjänstkonto (JWT) till OAuth Server-till-server-autentiseringsuppgifter

Det här webbinariet vägleder deltagarna genom att migrera från de inaktuella JWT-autentiseringsuppgifterna (Service Account) till de nya OAuth Server-to-Server-autentiseringsuppgifterna. Eftersom JWT-inloggningsuppgifterna inte längre fungerar efter 27 januari 2025 är det viktigt för utvecklare och organisationer att förstå migreringsprocessen för att undvika potentiella tjänstavbrott. Webbseminariet visar också fördelarna med autentiseringsuppgifterna för OAuth Server-till-Server och hur man säkerställer en migrering utan driftstopp.

>[!VIDEO](https://video.tv.adobe.com/v/3440936/?learn=on&enablevpops)

## Viktiga uppgifter

* **Mötesinspelning och bilder** Mötet spelades in och en länk till inspelningen är tillgänglig i slutet.
* **Introduktion till högtalare** Jeff Homequest och Marco Lara, båda chefsfältingenjörer på Adobe, ledde webbinariet.
* **Webbseminariefokus** Webbseminariet fokuserar på att migrera från tjänstkontot JWT till OAuth server-till-server-autentiseringsuppgifter.
* **Deadline för borttagning** Adobe tar bort JWT-autentiseringsuppgifter och de måste migreras före slutet av januari 2025.
* **Målgrupp** Webbseminariet vänder sig till programutvecklare, tekniska leads och integreringsarkitekter som använder JWT-referenser i Adobe-program.
* **Migreringssteg** Webbseminariet innehöll en steg-för-steg-migreringsguide och en demo.
* **Frågor och svar** togs under hela mötet, med en dedikerad session i slutet.
* **Fördelarna med OAuth** OAuth förenklar utveckling, förbättrar säkerhet och effektiviserar underhåll jämfört med JWT.
* **Tidslinje för migrering**
   * 1 maj 2023 - Meddelande om framtida borttagning.
   * 2 juni 2024 - Senaste datum för att skapa autentiseringsuppgifter för nytt tjänstkonto.
   * 27 januari 2025 - Slutet på livscykeln för tjänstkonton och API:er som använder dem kommer att upphöra att fungera.
* **&#x200B; särskild hänsyn för AEM** Webbseminariet behandlade hur migreringen påverkar AEM moln- och lokala kunder, inklusive specifika autentiseringsmönster och konfigurationer.
* **Automatiskt genererade integreringar** Automatiskt genererade integreringar migreras automatiskt av Adobe före tidsgränsen.
* **Support och dokumentation** Adobe tillhandahåller omfattande dokumentation och support för migreringsprocessen. Kunderna kan kontakta Adobe representanter eller professionella tjänster för att få hjälp.
* **Testar och validering** Du bör testa integreringar noggrant efter migrering och innan du tar bort gamla JWT-autentiseringsuppgifter.
* **Anpassade integreringar** Kunder med anpassade integreringar bör identifiera och planera för migrering så snart som möjligt, särskilt om tredjepartsleverantörer är inblandade.
