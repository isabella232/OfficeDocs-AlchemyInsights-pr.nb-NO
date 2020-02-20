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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157660"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensjonering av eldre eDiscovery-verktøy

Som et resultat av den nye og forbedrede eDiscovery-funksjonaliteten i Microsoft 365 Compliance Center, vil følgende eldre eDiscovery-verktøy og -kommandoer bli pensjonert i de kommende månedene:

- [EDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [På stedet holder](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i administrasjonssenteret for Exchange.

- Cmdleter for Exchange Online PowerShell som støtter in-Place eDiscovery og på stedet holder. (Disse cmdletene er samlet identifisert som *-MailboxSearch cmdleter.) Dette inkluderer følgende cmdleter:

    - [Søk i ny postboks](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start postbokssøk](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stopp-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdleten [Søk postboks](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Følgende operasjoner i Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Avansert eDiscovery v1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje for pensjonering**:
- 1. april 2020: Du kan ikke opprette nye søk og sperrer, men du kan fortsatt kjøre, redigere og slette eksisterende søk på egen risiko. Microsoft Support støtter ikke lenger in-place eDiscovery & holder i EAC.

- 1. juli 2020: In-Place eDiscovery & Har funksjonalitet i EAC vil bli plassert i en skrivebeskyttet modus. Dette betyr at du bare kan fjerne eksisterende søk og sperrer.

Hvis du vil ha **mer informasjon, kan du se**:

 - [Overføre eldre eDiscovery-søk og holder til Microsoft 365-samsvarssenteret](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensjonering av eldre eDiscovery-verktøy](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanlige spørsmål om eDiscovery og på stedet holder](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



