---
title: AEM GEM - Komma igång med Adobe Managed CDN
description: Lär dig hur du konfigurerar hanterad CDN för Adobe i AEM Cloud Service för att förbättra prestanda och säkerhet med nya CDN-konfigurationsfunktioner.
role: Developer, User
level: Intermediate
doc-type: Event
duration: 3438
last-substantial-update: 2025-01-30T00:00:00Z
jira: KT-17227
source-git-commit: 1cfa9cdb0e973e6d088b1faeaa63539b0a7fba36
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---


# AEM GEM - Komma igång med Adobe Managed CDN

Lär dig mer om hanterad CDN i AEM Cloud Service och hur den kan konfigureras. Följ oss och utforska de nya CDN-konfigurationsfunktionerna som kan användas för att förbättra både prestanda och säkerhet i dina AEM as a Cloud Service-program. I den här sessionen kommer du att upptäcka

* Vad är Adobe CDN?
* Relevanta topologier för AEMaaCS och Edge Delivery Services
* Vanliga användningsområden som kan implementeras med CDN-regler
* Så här använder du RDE:er för att snabbt testa och distribuera CDN-konfigurationer

>[!VIDEO](https://video.tv.adobe.com/v/3443168/?learn=on&enablevpops)

*Inspelat den 22 januari 2025*

Har du en fråga, kanske en kommentar?  Gå med i diskussionen i [Experience League Communities](https://adobe.ly/4haufPK)!

## Viktiga uppgifter

### Viktiga funktioner för hanterad CDN i Adobe

* **Anpassade domäner och certifikat** Grundläggande för att skapa säkra anslutningar för anpassade domäner och certifikat.
* **Cachelagring** Att leverera HTTP-svar från cachen är betydligt snabbare (under 10 millisekunder) jämfört med att hämta från ursprungsläget (hundratals millisekunder).
* **Körklar och anpassad CDN** Adobe ger ett körklart CDN, men användare kan också ta med sitt eget CDN.

### Konfigurationsalternativ

* **Begär omformningar** Ändra huvuden, skriv om sökvägar, blocktrafik och omdirigeringsbegäranden.
* **Trafikfilter** Blockera eller tillåt trafik baserat på specifika regler.
* **Autentisering** Stöd för edge-nyckel, punch-nyckel och grundläggande autentisering.
* **Ursprungsväljare** Proxybegäranden till olika ursprung baserat på definierade regler.
* **Svarsomvandlingar** Ändra svarshuvuden och status.

### Driftsättning och anpassning

* **Konfigurationspipeline** Distribuera YAML-filer för att konfigurera CDN-regler.
* **Trafikskydd** Använd trafikfilterregler för att blockera, logga och avisera trafik baserat på mönster.
* **Hastighetsbegränsning** Protect mot DDoS-attacker genom att begränsa antalet begäranden per IP.

### Verktyg och analys

* **Elasticsearch Kibana Stack** Analysera användning och trafik med de angivna instrumentpanelerna.
* **Logga vidarebefordran** Vidarebefordrar till en Splunk-instans för analys.

### Demonstrationer

* **Distribuerar konfigurationer** Visar distribuering av trafikfilterregler och omdirigeringar.
* **Autentisering och ursprungsval** Visar hur du konfigurerar grundläggande autentisering och proxytrafik till olika ursprung.

### Bästa praxis

* **Snabba svar** Se till att det finns snabba svar från originalen för att undvika sårbarheter.
* **Bra cachning** Använd cachning för att hantera trafiken effektivt.
* **Använd instrumentpaneler** Analysera trafik och användning för att ange lämpliga hastighetsbegränsningar.
* **Kombinera strategier** Använd olika hastighetsbegränsande strategier för bättre skydd.
* **Ange aviseringar** Få aviseringar när webbplatsen attackeras.
* **Testregler** Börja med att logga åtgärder innan du blockerar för att se till att reglerna fungerar som förväntat.

### Kontakt och feedback

* **Feedback och användningsfall** Kontakta teamet för mer avancerade användningsfall och feedback.
* **Framtida sessioner** Delta i omröstningar för att föreslå ämnen för framtida sessioner.