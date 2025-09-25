---
title: Användningsexempel för identitetsdiagram och felsökning
description: Läs om hur Adobe Experience Platform Identity Service hanterar segmentering, aktivering och sammanslagning av profiler för att lösa marknadsföringsutmaningar i verkligheten.
feature: Identities, Profiles, Segments
solution: Experience Platform
role: Admin, Developer, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3232
last-substantial-update: 2025-09-24T00:00:00Z
jira: KT-19286
source-git-commit: ae72352725cfb057cab771b08c4419c11e17e385
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# Användningsexempel för identitetsdiagram och felsökning

Det här webbinariet ger en djupgående förståelse för hur Adobe Experience Platform Identity Service fungerar för att ge digitala marknadsföringsansvariga den kunskap de behöver för att utforma segmenterings- och aktiveringsscenarier. Genom att förstå exakt hur multienheter och andra användningsfall fungerar är realistiska lösningar möjliga.

* Större förståelse för egenskaperna/begränsningarna i profilsammanfogning. På så sätt kan en större grupp intressenter utforma segmenterings- och aktiveringsscenarier.
* Första radens identifiering av möjliga problem med komprimering av profiler.
* Identitetstjänst jämfört med kundprofil i realtid.

>[!VIDEO](https://video.tv.adobe.com/v/3475214/?learn=on&enablevpops)

## Grundläggande om identitetsdiagram

Identitetsdiagrammet är ryggraden i enhetligheten i kunddata i Adobe Experience Platform. Den länkar flera identifierare - som e-post, CRM-ID, förmånskort, cookies och enhets-ID:n - mellan kanaler och enheter.

* **Identitetstjänsten** Skapar diagrammet genom att koppla identifieringspar från dataöverföring och händelser.
* **Profiltjänst** Sammanfogar profilfragment med hjälp av diagrammet, sammanfogningsattribut, beteenden och identiteter i en enhetlig kundvy.
* **Sammanslagningsprinciper** Bestäm hur datakonflikter ska lösas, antingen med hjälp av senaste (tidsstämpel) eller datauppsättningsutfärdare.
* **Affärspåverkan** Korrekt konfiguration säkerställer korrekt rapportering, rätt till marknadsföring och efterlevnad av regler som GDPR.

## Låsa upp kunddataanslutningar

Upptäck hur Adobe Experience Platform identitetsdiagram förenar kunddata för djupare insikter och bättre affärsresultat.

* **Identitetsdiagram** Länka kundinteraktioner mellan enheter och kanaler, vilket skapar en omfattande profil.
* **Namnområdesprioriteter** Affärsdrivna regler avgör vilka identifierare (e-post, CRM-ID, förmånskort) som är ankarprofiler och löser konflikter.
* **Sammanslagningsprinciper** Styr hur data från olika källor kombineras med hjälp av tidsstämplar eller datauppsättningsprioritet.
* **Diagramkomprimering och korrigering** Delade enheter, ovaliderade data eller implementeringsfel kan fragmentprofiler. Simuleringsverktyg och reparationsjobb hjälper till att återställa noggrannheten.

Genom att förstå dessa begrepp kan organisationer maximera datavärdet, säkerställa regelefterlevnad och leverera personaliserade upplevelser.

