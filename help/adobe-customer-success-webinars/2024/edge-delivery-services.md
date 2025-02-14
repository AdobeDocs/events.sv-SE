---
title: Optimera innehållsleverans - Frigör kraften i Edge Services
description: Sessionen med Edge Delivery Services (EDS) behandlade dess arkitektur, integrering med dokumentbaserad och AEM-baserad redigering, snabb framtagning av webbplatser, anpassningsalternativ och bästa praxis för att upprätthålla höga prestanda.
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
exl-id: 2057e491-9ec3-4bfe-b85a-6b74d70822bf
source-git-commit: 32060a6a0d2cc24b8dc09c8f5e9f9d9c679e6d3e
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Optimera innehållsleverans: Frigör kraften i Edge Services

Under det här seminariet kommer vi att ge en översikt över Edge Delivery Services (EDS) och dess arkitektur. Vi kommer att ta reda på hur EDS kan integreras med dokumentbaserad redigering och AEM-baserad redigering via den universella redigeraren. En live-demo visar upp EDS i praktiken, följt av resurser för ytterligare utforskande och en session med Frågor och svar.

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## Viktiga uppgifter

### Introduktion till EDS

* EDS är en uppsättning sammansättningsbara tjänster som utformats för att förbättra ATM funktioner. &#x200B;
* Syftet är att leverera enastående upplevelser som driver engagemang och konverteringar med snabba utvecklingscykler och en 100-procentig fyndighetspoäng. &#x200B;

### Redigeringsalternativ

* **Dokumentbaserad redigering** Använder välbekanta verktyg som Microsoft Word eller Google Docs för att skapa innehåll, vilket gör det möjligt att snabbt skapa innehåll utan omfattande utbildning. &#x200B;
* **Universell redigerare** Tillhandahåller ett WYSIWYG-gränssnitt som liknar traditionella ATM-webbplatser, vilket gör det möjligt att skapa mer detaljerat och visuellt innehåll. &#x200B;

### Arkitektur

* EDS kan integreras i Amazon Cloud Service. &#x200B;
* Den stöder serverlös implementering och kan fungera utan någon traditionell författare eller utgivarinstans. &#x200B;
* Två cachenivåer kan implementeras: på kundinfrastrukturnivå och EDS-nivå. &#x200B;

### Innehållshantering

* För dokumentbaserad redigering krävs ett GitHub-konto, Google Drive eller Microsoft SharePoint, ett plugin-program för sidosparkning och ett kodsynkroniseringsverktyg. &#x200B;
* EDS med IAM-redigering kräver ett GitHub-konto, en IAM som molntjänstlicens och ett kodsynkroniseringsverktyg.

### Utveckling och driftsättning

* Det går snabbt att skapa en webbplats med EDS, vilket ofta tar mindre än en dag. &#x200B;
* Lokal utveckling kan göras med kommandot aem up för att skapa en lokal version av webbplatsen.
* Ändringarna kan implementeras i grenar för testning innan de sammanfogas i huvudgrenen. &#x200B;

### Anpassning och utbyggbarhet

* Anpassade komponenter kan skapas med enkel CSS och JavaScript. &#x200B;
* Arkitekturen tillåter integreringar från tredje part och anpassade redigeringskällor.

### Bästa praxis

* Vi rekommenderar att du använder vanilj JavaScript och CSS för att behålla höga fyr-resultat.
* Alla introduktioner av bibliotek som React bör noggrant övervägas och testas för att undvika prestandaförsämring.

### Support och dokumentation

* Det finns omfattande dokumentation som vägleder användarna genom installations- och anpassningsprocessen. &#x200B;
* Vi rekommenderar att du kontaktar Adobe support för olösta problem. &#x200B;
