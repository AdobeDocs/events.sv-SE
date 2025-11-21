---
title: Navigera enkelt i Workfront API och Fusion Changes for Multi-Select Fields
description: Läs mer om kommande ändringar i Adobe Workfront API och Fusion, inklusive flervalsuppdateringar, versionshantering av händelseprenumerationer och strategier för att förhindra förändringar.
feature: Workfront API, Workfront Fusion, Workfront Integrations and Apps
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3172
last-substantial-update: 2025-08-08T00:00:00Z
jira: KT-18631
exl-id: 8581b9e5-674b-447a-8a52-1217d197891a
source-git-commit: 48d93e64b075db84d164a743db97fa0202b3e26c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Navigera enkelt i Workfront API och Fusion Changes for Multi-Select Fields

Den här workshopen spelades in den 25 juni 2025 och Andy Hess presenterade en demo som delade de kommande förändringarna av Workfront API och Fusion.

>[!VIDEO](https://video.tv.adobe.com/v/3469978/?learn=on&enablevpops)

## Resurser

Tillsammans med on-demand-inspelningen har vi lagt in bildspel och ytterligare resurser:
* [Bildband, PDF](https://workfront-experience.s3.us-west-2.amazonaws.com/Training/Guides/Customer+Success+at+Scale/Navigating+the+API+and+Fusion+Changes+for+Multi-Select+Fields+with+Ease+062425.pdf)
* Ett evenemang som anordnades i samarbete med Adobe Software Development Team hölls i början av maj om ändringarna av Event-prenumerationer om du vill veta mer om det specifika området, [[Händelseuppföljning] Bevara dina Fusion-scenarier under Evenemangsprenumerationer v2-uppgradering](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/m-p/754182#M4041)

## Viktiga åtgärder och resurser

* Ändringar av Workfront API-fält med flera val kommer i version 21 (oktober 2025) för att säkerställa ett konsekvent JSON-arrayformat i stället för blandade sträng-/arraysvar
* Versionshantering för händelseprenumerationer introduceras - version 2 returnerar alltid flervalsfält som arrayer, medan version 1 behåller det nuvarande inkonsekventa beteendet
* Prenumerationer på nya evenemang får automatiskt version 2 som standard, och alla prenumerationer uppgraderas automatiskt till version 2 i mitten av januari 2026
* En ny version av Workfront Connector släpps senare i år med manuell uppgraderingsprocess för att bevara modulmappningen och förhindra att ändringar bryts
* Fusion AI-assistenten är för närvarande tillgänglig men kräver ett signerat AI-avtal och korrekt licensieringsinställning. Kontakta din kontoansvarige om du har frågor eller vill veta mer. [Mer information om hur du använder AI i Fusion](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/manage-scenarios/fusion-ai-assistant)
* [Workfront Fusion-mallar är tillgängliga](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/create-and-manage-templates/currently-available-fusion-templates)
* [Anropa för Fusion-mallar](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/call-for-fusion-template-ideas/m-p/732085#M3686)- Lägg till de här om du har förslag på nya Fusion-mallar! Det är här teamet hämtar idéer från  

Om du har frågor om uppföljning kan du svara på detta [Experience League Community Post](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-navigating-the-workfront-api-and-fusion-changes/td-p/761253)! 

Vi hoppas att vi får träffa dig på våra framtida kundframgångar!  Se till att du checkar ut [Workfront Events](https://experienceleague.adobe.com/events/?lang=sv-SE&filters=Workfront) på Experience League för att få en fullständig lista och för att registrera dig.
