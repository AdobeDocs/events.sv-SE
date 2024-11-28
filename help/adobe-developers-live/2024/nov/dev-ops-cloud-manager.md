---
title: Effektivisera DevOps med Cloud Manager
description: Optimera arbetsflödena för driftsättning med den nya funktionen "Bring Your Own Git" i AMP Cloud Manager, som möjliggör direkt integrering av externa Git-databaser, som stöder en strategi där man kan skifta-vänstra för tidig kodkvalitetskontroll samt förbättrar effektiviteten och anpassningsbarheten.
solution: Experience Manager, Experience Manager Cloud Manager
feature: Git Repositories, CI-CD Pipeline
topic: Integrations
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1034
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16547
source-git-commit: a5b6c2c3150fcc98686fe74d68f186bfe4e1befa
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---


# Effektivisera DevOps med Cloud Manager

Effektiva DevOps-rutiner är nödvändiga för att leverera upplevelser i stor skala. Adrian Tanase, Software Development Engineer på Adobe, undersöker hur Adobe Experience Manager Cloud Manager kan effektivisera arbetsflöden för driftsättning, förbättra automatiseringen och stödja kontinuerlig integrering och leverans (CI/CD).

>[!VIDEO](https://video.tv.adobe.com/v/3439904/?learn=on&enablevpops)

## Community-diskussion

Fortsätt konversationen i [diskussionen](https://adobe.ly/3Ywf7Vm) i Adobe Developers Live Community.

## Viktiga uppgifter

* **Adriana Clayton från Adobe introducerade en ny funktion i AMP Cloud Manager som hette &quot;Bring Your Own Git&quot;.**
* **Syfte med funktionen** Funktionen är utformad för att optimera arbetsflöden för distribution, vilket gör dem snabbare, effektivare och anpassningsbara för de leverantörer som du föredrar.
* **Utmaningar som har åtgärdats** Funktionen åtgärdar komplexiteten i synkroniseringen av externa Git-databaser med Adobe Git-databaser, som lägger till extra steg och tid i distributionsprocessen.
* **Lösning** &quot;Bring Your Own Git&quot; tillåter direktanslutning av privata och offentliga externa Git-databaser till Cloud Manager-pipelines, vilket gör det möjligt att omedelbart se kodändringar och köra åtgärder innan kodsammanslagningen.
* **Byt vänsterstrategi** Integreringen har stöd för en vänsterskiktsstrategi, vilket gör att kodkvalitetskontroller kan köras tidigare i utvecklingsprocessen, vilket ger utvecklarna snabb feedback.
* **Demo och validering** En demonstration om hur du integrerar databaser och validerar dem med Cloud Manager, inklusive steg för GitHub- och Bitbucket-databaser.
* **Kundpåverkan** Sedan den allmänna tillgängligheten har över 130 kunder anslutit till sina databaser, vilket förhindrar att fler än 2 500 pull-begäranden med kodkvalitetsproblem når upp till produktionen.
* **Framtida förbättringar** avser att utöka funktionen så att den omfattar rapporter direkt i GitLab och Bitbucket, och att utöka&quot;Bring Your Own Git&quot; till avancerade leveranstjänster för större flexibilitet.
* **Uppmuntra till feedback** Kunder uppmuntras att ge feedback och delta i den tidiga adopterfasen för andra databaser än GitHub.
