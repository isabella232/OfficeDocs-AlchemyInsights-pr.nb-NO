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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798558"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="fe1be-102">Pensjonering av eldre eDiscovery-verktøy</span><span class="sxs-lookup"><span data-stu-id="fe1be-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="fe1be-103">Som et resultat av den nye og forbedrede eDiscovery-funksjonaliteten i Samsvarssenteret for Microsoft 365, vil følgende eldre eDiscovery-verktøy og kommandoleter bli fjernet i de kommende månedene:</span><span class="sxs-lookup"><span data-stu-id="fe1be-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="fe1be-104">[Stedsdekkende eDiscovery-](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [og På stedet-sperringer i administrasjonssenteret](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) for Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe1be-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="fe1be-105">Exchange Online PowerShell-cmdleter som støtter In-Place eDiscovery og In-Place sperringer.</span><span class="sxs-lookup"><span data-stu-id="fe1be-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="fe1be-106">(Disse cmdletene identifiseres samlet som \*-MailboxSearch-cmdleter.) Dette omfatter følgende cmdleter:</span><span class="sxs-lookup"><span data-stu-id="fe1be-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="fe1be-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fe1be-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="fe1be-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fe1be-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="fe1be-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fe1be-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="fe1be-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="fe1be-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="fe1be-111">Cmdleten [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fe1be-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="fe1be-112">Følgende operasjoner i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="fe1be-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="fe1be-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="fe1be-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="fe1be-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="fe1be-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="fe1be-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="fe1be-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="fe1be-116">Avansert eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="fe1be-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="fe1be-117">**Tidslinje for pensjonering:**</span><span class="sxs-lookup"><span data-stu-id="fe1be-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="fe1be-118">**1. juli 2020** Du kan ikke lenger opprette nye søk og sperringer, men du kan kjøre, redigere og slette eksisterende søk på eget ansvar.</span><span class="sxs-lookup"><span data-stu-id="fe1be-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="fe1be-119">Microsoft Kundestøtte støtter ikke lenger In-Place eDiscovery & sperringer i EAC.</span><span class="sxs-lookup"><span data-stu-id="fe1be-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="fe1be-120">**1. oktober 2020** In-Place eDiscovery & Sperringsfunksjonalitet i EAC plasseres i skrivebeskyttet modus, slik at du bare kan fjerne eksisterende søk og sperringer.</span><span class="sxs-lookup"><span data-stu-id="fe1be-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="fe1be-121">**Hvis du vil ha mer informasjon, kan du se:**</span><span class="sxs-lookup"><span data-stu-id="fe1be-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="fe1be-122">Overføre eldre eDiscovery-søk og sperringer til Samsvarssenteret for Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fe1be-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="fe1be-123">Pensjonering av eldre eDiscovery-verktøy</span><span class="sxs-lookup"><span data-stu-id="fe1be-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="fe1be-124">Vanlige spørsmål om In-Place eDiscovery og In-Place sperringer</span><span class="sxs-lookup"><span data-stu-id="fe1be-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



