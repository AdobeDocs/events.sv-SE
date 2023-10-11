---
title: Fråga experten - Kvalitet på och engagemang i mätningarna
description: Lär dig skapa rapporter som besvarar frågor om kvalitet och engagemang. Det här webbinariet spelades in den 13 november 2019.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9914
exl-id: 76a8e418-71c7-414a-9938-e64e4e73c184
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '1211'
ht-degree: 1%

---

# Fråga experten - Kvalitet på och engagemang i mätningarna

Lär dig skapa rapporter som besvarar frågor om kvalitet och engagemang. Det här webbinariet spelades in den 13 november 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## Frågor och svar

**Fråga**

Det finns vissa fält som kan filtreras efter, men som inte är tillgängliga när du försöker gruppera efter dem. Arbetar du med att göra dem enhetliga?

**Svar**

Rapporteringsverktygen tillåter inte att du grupperar efter ett dynamiskt fält eller ett som kan ha flera val markerade samtidigt, som ett kryssrutefält. Du kan bara gruppera fält som har ett enda värde, även om de kan ha många alternativ.

Du kan filtrera efter kryssrutor och visa dem. Du kan bara inte gruppera dem.

**Fråga**

Får jag visa den primära fetstilen i iteration på jobbroller?

**Svar**

Under arbetets gång kan vi identifiera den primära rollen. Detta måste göras i ett värdeuttryck, men HTML-koder känns inte igen i ett värdeuttryck. Därför måste vi komma fram till ett annat sätt att identifiera rollen som den primära. Jag skrev &quot;**&quot; före och efter det primära rollnamnet i den här koden. Prova själv:

```
displayname=All Job Roles 
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("**",{role}.{name},"**"),{role}. {name})
valueformat=HTML
```

Då får du en sådan lista:

```
Support Engineer 
QA Engineer 
**Designer**
```

Där Designer är den primära rollen för den här användaren.

**Fråga**

Hej! Jag sätter ihop ett arbetsflöde för vårt redaktionsteam som håller reda på var en artikel befinner sig i sin livscykel (inledande skrivning —> granskningar —> färdiga redigeringar —> publicering). De vill enkelt se vilken milstolpe eller uppgift de har just nu. Den feedback jag får är standardvyn Milstolpe (med röd eller grön skuggning) som är för &quot;upptagen och komplex&quot;. Finns det något sätt att bara visa&quot;Projektnamn&quot; och&quot;Aktuell milstolpe&quot; i en tabell eller ett rutnät?

**Svar**

Ja. Du kan skapa en uppgiftsrapport som visar de milstolpeuppgifter som för närvarande bearbetas och vilken uppgift den är kopplad till. Det kan du göra i en tabell eller i en listrapport.

**Fråga**

Kan vi ha korrekturinformation i kombination med projektinformation i en rapport?

**Svar**

Om du har skapat en korrekturgodkännanderapport kan projektinformation hämtas till kolumner i textläge. Om du till exempel vill referera till projektnamnet i en kolumn kan du använda följande:

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**Fråga**

Jag vill också ha mer information om rapportering av korrekturdata när det gäller projektet. Exempel: en projektrapport som innehåller beslutsbevis och kommentarer.

**Svar**

Om du vill referera till projektinformation och korrekturinformation i en enda rapport måste du skapa en rapport för korrektur av godkännande. För närvarande går det inte att hämta kommentarer från ett bevis i den här rapporten, men varje beslut om godkännande finns på sin egen radartikel i kolumnen för godkännarbeslut.

**Fråga**

Jag använder ofta Sharecol för att skapa status för en sida (många kolumner). Men jag tycker att om jag vill lägga till en kolumn högst upp på sidan efter att jag skapat en rapport är det väldigt tidsödande att gå tillbaka och ändra. Har du några tips eller trick för att göra den här typen av förändring?

**Svar**

Om du talar om att placera en kolumn högst upp i en kolumnlista i textläge behöver du bara numrera om kolumnerna manuellt.

Men om du redan har skapat rapporten med den första kolumnen som några delade kolumner och vill placera en annan delad kolumn högst upp i listan, är det här enklare.

Lägg bara till några nya kolumner i rapportredigeraren och dra dem längst till vänster på skärmen Kolumner (Visa). När du har gjort det här tar du en titt på vad som tidigare var den vänstra kolumnen och ser att kolumnnumren i textläget har ökat. Dra så många tomma kolumner du behöver. Se till att du placerar något i de tomma kolumnerna innan du sparar dem, annars tas de bort.

**Fråga**

Hej - vad gäller den sista felrapporten - hur kan rapporterna göras för flera projekt - om det kommer buggar för flera projekt?

**Svar**

