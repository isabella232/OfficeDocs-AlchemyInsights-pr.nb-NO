---
title: Pensjonering av eldre eDiscovery-verktøy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600387"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensjonering av eldre eDiscovery-verktøy

Som et resultat av den nye og forbedrede eDiscovery-funksjonaliteten i Microsoft 365 Compliance center, vil følgende eldre eDiscovery-verktøy og -kommandoer bli pensjonert i de kommende månedene:

- [Lokale eDiscovery-](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [In-Place-sperringer i](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) administrasjonssenteret for Exchange.

- Exchange Online PowerShell-cmdleter som støtter innebygde eDiscovery- og In-Place-sperrer. (Disse cmdleter er kollektivt identifisert som *-MailboxSearch cmdlets.) Dette inkluderer følgende cmdleter:

    - [Nytt postbokssøk](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-PostboksSøk](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stopp-postboksSøk](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Sett postbokssøk](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdleten Søk-postboks](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Følgende operasjoner i Exchange Web Services API:
    - [Få SøkbarePostbokser](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes (SettHoldOnMailboxes)](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes (andre betydninger)](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avansert eDiscovery for Office 365](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje for pensjonering**:
- 1. april 2020: Du kan ikke opprette nye søk og sperrer, men du kan fortsatt kjøre, redigere og slette eksisterende søk på egen risiko. Microsoft Support støtter ikke lenger eDiscovery-& holder i EAC.

- 1. juli 2020: Funksjonen på stedet eDiscovery & Holder i EAC vil bli plassert i skrivebeskyttet modus. Dette betyr at du bare kan fjerne eksisterende søk og sperrer.

**Hvis du vil ha mer informasjon, kan du se**:

 - [Overføre eldre eDiscovery-søk og holder til Microsoft 365-samsvarssenteret](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensjonering av eldre eDiscovery-verktøy](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanlige spørsmål om eDiscovery og på stedet](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



