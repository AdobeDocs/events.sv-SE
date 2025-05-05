---
title: Bästa praxis för leverans av prestanda
description: Optimera medieleveransen och prestandan med Dynamic Media genom att utnyttja adaptiv strömning, anpassade videoprofiler, SEO, bästa praxis, bildoptimering, masshantering av innehåll, visningsförinställningar, cache-ogiltigförklaring och smart bildhantering.
feature: Dynamic Media, Video, SEO Optimization, Smart Imaging, Viewer Presets, Best Practices
topic: Content Management
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1596
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16572
exl-id: a1920020-b9ce-43be-8f9e-e52aac68da7b
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Bästa praxis för leverans av prestanda

Följ Riya Midha, Sr. Product Manager på Adobe, och utforska de bästa sätten att konfigurera Adobe Experience Manager Assets Dynamic Media. Lär dig hur du optimerar leverans av resurser, förbättrar direktuppspelad video, konfigurerar visningsprogram samt mäter och förbättrar prestanda.

>[!VIDEO](https://video.tv.adobe.com/v/3440421/?learn=on&enablevpops&captions=swe)

## Community-diskussion

Fortsätt konversationen i [diskussionen](https://adobe.ly/3YGedpb) i Adobe Developers Live Community.

## Viktiga uppgifter

* **Dynamic Media Capabilities** Dynamic Media möjliggör snabb och flexibel leverans av personaliserade medier av hög kvalitet över olika enheter, som hanterar över 9 biljoner medieleveranser årligen och dagliga toppvolymer på upp till 69 miljarder mediefiler.
* **Adaptiv strömning** Om adaptiv strömning används för videoleverans minskar buffringen avsevärt. Ett test visade en minskning av buffertantalet från 50 till 5 i en 60-sekundersvideo med en begränsad bandbredd på 5 Mbit/s.
* **Videoprofiler** Om du skapar anpassade videoprofiler med olika kvalitetskoder får du optimala videoprestanda för olika nätverksförhållanden.
* **SEO Best Practices**
   * Använd regeluppsättningar för att skapa beskrivande URL:er för bättre SEO.
   * Lägg till alt-text och rubrikattribut i bilder.
   * Använd smart bildbehandling och de senaste bildformaten som WebP för bättre sökresultat.
* **Bildoptimering**
   * Använd skalparametrar för att justera bildupplösningen baserat på skärmstorleken.
   * Undvik att använda 100 % bildkvalitet. Använd i stället ett intervall på 80-90 % för att minska filstorleken utan märkbar kvalitetsförlust.
   * Använd skärpeparametrar för att göra texten tydligare i bilder.
* **Hantering av massinnehåll**
   * Segmentera innehåll som är avsett för dynamisk medieleverans från annat innehåll.
   * Använd selektiv synkronisering för att optimera bearbetningstiden och förbättra time-to-market.
* **Förinställningar för visningsprogram** Anpassa visningsprogrammets utseende och beteende med hjälp av förinställningar för visningsprogram utan kodändringar. Exempel är att redigera uppspelnings-/pausknappar, aktivera automatisk uppspelning och slinga samt lägga till bildövertäckningar.
* **Cacheinvalidering** Använd cacheogiltigförklaring för att omedelbart spegla ändringar som gjorts i redan publicerade resurser, utan att standardinställningen för 10-timmars TTL har överskridits.
* **Övervakning och felsökning** Använd verktyg som AEM skrivbordsapp och felsökningssida för frågor för att spåra bearbetningsjobb och identifiera obearbetade resurser.
* **Smart bildåtergivning** Smart bildåtergivning är aktiverat som standard på alla domäner, vilket minskar bildfilernas storlek och förbättrar inläsningstiden.