Du kan filtrera efter portfölj eller projekt, beroende på hur du har organiserat ditt arbete.

Du kan också filtrera på begärandeköer. Du kanske vill skapa begärandeköer för varje projekt där du kan skapa kundanvändare som granskare som kan logga in och skicka biljetter direkt till de begärandeköer som du har delat med dem.

**Fråga**

De första rapporterna baserades på projekt-/projektnamn. Detta kan även utföras på uppgifter och i så fall vad som är det bästa sättet att gruppera dem, eftersom det är möjligt att aktivitetsnamnet är ett annat namn än inte ... tack!

**Svar**

Alla dessa rapporter kan göras antingen som uppgifts-, utfalls- eller projektrapporter, beroende på hur du bestämmer dig för att spåra saker.

Ett vanligt sätt att gruppera uppgifter är att först gruppera dem efter deras projektnamn och sedan efter aktivitetsnamnet i varje projekt. Om du har två uppgifter med samma namn är det då enkelt att se vilket projekt de har i.

**Fråga**

Jag vill veta vilka korrektur som är utestående, vilken uppgift och vilket projekt de är kopplade till, när de slussas vidare, när det är rätt och vem som är moderator och godkännare.

**Svar**

Utestående korrektur kan filtreras genom Väntande beslut > Lika med > Sant i en korrekturgodkännanderapport. Det finns en kolumn för Godkännare, som talar om för dig vem som ännu inte har fattat något beslut.

