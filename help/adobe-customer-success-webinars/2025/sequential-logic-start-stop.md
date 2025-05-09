---
title: Mastering Sequential Logic in Adobe Analytics and Customer Journey Analytics - Starts and Stops
description: Använd sekventiell logik i Adobe Analytics med avancerad segmentering, omfångskontroller och härledda fält för att identifiera kundbeteendemönster och förbättra datakvaliteten.
solution: Analytics, Customer Journey Analytics
role: Developer
level: Intermediate
doc-type: Event
duration: 3370
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18017
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Mastering Sequential Logic in Adobe Analytics and Customer Journey Analytics: Starts and Stops

Under den här sessionen ska vi titta närmare på hur du konfigurerar sekvenser med operatorn THEN i Adobe Analytics (AA) och Customer Journey Analytics (CJA). Lär dig att hämta exakta delmängder av aktivitet genom att kombinera ENDAST EFTER/ENDAST FÖRE SEKVENSEN med EXCLUDE-kontrollpunkter.

## Diskussionspunkter

* Snabbgranskning av fristående sekventiella logikoperatorer och visuella ramverk.
* Beskriv hur EXCLUDE påverkar resultatet av sekvenser med ENDAST AFTER/BEFORE-SEKVENSEN.
* Aktuella användningsexempel och demonstrationer som visar hur du kan använda metoderna för ditt företag.

>[!VIDEO](https://video.tv.adobe.com/v/3458040/?learn=on&enablevpops)

## Högdagrar


1. Sekventiell logik och segmentering i analyser

   * Mötet fokuserade på avancerade tekniker för att tillämpa sekventiell logik i analyser, och betonade vikten av att förstå start- och stoppunkter i datasekvenser för att analysera kundbeteenden effektivt.
   * Sekventiella operatorer diskuterades som verktyg för att identifiera mönster som &quot;webbträff följt av e-postträff&quot; eller &quot;programinlämning följt av efterföljande sessioner&quot;.
   * Den giriga typen av segmentlogik markerades, vilket förklarar hur den returnerar den största möjliga datauppsättningen om den inte begränsas av ytterligare villkor.
   * Tekniker för att definiera omfång, som&quot;endast före&quot; och&quot;endast efter&quot;-sekvenser, introducerades för att studera delmängder av data baserat på specifika affärsfrågor.
   * Användningen av kontrollpunkter, närhetsvillkor och uteslutningskriterier förklarades för att förfina dataanalysen och besvara komplexa affärsfrågor.

2. Hantera flera intressepunkter i dataanalys

   * Andy diskuterade scenarier där kunderna har flera inskickade ansökningar och behovet av att analysera beteenden efter varje inskickat material snarare än bara det första.
   * Man tog itu med problem som överlappande ansökningar och definiering av huruvida de ursprungliga intressepunkterna skulle inkluderas eller inte.
   * Vikten av att förtydliga antaganden och förfiningslogik för att hantera flera förekomster av en sekvens betonades, vilket säkerställer en korrekt analys av kundbeteenden under hela deras livscykel.

3. Avancerade tekniker för att stoppa datamatchning

   * Under sessionen introducerades metoder för att stoppa datamatchning vid specifika kontrollpunkter med hjälp av undantagskriterier, vilket gör att analytiker kan studera data mellan definierade start- och stopppunkter.
   * Exemplen inkluderar analys av beteenden mellan&quot;webbsuccé följt av mobilappsinteraktion&quot; och att stoppa vid&quot;e-postinteraktion&quot;.
   * Användningen av villkoren &quot;inom&quot; och &quot;efter&quot; förklarades för att tillämpa striktare närhetsregler och undvika oavsiktliga resultat från logik.
   * Andy visade hur dessa tekniker kan användas för att studera kundbeteenden i förhållande till specifika händelser, som inskickade ansökningar.

4. Validerar och finjusterar dataanalyslogik

   * Andy betonade vikten av att validera antaganden och testlogik för att säkerställa korrekta resultat, eftersom misstag i segmentuppbyggnaden eller dataantaganden är vanliga.
   * Exempel på oväntade resultat på grund av girig logik delades, vilket visar att det behövs strikta villkor som &quot;inom en händelse&quot; eller &quot;inom en session&quot;.
   * Valideringsriktmärken, t.ex. små datauppsättningar med kända egenskaper, rekommenderades för att testa och förfina analysmetoder.

5. Tillämpning av sekventiell logik i verkliga användningsfall

   * Andy gav exempel på verkliga användningsfall, som att analysera kundbeteenden efter att ha skickat in ansökningar eller identifiera vanliga åtgärder efter köp eller negativa granskningar.
   * Sessionen visade hur sekventiell logik kan tillämpas på studiemönster som &quot;första sessionen efter tillämpning&quot; eller &quot;andra sessionen efter tillämpning&quot; för flera förekomster.
   * Betydelsen av skalningsanalys för bredare datauppsättningar, samtidigt som noggrannheten bibehålls, diskuterades med exempel på överlappande effekter i data på sessionsnivå.

6. Använda härledda fält för flexibel analys

   * Andy introducerade begreppet att använda härledda fält i Adobe Customer Journey Analytics (CJA) för att dynamiskt definiera ögonblick av intresse och minska behovet av att redigera flera filter för varje analys.
   * Med hjälp av härledda fält kan analytiker skapa filter i förhållande till ett enda fält, vilket möjliggör snabba justeringar för att studera olika intressepunkter, t.ex. produktspecifika program eller andra kundhändelser.

7. Praktiska program och framtida planer

   * Andy delade planer för nästa webbseminarium, som fokuserar på mallar, mallar och praktiska applikationer för de koncept som diskuterades, och övergick från utbildning till konkreta användningsfall.
   * Mötet avslutades med en begäran om feedback via en omröstning för att fastställa intresset för framtida ämnen och säkerställa en anpassning till deltagarnas mål.
   * Andy belyste Ultimate Success-teamets mikroengagemang och erbjöd riktade coachningssessioner för att hjälpa företag att tillämpa dessa koncept på sina specifika användningsfall.

8. Dela material och uppföljningsåtgärder

   * Andy bekräftade att webbseminariematerialet, inklusive inspelningar och blogginlägg, kommer att delas med deltagarna, vilket utgör en dokumenterad form av sessionens innehåll.
   * Deltagarna uppmanades att kontakta sina TAM eller CSM för ytterligare hjälp och att utforska Ultimate Success licensiering för personaliserade kodningssessioner.
