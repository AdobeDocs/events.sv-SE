---
title: Optimera innehållsleverans - Frigör kraften i Edge Services
description: ATM Edge Delivery Services (EDS) förbättrar ATM med sammanställningsbara tjänster, snabba utvecklingscykler och höga fyrar, stöd för dokumentbaserad och WYSIWYG-baserad redigering, serverlös arkitektur, snabb framtagning av webbplatser och omfattande anpassningsmöjligheter.
solution: Experience Manager, Experience Manager as a Cloud Service
feature: Edge Delivery Services
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3589
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16631
source-git-commit: 47ae42d06ed311e60ebce194e0683bb95e8e5b69
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---


# Optimera innehållsleverans: Frigör kraften i Edge Services

Under det här seminariet kommer vi att ge en översikt över Edge Delivery Services (EDS) och dess arkitektur. Vi kommer att ta reda på hur EDS kan integreras med dokumentbaserad redigering och AEM via den universella redigeraren. En live-demo visar upp EDS i praktiken, följt av resurser för ytterligare utforskande och en session med Frågor och svar.

>[!VIDEO](https://video.tv.adobe.com/v/3440938/?learn=on&enablevpops)

## Viktiga uppgifter

### Introduktion till EDS

* EDS är en uppsättning sammansättningsbara tjänster som utformats för att förbättra ATM funktioner. &#x200B;
* Syftet är att leverera enastående upplevelser som driver engagemang och konverteringar med snabba utvecklingscykler och en 100-procentig fyndighetspoäng. &#x200B;

### Redigeringsalternativ

* **Dokumentbaserad redigering** Använder välbekanta verktyg som Microsoft Word eller Google Docs för att skapa innehåll, vilket gör det möjligt att snabbt skapa innehåll utan omfattande utbildning. &#x200B;
* **Universell redigerare** Tillhandahåller ett WYSIWYG-gränssnitt som liknar traditionella ATM, vilket gör att du kan skapa mer detaljerat och visuellt innehåll. &#x200B;

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
* Vi rekommenderar att man kontaktar Adobe för att få hjälp med olösta problem. &#x200B;