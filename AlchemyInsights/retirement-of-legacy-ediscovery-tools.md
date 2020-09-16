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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="cb5bc-102">Pensjon av eldre eDiscovery-verktøy</span><span class="sxs-lookup"><span data-stu-id="cb5bc-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="cb5bc-103">Som et resultat av den nye og forbedrede eDiscovery-funksjonen i Samsvars senteret for Microsoft 365, vil følgende eldre eDiscovery-verktøy og-cmdleter bli trukket tilbake i de kommende månedene:</span><span class="sxs-lookup"><span data-stu-id="cb5bc-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="cb5bc-104">[Lokal eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [Lokal sperring](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i administrasjons senteret for Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb5bc-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="cb5bc-105">Exchange Online PowerShell-cmdleter som støtter lokal eDiscovery og lokal sperring.</span><span class="sxs-lookup"><span data-stu-id="cb5bc-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="cb5bc-106">(Disse cmdletene er samlet identifisert som \*-MailboxSearch-cmdleter.) Dette inkluderer følgende cmdleter:</span><span class="sxs-lookup"><span data-stu-id="cb5bc-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="cb5bc-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="cb5bc-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="cb5bc-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="cb5bc-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="cb5bc-109">Stopp-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="cb5bc-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="cb5bc-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="cb5bc-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="cb5bc-111">Cmdleten for [søke post boksen](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cb5bc-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="cb5bc-112">Følgende operasjoner i API-en for Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="cb5bc-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="cb5bc-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="cb5bc-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="cb5bc-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="cb5bc-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="cb5bc-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="cb5bc-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="cb5bc-116">Avansert eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="cb5bc-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="cb5bc-117">**Tids linje for pensjon**:</span><span class="sxs-lookup"><span data-stu-id="cb5bc-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="cb5bc-118">**1. juli 2020** Du kan ikke lenger opprette nye søk og sperringer, men du kan kjøre, redigere og slette eksisterende søk på egen risiko.</span><span class="sxs-lookup"><span data-stu-id="cb5bc-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="cb5bc-119">Microsoft kunde støtte støtter ikke lenger lokal eDiscovery-& sperringer i EAC.</span><span class="sxs-lookup"><span data-stu-id="cb5bc-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="cb5bc-120">**1. oktober 2020** Lokal eDiscovery-& inneholder funksjonalitet i en skrivebeskyttet modus, slik at du bare kan fjerne eksisterende søk og sperringer.</span><span class="sxs-lookup"><span data-stu-id="cb5bc-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="cb5bc-121">**Hvis du vil ha mer informasjon, kan du se**:</span><span class="sxs-lookup"><span data-stu-id="cb5bc-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="cb5bc-122">Overføre eldre eDiscovery-søk og sperringer til samsvars senteret for Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cb5bc-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="cb5bc-123">Pensjon av eldre eDiscovery-verktøy</span><span class="sxs-lookup"><span data-stu-id="cb5bc-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="cb5bc-124">Vanlige spørsmål om lokal eDiscovery og lokal sperring</span><span class="sxs-lookup"><span data-stu-id="cb5bc-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



