---
title: Endre standarddomene for Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991203"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Endre standarddomene/primært domene for Yammer

Nettadressen til Yammer inneholder gjeldende primære domenenavn for Yammer-nettverket. Dette domenenavnet samsvarer kanskje ikke med det primære domenenavnet som er angitt i Office 365 eller Azure AD. Det finnes forskjeller i virkemåte basert på antallet egendefinerte domener som er lagt til i tenanten, og om Yammer er i en støttet konfigurasjon (1 Tenant: 1 nettverk eller 1:1). Dokumentasjon om [Yammer-domener og Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) er tilgjengelig.

Den vanligste årsaken til at du ser feil domene, er at det finnes flere Yammer-nettverk, og disse må konsolideres. [Å konsolidere ned til et enkelt nettverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ved hjelp av nettverksmigreringsverktøyet er et viktig sted å starte. Fullfør dette før du prøver å angi primært domene.

**Ingen egendefinerte domener**

Standarddomenet (f.eks. fabrikam.onmicrosoft.com) fra tenanten brukes for Yammer for nye tenanter. Det primære domenet er angitt til yammer.com/fabrikam.onmicrosoft.com.

**Enkelt egendefinert domene**

Yammer velger automatisk det egendefinerte domenet (f.eks. fabrikam.com) fra tenanten som primært domene i Yammer. Det er angitt til yammer.com/fabrikam.com. Denne endringen gjøres av synkroniseringstjenesten for domenet, og det kan ta opptil 24 timer før den trer i kraft.

**Flere egendefinerte domener**

Yammer kan ha et primært domene som er forskjellig fra standard tenantdomene. Siden det finnes flere egendefinerte domener, forsøker ikke Yammer å gjette korrekt domene fra de som er tilgjengelige. Du må åpne en sak hos kundestøtte for å be om at det primære domenenavnet endres til det primære domenet du ønsker.

**Mer informasjon om feilsøking**

I noen tilfeller kan det hende at domener er flyttet mellom tenanter og at synkroniseringstjenesten for domenet ikke har kjørt. Det kan hende du opplever problemer med pålogging eller andre ting, i tillegg til et primært domene som er feil. For å løse dette problemet må domener flyttes til riktig nettverk med hjelp fra Microsoft kundestøtte. Denne situasjonen krever direktehjelp og kan ta litt tid å løse, særlig hvis det finnes en svært lang liste over domenenavn. Åpne en sak hos kundestøtte for å få hjelp med å løse disse problemtypene.

Når du arbeider med kundestøtterepresentanter, kontrollerer de at domener er verifisert på en tenant som er under din kontroll. De kan stille tilleggsspørsmål knyttet til verifiseringen av domenene hvis de legges til på tenanten, men ikke er verifisert av DNS. Kontroller at domenene er verifisert av DNS for å gjøre prosessen raskere.
