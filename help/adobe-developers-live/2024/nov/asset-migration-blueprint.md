---
title: Assets Migration Blue
description: Lär dig hur du migrerar ett gammalt resurshanteringssystem till Adobe Experience Manager Assets med insikter från Achim Koch, som omfattar intressentanalys, resursplanering, dataomvandling och metodtips som att använda CSV-filer för datahantering.
feature: Migration
topic: Migration
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1690
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16576
exl-id: f588055b-05c7-44df-be67-799a0e3ee1ed
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Assets Migration Blue

Träffa Achim Koch, Principal Technical Architect på Adobe, och lär dig hur du migrerar en äldre DAM till Adobe Experience Manager Assets. Få insikter i intressentanalys, resursplanering, dataomvandling och bästa praxis, som att använda CSV-filer för datahantering. Bygg en färdplan för era egna Adobe Experience Manager-migreringsprojekt.

>[!VIDEO](https://video.tv.adobe.com/v/3440403/?learn=on&enablevpops)

## Community-diskussion

Fortsätt konversationen i [diskussionen](https://adobe.ly/4hKHpnF) i Adobe Developers Live Community.

## Viktiga uppgifter

* **Inget körklart verktyg för migrering** Det finns inget enskilt verktyg som kan migrera från olika äldre system till Adobe Experience Manager (AEM) på grund av produktens och de anpassade lösningarnas mångfald.

* **Fem migreringssteg**

   * Projektplanering
   * Implementeringsplanering
   * AEM
   * Implementering av migreringsskript
   * Migreringskörning

* **Intressentdeltagande** Det är viktigt att identifiera och engagera intressenter som sponsorer, företagsanvändare, IT-systemadministratörer och äldre systemsupport.

* **Resurs- och tidsplanering** Kontrollera att det finns resurser tillgängliga och planera runt helger, högsta verksamhetstid och icke-begränsade fönster.

* **Teknisk planering** Detta omfattar kravanalys, dataomvandling och infrastrukturplanering.

* **Interaktiv processmigrering** innebär flera iterationer av skriptkörning, analys, feedback och anpassning.

* **CSV-filer** är att föredra om du vill att de ska vara lätta att använda och läsa under migreringsprocessen.

* **Skriptspråk** Node.js rekommenderas för CSV, AWS och HTTP, och för att det är ett bra tillfälle att lära sig JavaScript.

* **Kvalitet och repeterbarhet** Se till att datamigreringen håller hög kvalitet, att originaldata och CSV-filer är referensdata och gör processen upprepningsbar.

* **Frys innehåll** Deklarera frysning av innehåll under migreringen för att förhindra att nya data läggs till efter att ögonblicksbilden har tagits.

* **Verktyg och tips** Använd verktyg som VS-kod med Regnbåge-CSV-tillägget och överväg byteordningsmarkeringen (BOM) för UTF-8-textfiler.

* **Affärsgodkännande** Bevara tiden för testning och inhämtning av officiellt affärsgodkännande efter migrering för att lyfta innehållets frysning.