Du kan referera till uppgiften eller projektet som korrekturet är kopplat till med hjälp av textläge (se exempel nedan).

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name
valueformat=HTML
```

När det gäller routningsdatumet, förfallodatumet och moderatorn kan dessa fält för närvarande inte hämtas till någon av Workfront-rapporterna, så du måste klicka i korrekturfilen direkt för att kunna visa den informationen.

**Fråga**

Kan du skapa ett anpassat formulär som automatiskt skickas till en begärande när deras begäran är slutförd? Som en kundnöjdhetsundersökning?

**Svar**

Här är en sak du kan göra som kan uppfylla dina behov. Du kan bifoga ett påminnelsemeddelande till en utgåva som skickar ett e-postmeddelande till&quot;Angivet av&quot; efter att ett faktiskt slutförandedatum har angetts. Anges av är den person som skapade problemet.

Du skapar påminnelsemeddelandet på samma sätt som i webbinariet för&quot;Påminnelse för att fylla i AAR (After Action Review)&quot;, förutom att det är en påminnelse om att du har problem. Du vill förmodligen skapa en e-postmall för den och även länka till enkäten. Du måste använda påminnelsemeddelandet manuellt för varje problem (eller använda massredigering).

En integrering skulle vara bättre eftersom den kan automatisera de manuella stegen, men påminnelsemeddelandet kan göras direkt.

**Fråga**

Jag skapade en rapport som visar projekt efter malltyp. Jag kan lista projektägaren men inte de personer som har tilldelats ett projekt.

**Svar**

Om du vill hämta en kolumn i projektrapporten från fliken Projektteam (bemanning) måste du skapa den i textläge. Textläget är följande:

```
displayname=Staffing 
listdelimiter=<p> 
listmethod=nested(projectUsers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

## Text Mode-kod för AAR-engagemangsrapporten

```
column.0.displayname=Task Details
column.0.value=<b>Project Name:</b>&nbsp;
column.0.valueformat=HTML
column.0.sharecol=true
column.1.valuefield=project:name
column.1.valueformat=HTML
column.1.sharecol=true
column.2.value=<br>
column.2.valueformat=HTML
column.2.sharecol=true
column.3.value=<b>Task Name:</b>&nbsp;
column.3.valueformat=HTML
column.3.sharecol=true
column.4.valuefield=name
column.4.valueformat=HTML
column.4.sharecol=true
column.5.value=<br>
column.5.valueformat=HTML
column.5.sharecol=true
column.6.value=<b>Task Owner:</b>&nbsp;
column.6.valueformat=HTML
column.6.sharecol=true
column.7.valuefield=assignedTo:name
column.7.valueformat=HTML
column.7.sharecol=true
column.8.value=<br>
column.8.valueformat=HTML
column.8.sharecol=true
column.9.value=<b>Actual Completion Date:</b>&nbsp;
column.9.valueformat=HTML
column.9.sharecol=true
column.10.valuefield=actualCompletionDate
column.10.valueformat=HTML
column.11.displayname=Name of Reviewer
column.11.linkedname=Name of Reviewer
column.11.namekey=view.relatedcolumn
column.11.namekeyargkey.0=Name of Reviewer
column.11.namekeyargkey.1=name
column.11.querysort=DE:Name of Reviewer:name
column.11.valuefield=Name of Reviewer:name
column.11.valueformat=customReferenceObjectAsString
column.12.displayname=AAR 1
column.12.description=In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.12.value=<b>AAR 1 Score:</b>&nbsp;
column.12.valueformat=HTML
column.12.sharecol=true
column.13.valuefield=AAR 1 - In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.13.valueformat=customDataLabelsAsString
column.13.sharecol=true
column.14.value=<br>
column.14.valueformat=HTML
column.14.sharecol=true
column.15.value=<br><b>AAR 1 User Comment:</b>&nbsp;
column.15.valueformat=HTML
column.15.sharecol=true
column.16.valuefield=AAR 1 User Comment
column.16.valueformat=customDataLabelsAsString
column.17.linkedname=direct
column.17.namekey=AAR 1 Reviewer Comment
column.17.querysort=DE:AAR 1 Reviewer Comment
column.17.valuefield=AAR 1 Reviewer Comment
column.17.valueformat=customDataLabelsAsString
column.18.linkedname=direct
column.18.displayname=AAR 1 Needs Attn
column.18.querysort=DE:AAR 1 Needs Attention
column.18.valuefield=AAR 1 Needs Attention
column.18.valueformat=customDataLabelsAsString
column.19.linkedname=direct
column.19.displayname=AAR 1 Needs Attn Notes
column.19.querysort=DE:AAR 1 Needs Attention Notes
column.19.valuefield=AAR 1 Needs Attention Notes
column.19.valueformat=customDataLabelsAsString
column.20.displayname=AAR 2
column.20.description=Do You Believe This Work Will Make an Impact?
column.20.value=<b>AAR 2 Score:</b>&nbsp;
column.20.valueformat=HTML
column.20.sharecol=true
column.21.valuefield=AAR 2 - Do You Believe This Work Will Make an Impact?
column.21.valueformat=customDataLabelsAsString
column.21.sharecol=true
column.22.value=<br>
column.22.valueformat=HTML
column.22.sharecol=true
column.23.value=<br><b>AAR 2 User Comment:</b>&nbsp;
column.23.valueformat=HTML
column.23.sharecol=true
column.24.valuefield=AAR 2 User Comment
column.24.valueformat=customDataLabelsAsString
column.25.linkedname=direct
column.25.namekey=AAR 2 Reviewer Comment
column.25.querysort=DE:AAR 2 Reviewer Comment
column.25.valuefield=AAR 2 Reviewer Comment
column.25.valueformat=customDataLabelsAsString
column.26.linkedname=direct
column.26.displayname=AAR 2 Needs Attn
column.26.querysort=DE:AAR 2 Needs Attention
column.26.valuefield=AAR 2 Needs Attention
column.26.valueformat=customDataLabelsAsString
column.27.linkedname=direct
column.27.displayname=AAR 2 Needs Attn Notes
column.27.querysort=DE:AAR 2 Needs Attention Notes
column.27.valuefield=AAR 2 Needs Attention Notes
column.27.valueformat=customDataLabelsAsString
column.28.displayname=AAR 3
column.28.description=Are you proud of the work you did on this?
column.28.value=<b>AAR 3 Score:</b>&nbsp;
column.28.valueformat=HTML
column.28.sharecol=true
column.29.valuefield=AAR 3 - Are you proud of the work you did on this?
column.29.valueformat=customDataLabelsAsString
column.29.sharecol=true
column.30.value=<br>
column.30.valueformat=HTML
column.30.sharecol=true
column.31.value=<br><b>AAR 3 User Comment:</b>&nbsp;
column.31.valueformat=HTML
column.31.sharecol=true
column.32.valuefield=AAR 3 User Comment
column.32.valueformat=customDataLabelsAsString
column.33.linkedname=direct
column.33.namekey=AAR 3 Reviewer Comment
column.33.querysort=DE:AAR 3 Reviewer Comment
column.33.valuefield=AAR 3 Reviewer Comment
column.33.valueformat=customDataLabelsAsString
column.34.linkedname=direct
column.34.displayname=AAR 3 Needs Attn
column.34.querysort=DE:AAR 3 Needs Attention
column.34.valuefield=AAR 3 Needs Attention
column.34.valueformat=customDataLabelsAsString
column.35.linkedname=direct
column.35.displayname=AAR 3 Needs Attn Notes
column.35.querysort=DE:AAR 3 Needs Attention Notes
column.35.valuefield=AAR 3 Needs Attention Notes
column.35.valueformat=customDataLabelsAsString
column.36.displayname=Done
column.36.valuefield=Review Complete
column.36.valueformat=customDataLabelsAsString
```
