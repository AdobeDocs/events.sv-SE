---
title: Be experterna - användbara tillägg i Taggar (Launch) för att få hjälp att ladda upp Web SDK
description: Funderar du på att migrera implementeringen till nya Adobe Web SDK?  Vi kommer att gå igenom några av våra favorittillägg i Adobe Tags Library som hjälper dig att ta datainsamlingen till nästa nivå.
solution: Data Collection, Experience Platform
feature: Tags
kt: 10528
event-start-time: 2022-08-23 09:00-7
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
duration: 3833
source-git-commit: 0b2f63198af8767f24783dbafd244c9398c24f33
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# Fråga experterna: Användbara tillägg i Taggar (Launch) för att ge superladdning åt Web SDK

Funderar du på att migrera implementeringen till nya Adobe Web SDK?  Vi kommer att gå igenom några av våra favorittillägg i Adobe Tags Library som hjälper dig att ta datainsamlingen till nästa nivå.

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## Frågor och kommentarer från programmet

### Utökning av dataelementassistenten från Erangtics

<br> 
**Fråga:** Är Erangtics säkert att använda ur datasäkerhetsperspektiv, eftersom detta är ett tillägg från tredje part?

**Svar:** Ja. Du kan granska tilläggskoden om du vill, men den sparar inte datumet, utan bara en omformning.

<br> 

**Fråga:** Fångar även detta Adobe ECID?

**Svar:** Adobe ECID hämtas inte i det tillägget. Det här tillägget är avsett för att skapa ytterligare, anonyma identifierare (bland annat).

**Svar:** Adobe ECID kan dock hämtas på andra sätt. Vi kommer att dela ut det via ExL-anteckningarna och Twitterna eftersom vi inte kan dela länkar i chatten här.

<br> 

**Fråga:** Hash-funktionen erbjuder den olika hashtekniker som SHA-256 och tillhandahåller offentliga och privata nycklar?

**Svar:** Ja! SHA-256 är standard

<br> 

### Allmänna frågor och kommentarer:

<br> 

**Fråga:** Vad klickar vi på för att hämta källfilerna för tilläggen? Är det i &quot;3-punktsmenyn&quot;?

**Svar:** Ja! De tre punkterna och sedan Ladda ned Source (från katalogvyn)

<br> 

**Kommentar:** En av de saker jag gillar med tillägg är den tidsbesparande aspekten av dem. Många av dem gör saker som du *skulle kunna* göra med anpassad kod, men med ett tillägg behöver du inte skriva den koden.

**Svara:** Direkt. Och den är upprepningsbar utan att behöva återskapa hjulet varje gång.

<br> 

**Fråga:** Hur stöds eller ersätts plugin-program för analys med Web SDK-implementeringar?

**Svar:** Många analysplugin-program är i själva verket inte nödvändiga nuförtiden tack vare den extra flexibiliteten i taggar för Workspace och Adobe. De som inte gör det migreras aktivt för användning av Web SDK.

<br> 

**Fråga:** Finns det någon utveckling av aktivitetsschemaspårning med Web SDK?

**Svar:** Jag är glad att kunna meddela att Activity Map aktivt arbetar för stöd i Web SDK också

<br> 

**Fråga:** Skulle vi kunna ha åtkomst till Adobe Edge-nätverk för att hantera händelser innan vi överför dem till slutdestinationerna? Jag förstår att vi också kan göra det i Launch, men skulle det i framtiden också vara möjligt att göra det på servern?

**Svar:** Ja! Detta är möjligt via vår Event Forwarding-funktion, som kunderna kan köpa via någon av våra Real-Time CDP-produkter (Real-Time CDP Connections, Prime eller Ultimate).

**Svar:** RTCDP-anslutningar (Event Forwarding) ger dig möjlighet att ha större kontroll innan du skickar den till icke-adobe-mål.

**Svara:** Kolla in några av våra andra ExL Live-videor och läs mer om detta (som [den här](exl-live-episode-06-23-22.md)).

<br> 

**Kommentar:** Snabbanrop för ett av mina favorittillägg: Det finns ett mappningstabelltillägg där du kan läsa en tabell för ett dataelement som &quot;Om det här värdet är det ska du ange det som det&quot;.

**Svar:** Den flexibilitet de ger är ganska imponerande. Observera också att företag kan skapa egna privata tillägg också om de vill.

<br> 

**Fråga:** Du visade enskilda data från CRM som ort och väder, så var lagrar vi det individuella svaret?

**Svar:** Svar lagras i varje unik händelse som utlöser en regel inom en händelsevidarebefordringsegenskap och används endast i den specifika händelsen.

<br> 

Fortsätt diskutera det här ämnet i [Experience League Community-diskussionen](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## Ytterligare Experience League LIVE-sessioner från den här datainsamlingsserien

* [Fråga experterna - Grunderna i Web SDK](exl-live-episode-05-26-22.md)
* [Fråga experterna - RTCDP-anslutningar](exl-live-episode-06-23-22.md)
* [Fråga experterna - Datastreams och Data Prep](exl-live-episode-07-21-22.md)

