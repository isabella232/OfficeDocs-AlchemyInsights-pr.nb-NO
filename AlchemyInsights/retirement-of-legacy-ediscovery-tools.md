---
title: Pensjonering av eldre eDiscovery-verktøy
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074683"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensjonering av eldre eDiscovery-verktøy

Som et resultat av den nye og forbedrede eDiscovery-funksjonaliteten i Microsoft 365 compliance-senteret, vil følgende eldre eDiscovery-verktøy og kommandoleter bli fjernet i de kommende månedene:

- [Stedsdekkende eDiscovery-](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [og Stedssperrer](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange administrasjonssenteret.

- De Exchange Online PowerShell-cmdletene som støtter In-Place eDiscovery og In-Place sperringer. (Disse cmdletene identifiseres samlet som *-MailboxSearch-cmdleter.) Dette omfatter følgende cmdleter:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdleten [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Følgende operasjoner i Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje for pensjonering:**
- **1. juli 2020** Du kan ikke lenger opprette nye søk og sperringer, men du kan kjøre, redigere og slette eksisterende søk på eget ansvar. Microsoft Kundestøtte støtter ikke lenger In-Place eDiscovery & sperringer i EAC.
    
- **1. oktober 2020** In-Place eDiscovery & Sperringsfunksjonalitet i EAC plasseres i skrivebeskyttet modus, slik at du bare kan fjerne eksisterende søk og sperringer.

**Hvis du vil ha mer informasjon, kan du se:**

 - [Overføre eldre eDiscovery-søk og sperringer til Samsvarssenter for Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensjonering av eldre eDiscovery-verktøy](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanlige spørsmål om In-Place eDiscovery og In-Place sperringer](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



