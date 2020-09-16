---
title: Pensjon av eldre eDiscovery-verktøy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727792"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensjon av eldre eDiscovery-verktøy

Som et resultat av den nye og forbedrede eDiscovery-funksjonen i Samsvars senteret for Microsoft 365, vil følgende eldre eDiscovery-verktøy og-cmdleter bli trukket tilbake i de kommende månedene:

- [Lokal eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [Lokal sperring](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i administrasjons senteret for Exchange.

- Exchange Online PowerShell-cmdleter som støtter lokal eDiscovery og lokal sperring. (Disse cmdletene er samlet identifisert som *-MailboxSearch-cmdleter.) Dette inkluderer følgende cmdleter:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stopp-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdleten for [søke post boksen](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Følgende operasjoner i API-en for Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avansert eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tids linje for pensjon**:
- **1. juli 2020** Du kan ikke lenger opprette nye søk og sperringer, men du kan kjøre, redigere og slette eksisterende søk på egen risiko. Microsoft kunde støtte støtter ikke lenger lokal eDiscovery-& sperringer i EAC.
    
- **1. oktober 2020** Lokal eDiscovery-& inneholder funksjonalitet i en skrivebeskyttet modus, slik at du bare kan fjerne eksisterende søk og sperringer.

**Hvis du vil ha mer informasjon, kan du se**:

 - [Overføre eldre eDiscovery-søk og sperringer til samsvars senteret for Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensjon av eldre eDiscovery-verktøy](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanlige spørsmål om lokal eDiscovery og lokal sperring](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



