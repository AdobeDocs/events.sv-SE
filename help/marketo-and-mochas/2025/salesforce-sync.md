---
title: Marketo & Mochas - Salesforce Sync
description: Hantera synkroniseringen mellan Marketo och Salesforce med experttips om behörigheter, synlighet på fältet, administratörssamarbete och metodtips för att säkerställa smidig, optimerad integrering.
feature: Salesforce Integration
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3547
last-substantial-update: 2025-08-07T00:00:00Z
jira: KT-18706
source-git-commit: bc5752512fb1bc50cefe0180c308574e821888a2
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# Marketo &amp; Mochas: Salesforce Sync

Marketo har mycket få inbyggda integreringar, men Salesforce är det kraftfullaste av dem alla. Cirka 90 % av Marketo-kunderna använder Salesforce, och Adobe ger sina kunder råd om hur de ska teoriisera, diagnostisera och optimera synkroniseringen mellan dem. Marketo-synkroniseringen med SFDC baseras till stor del på de behörigheter i SFDC som ges till Marketo Sync User. Detta kan vara svårt för kunderna på grund av att flera administratörer eller olika team skapar vattentäta skott i kommunikationen kring uppdateringar i systemet.

Det här webbinariet går igenom följande när det gäller Marketo &lt;-> SFDC-synkronisering:

・ Förklara hur synkroniseringen fungerar
・ Dölja fält och objekt från Marketo Sync User i SFDC
・ Kommunicera med SFDC-administratören
・ Effektivt samarbete med Marketo Support
・ Saker att undvika när du synkroniserar Marketo med SFDC

>[!VIDEO](https://video.tv.adobe.com/v/3470624/?learn=on&enablevpops)

## Bästa tillvägagångssätt för att använda Salesforce Sync

Om du vill använda Salesforce Sync effektivt med Marketo följer du de bästa sätten, som förklaras steg för steg i enkla termer:

1. **Förstå synkroniseringsprocessen**

   Synkroniseringen kopplar samman Marketo och Salesforce, så att data kan flöda mellan de två systemen. Se&quot;Marketo Sync User&quot; som en bro mellan de två plattformarna. Den här användaren har behörighet att läsa och skriva vissa data:

   * **Skriv åtkomst** Leads och kontakter (Marketo kan uppdatera dem i Salesforce).
   * **Läs åtkomst** Konton, affärsmöjligheter, anpassade objekt och aktiviteter (Marketo kan visa dessa men inte ändra dem).

   När data ändras i Salesforce eller Marketo uppdateras det andra systemet var femte minut. Du kan dock prioritera brådskande uppdateringar med hjälp av flödessteg som&quot;Synkronisera med SFDC&quot;.

1. **Rensa fält**

   Synkronisera endast fält som används aktivt. Exempel:

   * Om du har gamla fält som&quot;COVID-19-anteckningar&quot; som inte längre är relevanta tar du bort dem från synkroniseringen. Det minskar störande detaljer och snabbar upp processen.
   * Undvik synkronisering av formelfält (t.ex.&quot;lead age in days&quot;) eftersom de inte uppdaterar tidsstämplar, vilket kan orsaka problem.

1. **Förhindra eftersläpning**

   En eftersläpning inträffar när för mycket data väntar på synkronisering. Så här undviker du:

   * Begränsa onödiga uppdateringar: Om ett kontopoäng till exempel ändras något (från 60 till 61) kan det utlösa uppdateringar för alla relaterade kontakter. Gruppera bakgrundsmusik i intervall (t.ex. 0-25, 26-50) för att minska uppdateringarna.
   * Gruppkampanjer: Använd gruppkampanjer i stället för att utlösa kampanjer för att bearbeta data effektivare.

1. **Hantera fel**

   Fel kan uppstå när Marketo försöker uppdatera ett fält i Salesforce men inte har behörighet. Felsök:

   * Logga in på Salesforce som Marketo Sync-användare och försök utföra samma åtgärd. Detta hjälper till att identifiera behörighetsproblem eller ogiltiga data.
   * Ställ in återkommande kampanjer i Marketo för att åtgärda vanliga fel, som att standardisera värden för land/stat (t.ex.&quot;CA&quot; till&quot;Kalifornien&quot;).

1. **Använd anpassade synkroniseringsfilter**

   Med anpassade filter kan du styra vilka poster som ska synkroniseras mellan Salesforce och Marketo. Skapa till exempel ett fält med namnet&quot;Synkronisera inte med Marketo&quot;. Om det här fältet är markerat som&quot;true&quot; för en post synkroniseras det inte till Marketo. Detta är användbart när du vill utesluta ogiltiga e-postadresser eller inaktuella kontakter.

1. **Begränsa skapande av aktivitet**

   Elm Salesforce. Fokusera på meningsfulla aktiviteter som&quot;ifyllt formulär&quot; eller&quot;klickad länk i e-postmeddelanden&quot;.

1. **Samarbeta med din Salesforce-administratör**

   Eftersom synkroniseringen omfattar båda systemen samarbetar du nära med din Salesforce-administratör för att:

   * Hantera behörigheter för Marketo Sync User.
   * Rensa bort onödiga fält i Salesforce.
   * Felsöka synkroniseringsproblem tillsammans.

1. **Övervaka synkroniseringsprestanda**

   Kontrollera synkroniseringsstatusen regelbundet i Marketo administratörssektion:

   Håll utkik efter toppar på kontrollpanelerna Synkronisera eftersläpning eller Synkronisera genomströmning. Dessa indikerar fördröjningar eller för stora uppdateringar.
Om du upptäcker problem bör du undersöka vilka fält eller poster som orsakar problemet.

1. **Använd anpassade objekt helt enkelt**

   Anpassade objekt är särskilda datastrukturer som kan lagra ytterligare information (t.ex. produktinformation). Synkronisera endast anpassade objekt som är nödvändiga för era kampanjer för att undvika att databasen blottas.

1. **Planera för skalbarhet**

   När du konfigurerar synkroniseringen ska du tänka på följande:

   * Underhåll en dataordlista för att spåra vilka fält som har synkroniserats och varför.
   * Undvik att synkronisera onödiga fält och poster för att systemet ska fungera effektivt.

Genom att följa dessa steg kan du säkerställa en smidig och effektiv integrering mellan Marketo och Salesforce, minimera antalet fel och maximera datavärdet.
