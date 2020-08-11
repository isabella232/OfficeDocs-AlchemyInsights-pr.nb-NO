---
title: Teams-tillegget for Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629743"
---
# <a name="teams-add-in-for-mac"></a>Teams-tillegget for Mac

Følg denne Fremgangs måten for å feilsøke et manglende Teams-tillegg for Mac-brukere av operativ systemet:

**Trinn 1:** Hvis du har hybrid Exchange lokalt (2016 CU3 eller senere kreves), bruker du Test-HMA.ps1-verktøyet til å bekrefte at hybrid moderne godkjenning er riktig konfigurert. Hvis du vil ha mer informasjon, kan du se [validere hybrid moderne godkjennings konfigurasjon for Outlook for IOS og Android](https://aka.ms/AA980zq).  

**Obs!** Bruk UPN-adresse formatet (for eksempel [username@contoso.com](mailto:username@contoso.com)), ikke Domain\Username. Gjør dette selv for brukere med Exchange Online-postbokser.

**Trinn 2:** Få brukeren til å gå til **verktøy**  >  **kontoer**... i Outlook for Mac, og Finn og velg kontoen. Bekreft at bruker navnet som er oppført, er i UPN-format (for eksempel [username@contoso.com](mailto:username@contoso.com)).

**Trinn 3:** Bekreft at brukeren er en lisensiert Microsoft Teams-bruker. Brukeren må bruke Office 365 for Mac-abonnementet, produkt versjon 16,24 eller nyere.