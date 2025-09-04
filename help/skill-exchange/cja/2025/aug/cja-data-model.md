---
title: Analysarkitekturen - Hur ni använder er Customer Journey Analytics datamodell
description: Lär dig strukturera CJA datamodeller med händelsehierarkier, attribuering och nyckeltal för att få djupare insikter om kundresan.
feature: Attribution
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 0
last-substantial-update: 2025-09-04T00:00:00Z
jira: KT-18813
source-git-commit: 124b52203b98a80dd9202dab1b0dbe575475a52b
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Analysarkitekturen: Hur ni använder er Customer Journey Analytics datamodell

En viktig aspekt när det gäller att skapa en CJA-datamodell är att förstå det hierarkiska förhållandet mellan olika kontaktpunkter och interaktioner. Detta utgör grunden för meningsfulla analyser och insikter.

Viktiga överväganden är

* Identifiera och mappa kundinteraktionspunkter i alla kanaler
* Skapa tydliga händelsehierarkier och relationer
* Definiera konsekventa attribueringsmodeller
* Skapa standardiserade mätvärden och KPI:er

Genom att strukturera dessa element på rätt sätt kan organisationer bättre spåra och analysera hela kundresan, vilket leder till mer åtgärdbara insikter och förbättrade beslutsfunktioner.

>[!VIDEO](https://video.tv.adobe.com/v/3471111/?learn=on&enablevpops)

## Låsa upp datamodellering för kraftfull analys

Upptäck hur effektiv dataarkitektur i Adobe Experience Platform (AEP) och Customer Journey Analytics (CJA) skapar åtgärdbara insikter och rapporter.

* **Schemadesign är viktigt** Alternativet mellan platta scheman, arrayer och arrayer av objekt påverkar direkt analysfunktionerna och rapporteringsflexibiliteten.
* **Omvandlingsprocess** Data som hämtas in till AEP måste vara genomtänkt strukturerade för att omformningen och användbarheten i CJA ska vara sömlös.
* **Behållarhierarkin** Händelse-, sessions- och personnivåer är avgörande för analyser på flera nivåer och korrekt rapportering.
* **Praktiska strategier** Främsta planering, schemastyrning och användning av plattformsfunktioner är avgörande för skalbara, framtidssäkra implementeringar.

Genom att kombinera dessa koncept kan teamen optimera sina analysarbetsflöden och få djupare affärsinsikter.

## Schematyper och användningsfall för dem

* **Platta scheman** Passar bäst för enkla 1:1-datarelationer. Idealiskt för grundläggande händelsespårning och enkla mätvärden/dimensioner.
* **Matriser** är användbara för listor med relaterade objekt (t.ex. produktkategorier, innehållstaggar). Varje arrayelement blir en individuell dimension för analys.
* **Arrayer av objekt** Utformade för komplexa användningsområden, som produktinköp, där varje objekt behåller sina egna egenskaper och relationer. Möjliggör detaljerad analys på objektnivå.
* **Välja Wisely** Välj det enklaste schema som uppfyller dina behov, men utnyttja arrayer och objekt för avancerade scenarier som kräver relationsbevarande.