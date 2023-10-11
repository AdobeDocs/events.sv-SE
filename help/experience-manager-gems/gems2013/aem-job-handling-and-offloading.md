---
title: Introduktion till jobbhantering och avlastning i AEM 5.6.1.
description: En teknisk introduktion av de avancerade jobbhanteringsfunktionerna. Jobbhantering är den underliggande infrastrukturen för funktioner som replikering och arbetsflödesbearbetning. Lär dig mer om identifieringsmodulen tillsammans med det förbättrade API:t för jobbbearbetning och nya funktioner.
uuid: 181e3781-8eca-4a5d-879e-15ae4e1f6649
discoiquuid: ee4cd526-7363-4b8e-ad26-c2c937b70327
targetaudience: target-audience advanced
exl-id: bd10465b-6f45-4117-b8a0-1310422f5825
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 2%

---

# Introduktion till jobbhantering och avlastning i AEM 5.6.1. {#introduction-of-job-handling-and-offloading-in-aem}

Jobbhantering är den underliggande infrastrukturen för funktioner som replikering och arbetsflödesbearbetning. Det här är en teknisk introduktion av de avancerade jobbhanteringsfunktionerna. Vi diskuterar den nya identifieringsmodulen tillsammans med det förbättrade API:t för jobbbearbetning och de nya funktionerna. Avlastningsramverket bygger på jobbhantering och identifiering och är inriktat på att distribuera jobb mellan icke-klustrade instanser. Vi ska titta närmare på hur avlastning utökar hanteringen av distribuerade jobb. Sedan tittar vi på hur den används för den aktuella implementeringen av arbetsflödesavlastning och hur man kan använda den i ett eget projekt.

>[!VIDEO](https://video.tv.adobe.com/v/19580/?quality=9)

*Levererat 24 juli 2013*

**Presenteras av:**

Carsten Ziegeler, Senior Developer, Adobe

Marc Pfaff, Lead Developer, Adobe

Presentatörsbilder - del 1

[Hämta fil](assets/jobhandling.pdf)

Presentatörsbilder - del 2

[Hämta fil](assets/offloading.pdf)

## Relaterade länkar {#related-links}

* [Apache Sling Eventing och Jobhandling](https://sling.apache.org/documentation/bundles/apache-sling-eventing-and-job-handling.html)
* [API för identifiering och dess implementeringar](https://sling.apache.org/documentation/bundles/discovery-api-and-impl.html)
* [Avlastar jobb](https://docs.adobe.com/docs/en/cq/current/deploying/offloading.html)
