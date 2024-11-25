---
title: Körbara kampanjer - Lär dig hur körbara filer kan öka effektiviteten och påverka
description: Besök Chris Willis, Courtny Edwards-Jones och Jane Musatova i denna Adobe Champion Deep Dive för att lära dig hur körbara kampanjer i Marketo kan effektivisera processer, säkerställa datakvalitet och automatisera komplexa arbetsflöden, med praktiska exempel och fokus på att minimera fel och eftersläpningar.
role: Developer, User
level: Intermediate, Experienced
doc-type: Event
duration: 3778
last-substantial-update: 2024-03-07T00:00:00Z
jira: KT-15098
thumbnail: 3427704.jpeg
exl-id: cfea1a1a-2d29-4cf6-b633-aa2a2523114e
source-git-commit: 8da73b657295864a3bf6c64598b2fbd664a2379d
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Körbara kampanjer - Lär dig hur körbara filer kan öka effektiviteten och påverka

>[!VIDEO](https://video.tv.adobe.com/v/3427704/?learn=on)

**Modererat av** Chris Willis
**Talare** Courtny Edwards-Jones och Jane Musatova

## Översikt

I den här utgåvan av Adobe Champion Deep Dive diskuterar vi användningen av körbara kampanjer i Marketo och ger exempel på hur de kan användas för att effektivisera processerna och säkerställa datakvaliteten. Körbara kampanjer är en typ av smarta kampanjer som kör flöden synkront, vilket möjliggör beroenden mellan olika steg. De kan användas för att automatiskt försöka utföra misslyckade processer igen, t.ex. datastandardisering eller lead-kvalificering, innan de går vidare till nästa steg. Dokumentet innehåller även information om användningen av överordnade kampanjer och kapslade körbara filer, liksom begränsningar för körbara kampanjer, som oförmåga att använda webhooks eller väntesteg.

## Vad är syftet med körbara kampanjer?

Syftet med körbara kampanjer är att effektivisera och automatisera komplexa arbetsflöden i Marketo. Med körbara kampanjer kan ni definiera en sekvens av åtgärder som måste slutföras innan ni går vidare till nästa steg i en kampanj. På så sätt säkerställs att varje åtgärd utförs fullständigt innan du fortsätter, vilket minskar risken för fel eller ofullständiga processer. Körbara kampanjer kan användas för att testa misslyckade processer på nytt, standardisera och berika data, kvalificera leads, samla in intressanta ögonblick och mycket mer. De ger ett effektivare och mer organiserat sätt att hantera och automatisera era marknadsföringsaktiviteter.

## Vad är en körbar kampanj och hur fungerar den?

En körbar kampanj är en typ av smart kampanj i Marketo som gör att flera flöden kan köras sekventiellt i en och samma kampanj. Den är utformad för att säkerställa att varje flöde körs helt innan nästa börjar. Detta skiljer sig från en begärandekampanj, som körs asynkront och kan ha flera flöden parallellt.

Om du vill skapa en körbar kampanj måste du markera kryssrutan Körbar när du skapar kampanjen. När du har skapat en kampanj kan du lägga till flödessteg, till exempel ändra datavärden, skicka e-post eller uppdatera programstatus. Det finns dock vissa begränsningar för körbara kampanjer. Du kan inte använda utlösare, webhooks eller väntesteg i en körbar kampanj.

Körbara kampanjer är användbara för processer som är beroende av varandra, där ett flöde måste slutföras innan nästa kan börja. De kan effektivisera de operativa processerna, förenkla databehandlingen och minimera risken för fel och eftersläpningar. Genom att använda körbara kampanjer kan ni se till att alla steg i en process är slutförda innan ni går vidare till nästa, vilket förbättrar effektiviteten och exaktheten i era marknadsföringsåtgärder.