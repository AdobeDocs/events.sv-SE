---
title: Marketo Migration to the Adobe Admin Console - (Pre-Migration)
description: Adobe migrerar Marketo Engage till Admin Console för bättre användarhantering. Lär dig mer om automatisk och självmigrering, krav, ändringar efter migrering, bästa praxis, vanliga fallgropar och support. Gå till sessionsinspelningen på Adobe Experience League webbplats.
solution: Marketo Engage
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2280
last-substantial-update: 2025-03-14T00:00:00Z
jira: KT-17483
exl-id: 9c3da83f-9e02-4a2e-9784-10213facf056
source-git-commit: 088615f28aa91dfd4ba119c11c4c9f8a89441d84
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Marketo Migration to the Adobe Admin Console - Pre Migration

Gå med i Marketo och få en smidig migrering med Adobe Experts!

Ligg steget före migreringen av Marketo med Adobe Customer Experience &amp; Identity Team i det här informativa webbinariet. Vi följer dig igenom viktiga steg, bästa praxis och vanliga utmaningar för att säkerställa en smidig övergång till Adobe Admin Console.

What You&#39;ll Learn,

* En stegvis färdplan för er process före migrering
* Bästa tillvägagångssätt för att förenkla övergången och undvika fallgropar
* Expertsvar på vanliga migrationsfrågor

Vare sig du just har påbörjat migreringen eller förbereder dig för de sista stegen kommer den här sessionen att ge dig den kunskap och de verktyg du behöver för att navigera i processen på ett säkert sätt. Missa inte detta tillfälle att få försprång och effektivisera migreringen av Marketo!

>[!VIDEO](https://video.tv.adobe.com/v/3449712/?learn=on&enablevpops)

## Viktiga uppgifter

### Syfte med migrering och översikt

Adobe migrerar Marketo Engage till Admin Console för att konsolidera alla produkter till ett nav för bättre användarhantering och åtkomst.  Admin Console är navet för hantering av Adobe produkter, användarroller, behörigheter och åtkomst. URL:er för åtkomst till Marketo Engage ändras till Adobe Experience Cloud-plattform.

### Migreringstyper

* **Automatisk migrering** För organisationer med färre än 75 användare och utan SSL-installation. Adobe hanterar migreringen.
* **Självmigrering** För organisationer med SSL-konfiguration. Administratörer hanterar migreringsprocessen med hjälp av migreringskonsolen.

### Krav för migrering

* Systemadministratörer måste fylla i e-postmeddelandet om godkännande.
* SSL måste konfigureras i Admin Console (inte i Marketo-instansen).

### Ändringar efter migrering

* Användare loggar in med Adobe ID eller Federated ID (SSL).
* Administratörsroller och -behörigheter avgör åtkomstnivåerna i Admin Console.

### Bästa praxis

* Verifiera användarens e-post och åtgärda utlåsta konton före migreringen.
* Se till att rätt administratörsroller har tilldelats.
* Inaktivera annonsblockerare eller använd inkognito-läge för att undvika inloggningsproblem.

### Vanliga fallgropar

* Felaktiga administratörsbehörigheter kan begränsa åtkomsten.
* Webbläsartillägg och annonsblockerare kan störa åtkomsten.
* IP-vitlistning stöds ännu inte i Admin Console, men håller på att utvecklas.

### Påverkan på funktioner

* Automatiserade e-postmeddelanden, API-användare och munchkin-koder påverkas inte av migreringen.
* Migreringen påverkar i första hand användarautentisering och -hantering.

### Support

* Användare som har problem bör öppna ett supportärende hos Adobe kundtjänst.
* Inkludera IMS-org-ID i supportärenden för snabbare lösning.
