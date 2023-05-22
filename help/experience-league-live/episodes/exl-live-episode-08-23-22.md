---
title: Be experterna - användbara tillägg i Taggar (Launch) för att få hjälp att ladda upp Web SDK
description: Funderar du på att migrera implementeringen till nya Adobe Web SDK?  Vi kommer att gå igenom några av våra favorittillägg i Adobe Tags Library som hjälper dig att ta datainsamlingen till nästa nivå.
solution: Data Collection,Experience Platform
kt: 10528
thumbnail: 346610.jpeg
event-start-time: 2022-08-23 09:00-7
event-cta-url: null
event-guests: Rudi Shumpert,Jeff Chasin,Eric Matisoff
exl-id: 5ef987f4-37f5-473f-b9f2-1598b7e655ba
source-git-commit: 17070f55bae19ef0751a2c7c536af7758e31affc
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Fråga experterna: Användbara tillägg i taggar (Launch) för att ge superladdning åt Web SDK

Funderar du på att migrera implementeringen till nya Adobe Web SDK?  Vi kommer att gå igenom några av våra favorittillägg i Adobe Tags Library som hjälper dig att ta datainsamlingen till nästa nivå.

>[!VIDEO](https://video.tv.adobe.com/v/346610/?quality=12&learn=on)

## Frågor och kommentarer från programmet

### Utökning av dataelementassistenten från Erangtics

<br> 
**Fråga:** Ur datasäkerhetsperspektiv, är Erangtics säkert att använda, eftersom detta är ett tillägg från tredje part?

**Svar:** Ja. Du kan granska tilläggskoden om du vill, men den sparar inte datumet, utan bara en omformning.

<br> 

**Fråga:** Fångar detta även Adobe ECID?

**Svar:** Adobe ECID fångas inte in i det tillägget. Det här tillägget är avsett för att skapa ytterligare anonyma identifierare (bland annat).

**Svar:** ECID för Adobe kan dock fångas på andra sätt. Vi kommer att dela ut det via ExL-anteckningarna och Twitter eftersom vi inte kan dela länkar i chatten här.

<br> 

**Fråga:** Hash-funktionen erbjuder den olika hashtekniker som SHA-256 och erbjuder publika och privata nycklar?

**Svar:** Ja! SHA-256 är standard

<br> 

### Allmänna frågor och kommentarer:

<br> 

**Fråga:** Vad klickar vi på för att hämta källfilerna för tillägg? Är det i &quot;3-punktsmenyn&quot;?

**Svar:** Ja! De tre punkterna och sedan Hämta källa (från katalogvyn)

<br> 

**Kommentar:** En av de saker jag gillar med tillägg är den tidsbesparande aspekten av dem. Många av dem gör saker du *kunde* gör med viss anpassad kod, men med ett tillägg behöver du inte skriva den koden.

**Svar:** Just nu. Och den är upprepningsbar utan att behöva återskapa hjulet varje gång.

<br> 

**Fråga:** Hur stöds eller ersätts plugin-program för analys med Web SDK-implementeringar?

**Svar:** Många plugin-program för analys är i själva verket inte nödvändiga nuförtiden tack vare den extra flexibiliteten i Workspace och Adobe Tags. De som inte gör det migreras aktivt för användning av Web SDK.

<br> 

**Fråga:** Har du någon utveckling av aktivitetsschemats spårning med Web SDK?

**Svar:** Jag är glad att kunna meddela att Activity Map också arbetar aktivt för att få stöd i Web SDK

<br> 

**Fråga:** Skulle vi kunna få tillgång till Adobe Edge nätverk för att hantera händelser innan vi överför dem till slutdestinationerna? Jag förstår att vi också kan göra det i Launch, men skulle det i framtiden också vara möjligt att göra det på servern?

**Svar:** Ja! Detta är möjligt via vår Event Forwarding-funktion, som kunderna kan köpa via någon av våra Real-Time CDP-produkter (Real-Time CDP Connections, Prime eller Ultimate).

**Svar:** RTCDP-anslutningar (Event Forwarding) ger möjlighet att ha större kontroll innan du skickar den till icke-adobe-mål.

**Svar:** Ta en titt på några andra ExL Live-videor och läs mer om detta (som [den här](exl-live-episode-06-23-22.md)).

<br> 

**Kommentar:** Ring upp ett av mina favorittillägg: Det finns ett mappningstabelltillägg där du kan läsa en tabell för ett dataelement som &quot;om det här värdet är det ska du ange det som det&quot;.

**Svar:** Den flexibilitet de ger är mycket imponerande. Observera också att företag kan skapa egna privata tillägg också om de vill.

<br> 

**Fråga:** Du visade data från CRM som stad och väder, så var lagras svaret?

**Svar:** Svar lagras i varje unik händelse som utlöser en regel i en händelsevidarebefordringsegenskap och används endast i den specifika händelsen.

<br> 

Fortsätt diskutera det här ämnet i [Experience League Community-diskussion](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-platform/experience-league-live-post-session-discussion-useful-extensions/m-p/542620#M240).
<br> 

## Ytterligare Experience League LIVE-sessioner från den här datainsamlingsserien

* [Fråga experterna - Grunderna i Web SDK](exl-live-episode-05-26-22.md)
* [Fråga experterna - RTCDP-anslutningar](exl-live-episode-06-23-22.md)
* [Fråga experterna - Datastreams och Data Prep](exl-live-episode-07-21-22.md)
