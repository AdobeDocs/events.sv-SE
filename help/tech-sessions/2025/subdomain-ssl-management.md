---
title: Tech Sessions - Adobe Campaign Subdomain and SSL management in the Control Panel
description: Lär dig hur du delegerar och konfigurerar underdomäner på Adobe Campaign Kontrollpanel, konfigurerar SSL-certifikat och övervakar konfigurationen för att säkerställa säker e-postleverans.
solution: Campaign
feature: Subdomains and Certificates
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3409
last-substantial-update: 2025-09-05T00:00:00Z
jira: KT-18866
source-git-commit: 18ce421793d97372198151afc92b24f3bed053a8
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Tech Sessions: Adobe Campaign Subdomain and SSL management in the Control Panel

Under den här sessionen utforskar vi koncepten med delegering och konfigurering av underdomäner inom Adobe Campaign, inklusive installation av SSL-certifikat för att skydda underdomäner.

Lär dig vad en underdomän är, dess syften och de delegeringsmetoder som gör att Adobe kan använda den effektivt. Sessionen behandlar också principerna för att skydda en underdomän med SSL-certifikat och bästa praxis för att upprätthålla en säker miljö.

Vi ger stegvis vägledning om hur du konfigurerar underdomäner med hjälp av självbetjäningskontrollpanelen, där du kan lyfta fram potentiella hinder och hur du kan ta itu med dem. Deltagarna får praktiska kunskaper för att säkerställa smidig installation och säker hantering av sina underdomäner.

Oavsett om du är administratör, utvecklare eller plattformsägare får du under den här sessionen de kunskaper du behöver för att konfigurera och skydda underdomäner i Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3471391/?learn=on&enablevpops)

## Mastering av hantering av underdomäner i Adobe Campaign

Lås upp grunderna för delegering, konfiguration och säkerhet av underdomäner för Adobe Campaign e-postkommunikation:

* **Delegering av underdomän** Välj mellan fullständig delegering eller CNAME-delegering för att styra hur Adobe hanterar din DNS och e-postleverans.
* **Installation av DNS och SSL** Korrekt konfigurering av MX-, SPF-, DKIM-, DMARC- och SSL-certifikat är avgörande för säkra, välrenommerade e-postutskick.
* **Kontrollpanelen** Använd Adobe självbetjäningsverktyg för att effektivisera konfigurationen av underdomäner, övervaka poster och hantera SSL-certifikat.
* **Vanliga fallgropar** Undvik förseningar och fel genom att förstå tidslinjer för granskningen, krav på registrering och felsökningssteg.

Genom att hantera dessa processer kan ni säkerställa att era kampanjer är säkra, slutbara och behåller varumärkets rykte.

## Delegeringsmetoder** Fullständigt jämfört med CNAME

* **Fullständig delegering** Adobe hanterar alla DNS-poster för underdomänen, vilket ger optimal leverans och säkerhet. Rekommenderas för de flesta användare.
* **CNAME-delegering** Kunden och Adobe delar DNS-ansvarsområden. Kunden skapar CNAME-poster som pekar på resurser som hanteras av Adobe.
* **Viktiga skillnader:
* **Fullständigt** Adobe har fullständig behörighet, mindre kundunderhåll.
* **CNAME** Delat ansvar; fler manuella steg för kunden.
* **Tips** Du kan aldrig delegera din rotdomän - endast underdomäner - för att undvika att förlora kontrollen över din huvuddomän.
