---
title: AEM Sites-effektivitet - Prestandaoptimering, konfiguration och felsökning
description: 'Grundläggande information om att felsöka Adobe Experience Manager-webbplatser (AEM). Oavsett om du har prestandaproblem eller har att göra med komplexa konfigurationer kommer den här sessionen att ge praktiska kunskaper för att underhålla och optimera din AEM. Vi prioriterar live-demos framför bilder och ger praktiska erfarenheter av att tackla utmaningar i verkligheten. ​Viktiga diskussionspunkter: - konfiguration och domänmappning av virtuella värdar - prestandaproblem - auktorisering, identifiering, användarbehörigheter'
solution: Experience Manager
version: Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
source-git-commit: 3f245f71cd4db5097b5a9e712114112451d899e4
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# AEM Sites-effektivitet: Prestandaoptimering, konfiguration och felsökning

I det här webbinariet kommer vi att dyka upp i grunderna för felsökning av Adobe Experience Manager-sajter (AEM). Oavsett om du har prestandaproblem eller har att göra med komplexa konfigurationer kommer den här sessionen att ge praktiska kunskaper för att underhålla och optimera din AEM. Vi prioriterar live-demos framför bilder och ger praktiska erfarenheter av att tackla utmaningar i verkligheten. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3435114/?learn=on)

## Viktiga punkter

Webbseminariet fokuserar på effektiviteten hos AMP-webbplatser, inklusive prestandaoptimering, konfiguration och felsökning.

### Dispatcher Configuration

* Hur viktig dispatchern är när det gäller att leverera prestandawebbplatser.
* Viktiga aspekter av dispatcherkonfigurationen: konfiguration av virtuell värd, domänmappning med cachestruktur samt regelbunden rapportering och omdirigering.

### Rights Management

* Bästa tillvägagångssätt: tillämpa rättigheter på grupper, undvika neka-satser och undvika övertekniska åtgärder.
* Använd det Netcentric ACL-verktyget för att hantera rättigheter via en Yaml-fil, vilket gör det enkelt att driftsätta och spåra.

### Prestandaproblem

* Viktigt att identifiera deltoner i synkroniseringsåtgärder för att undvika tömningar av hela cachen.
* Undvik stora sidoperationer under kontorstid.
* Förenkla arbetsflödena med nödvändiga steg.
* Var försiktig med tredjepartssystemprocesser i redigeringssystem, särskilt med verktyg som ImageMagick.
* Undvik synkroniserade begäranden till tredjepartssystem som inte kan hantera belastningen.
* Hantera tunga anpassade komponenter för att undvika prestandaförsämringar.
* Övervaka om det finns långa sessioner för att förhindra att segment hittas.