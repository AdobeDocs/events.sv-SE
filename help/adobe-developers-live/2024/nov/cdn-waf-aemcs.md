---
title: Konfiguration av CDN och WAF i Adobe Experience Manager as a Cloud Service
description: Förbättra prestanda och säkerhet för Adobe Experience Manager as a Cloud Service-program med anpassningsbara CDN-regler, WAF-skydd och Config Pipeline, som delas av Adobe-experter.
feature: Security
topic: Performance, Security
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2211
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16574
exl-id: a9f38e79-c707-443d-8b2f-e534ce4dd43d
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Konfiguration av CDN och WAF i Adobe Experience Manager as a Cloud Service

Utnyttja Adobe Managed CDN till fullo med anpassningsbara CDN-regler, WAF-skydd och Config Pipeline. Marius Petria, Sr. Computer Scientist på Adobe, Quentin Vecchio, Software Development Engineer på Adobe och Florian Froese, Software Development Engineer på Adobe, delar strategier för att förbättra prestanda och säkerhet i Adobe Experience Manager as a Cloud Service-applikationer.

>[!VIDEO](https://video.tv.adobe.com/v/3440606/?learn=on&enablevpops&captions=swe)

## Community-diskussion

Fortsätt konversationen i [diskussionen](https://adobe.ly/3O0TyYa) i Adobe Developers Live Community.

## Viktiga punkter

* **Introduktion av nya konfigurationsfunktioner** Presentationen introducerar nya konfigurationsfunktioner för CDN i en molntjänst, med fokus på möjligheten att konfigurera CDN för olika användningsfall.
* **Konfigurationsalternativ för CDN** De nya alternativen tillåter interaktion med HTTP-begäranden och svar, t.ex. tillägg/borttagning av rubriker, omskrivning av begäransökvägar, blockering av trafik, omdirigering av klienter och proxering till olika ursprung.
* **Säkerhetsförbättringar** Bland de nya funktionerna finns trafikfilterregler för att blockera eller logga trafik baserat på begärandemönster och introduktionen av M WAF för avancerat skydd mot webbattacker som SQL-injektion och XSS.
* **Deklarativ konfiguration** Konfigurationen görs med YAML-filer och distribueras via en konfigurationsprocess i Cloud Manager, vilket gör den till en snabb och enkel process.
* **Transformeringar av begäranden och svar** De nya funktionerna gör att det går att normalisera URL-adresser och ta bort onödiga frågeparametrar, och att göra svarsomformningar för att ange rubriker innan svar skickas till klienter.
* **Trafikfilter och hastighetsbegränsning** Trafikfilter kan blockera specifika IP-adresser eller länder och implementera hastighetsbegränsning för att skydda mot DDoS-attacker. Hastighetsbegränsning kan konfigureras baserat på olika kriterier som klient-IP, användaragent och sökväg för begäran.
* **Övervaknings- och analysverktygen** Adobe tillhandahåller verktyg som Elasticsearch/Kibana och Splunk-instrumentpaneler för att analysera trafik och användning, vilket hjälper till att identifiera och mildra potentiella säkerhetshot.
* **Praktisk demo** Presentationen innehåller en demonstration av hur du distribuerar CDN-konfigurationer med Cloud Manager och hur du hanterar fel och validerar konfigurationer lokalt med AEM.
