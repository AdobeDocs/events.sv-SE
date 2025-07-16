---
title: Adobe Pass - nytt REST API v2
description: Under den här sessionen fokuserar vi på att lansera Adobe nya REST API v2 och vägleda användarna genom migreringsprocessen.
role: Developer
solution: Pass
level: Beginner, Intermediate, Experienced
doc-type: Technical Video
duration: 3230
last-substantial-update: 2025-04-07T00:00:00Z
jira: KT-17685
hidefromtoc: true
exl-id: 745411bb-48d7-4410-a236-d02c2927ac1b
source-git-commit: 088615f28aa91dfd4ba119c11c4c9f8a89441d84
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Adobe Pass - nytt REST API v2

Under den här sessionen fokuserar vi på att lansera Adobe nya REST API v2 och vägleda användarna genom migreringsprocessen.

>[!VIDEO](https://video.tv.adobe.com/v/3457461/?learn=on&enablevpops)

## Viktiga högdagrar

* **Översikt och fördelar**

   * REST API v2 är utformat för modern, flexibel och skalbar autentisering, med hänsyn till efterfrågade händelser och scenarier med flera enheter.
   * Bland huvudförbättringarna märks förbättrad kryptering, sessionskonsekvens, SSO mellan olika enheter och utökad felinformation för snabbare felsökning.

* **Migreringssteg**

   * Användarna måste skapa nya registrerade program med REST API v2-scope.
   * Befintliga konfigurationer som enhetsidentifiering och MVPD-mappningar kan återanvändas.
   * Migreringen omfattar faser som registrering, konfiguration, autentisering, förauktorisering och auktorisering.

* **Funktionsförbättringar**

   * Enhetligt RESTful-API ersätter SDK:er för grannar och förenklar implementeringen på olika plattformar.
   * Stöd för flera autentiseringsprofiler inom samma session och sömlösa enhetsövergripande övergångar.
   * Förauktoriserings- och auktoriseringsflöden är fortfarande obligatoriska för innehållsåtkomst.

* **Tidslinje**

   * REST API v1 kommer att sluta ta emot uppdateringar i december 2025 och vara helt pensionerad i slutet av 2026.
   * Användarna uppmanas att slutföra migreringen långt före dessa deadlines.

* **Resurser och support**

   * Dokumentation, kokböcker och vanliga frågor finns på Adobe Experience League.
   * Adobe erbjuder sandlådemiljöer, Zendesk-biljetter och migreringsmöten för support.

* **Q&amp;A-markeringar**

   * REST API v2 kräver omautentisering eftersom den inte är bakåtkompatibel med v1.
   * Förhandsauktorisering är för användargränssnittsändamål, medan auktorisering krävs för medietoken.
   * Det finns stöd för enkel inloggning via en ny Adobe-tjänsttoken.
