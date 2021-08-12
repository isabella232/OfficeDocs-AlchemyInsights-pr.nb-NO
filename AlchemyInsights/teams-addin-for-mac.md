---
title: Teams for Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940684"
---
# <a name="teams-add-in-for-mac"></a>Teams for Mac

Følg disse trinnene for å feilsøke Teams for Mac-operativsystembrukere:

**Trinn 1:** Hvis du har hybrid Exchange lokalt (2016 CU3 eller nyere kreves), bruker du Test-HMA.ps1-verktøyet til å bekrefte at hybrid moderne godkjenning er riktig konfigurert. Hvis du vil ha mer informasjon, kan du se Validere konfigurasjon av hybrid moderne [godkjenning for Outlook for iOS og Android.](https://aka.ms/TestHMAEAS)  

**Obs!** Bruk UPN-adresseformatet (for eksempel username@contoso.com [),](mailto:username@contoso.com)ikke domene\brukernavn. Gjør dette selv for brukere med Exchange Online postbokser.

**Trinn 2:** Be brukeren gå til **Verktøykontoer**  >  ... i Outlook for Mac, og finn og velg kontoen. Bekreft at brukernavnet som er oppført, er i UPN-format (for [eksempel username@contoso.com](mailto:username@contoso.com)).

**Trinn 3:** Bekreft at brukeren er en lisensiert Microsoft Teams bruker. Brukeren må bruke abonnementet Office 365 for Mac, produkt versjon 16.24 eller nyere.