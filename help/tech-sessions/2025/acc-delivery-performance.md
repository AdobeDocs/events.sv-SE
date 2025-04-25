---
title: Adobe Campaign Classic Delivery Performance - felsökning
description: Den här sessionen behandlade viktiga strategier för att förbättra e-post- och SMS-leveransen med Adobe Campaign. Här har vi tagit itu med vanliga utmaningar som leveransförseningar, låg genomströmning och transaktionell långsamhet, och erbjuder lösningar som batchoptimering, SQL-loggning och övervakning av serverprestanda. De effektivaste sätten att leverera inkluderar korrekt e-postautentisering (SPF, DKIM, DMARC), svartlistsövervakning och skräppostkontroller. För bättre prestanda rekommenderade experterna rena arbetsflöden, strypningsregler och att delade behållare undviks. SMS-leveranstips fokuserar på korrekt konfiguration av externa konton och logganalys. Sessionen betonade även spårningsvalidering, databasunderhåll med bloatrapporter och tillämpning av tryck-/trötthetsregler för att öka engagemanget. En sessionsinspelning delas via e-post och läggs upp på webbplatsen Adobe Experience.
version: Classic v7
solution: Campaign Classic v7
product: Adobe Campaign
feature: SMS, Deliverability, Troubleshooting
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2257
last-substantial-update: 2025-04-25T00:00:00Z
jira: KT-17869
source-git-commit: 373605f79b3122382e221252232a26535ff3109b
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---


# Tekniska sessioner: Adobe Campaign Classic Delivery Performance - felsökning

Under den här sessionen kommer vi att utforska vanliga utmaningar när vi levererar optimala prestanda med Adobe Campaign Classic (ACC) och tillhandahålla användbara strategier för felsökning och problemlösning. Deltagarna får lära sig att identifiera flaskhalsar i prestandan, åtgärda inkonsekvenser i leveransförberedelser/konfiguration och implementera bästa praxis för att säkerställa smidig kommunikation. Det här webbinariet ger deltagarna den kunskap och de verktyg de behöver för att effektivisera sina ACC-kampanjer, få bättre resultat och leverera högkvalitativa kundupplevelser - från att optimera leveranser till att övervinna tekniska svårigheter.

>[!VIDEO](https://video.tv.adobe.com/v/3457826/?learn=on&enablevpops)

## Viktiga uppgifter

**Leveransproblem och -lösningar**

* Vanliga problem är leveransförseningar, fel vid förberedelser, fastlagda leveranser, låga leveransgrader, låg genomströmning, lågt engagemang och långsam leverans av transaktioner.
* Lösningarna inkluderar optimering av leveransbatchbearbetning, övervakning av serverprestanda, aktivering av SQL-frågeloggning, granskning av granskningsloggar och korrekt konfigurering av MTA- och IP-tillhörigheter.

**Bästa praxis för slutleverans**

* Säkerställ korrekt e-postautentisering (SPF, DKIM, DMARC).
* Övervaka svartlistningsstatus och undvik skräppostutlösande innehåll.
* Använd skräppostkontroller för att utvärdera skräppostpoäng innan du skickar e-post.

**Optimerar leveransresultat**

* Använd rena arbetsflöden för målinriktning och begränsa antalet personaliseringsfält.
* Implementera begränsningsregler, gruppbearbetning och topologiregler för undantag och filtrering.
* Undvik att dela behållare över flera kanaler för att förhindra flaskhalsar.

**Felsökning av SMS-leveransproblem**

* Kontrollera att externa konton är unikt konfigurerade och att SMS-processer körs.
* Kontrollera om det finns fel i SMS-loggar och verifiera reguljära uttryck i SMP-inställningar.
* Kontakta tjänsteleverantören för felkonfigurationsproblem.

**Långsam transaktionsleverans**

* Övervaka interna och totala bearbetningstider.
* Kontrollera att leveransstorleken är inom gränsen (60 GB för batch, 30 GB för händelse).
* Granska typologiregler och personaliseringsinställningar.

**Spårning och engagemang**

* Validera arbetsflöden för spårning och serverloggar.
* Testa anpassade spårningsformler i lägre miljöer före produktionen.
* Kontrollera att spårningsservrar är igång.

**Databasunderhåll**

* Använd bloatrapporter för att identifiera tabeller med hög uppblåsning och motivera ett databasvakuum.

**Allmänna rekommendationer**

* Använd tryck- och trötthetsregler för att begränsa onödiga e-postmeddelanden.
* Segmentera stora leveranser i mindre grupper för att optimera prestandan.