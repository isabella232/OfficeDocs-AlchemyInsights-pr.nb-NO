---
title: Teams-tillegget for Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670337"
---
# <a name="teams-add-in-for-mac"></a>Teams-tillegget for Mac

Følg denne Fremgangs måten for å feilsøke et manglende Teams-tillegg for Mac-brukere av operativ systemet:

**Trinn 1:** Hvis du har hybrid Exchange lokalt (2016 CU3 eller senere kreves), bruker du Test-HMA.ps1-verktøyet til å bekrefte at hybrid moderne godkjenning er riktig konfigurert. Hvis du vil ha mer informasjon, kan du se [validere hybrid moderne godkjennings konfigurasjon for Outlook for IOS og Android](https://aka.ms/AA980zq).  

**Obs!** Bruk UPN-adresse formatet (for eksempel [username@contoso.com](mailto:username@contoso.com)), ikke Domain\Username. Gjør dette selv for brukere med Exchange Online-postbokser.

**Trinn 2:** Få brukeren til å gå til **verktøy**  >  **kontoer**... i Outlook for Mac, og Finn og velg kontoen. Bekreft at bruker navnet som er oppført, er i UPN-format (for eksempel [username@contoso.com](mailto:username@contoso.com)).

**Trinn 3:** Bekreft at brukeren er en lisensiert Microsoft Teams-bruker. Brukeren må bruke Office 365 for Mac-abonnementet, produkt versjon 16,24 eller nyere.