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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="ff3d2-102">Pensjonering av eldre eDiscovery-verktøy</span><span class="sxs-lookup"><span data-stu-id="ff3d2-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="ff3d2-103">Som et resultat av den nye og forbedrede eDiscovery-funksjonaliteten i Microsoft 365 Compliance Center, vil følgende eldre eDiscovery-verktøy og -kommandoer bli pensjonert i de kommende månedene:</span><span class="sxs-lookup"><span data-stu-id="ff3d2-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="ff3d2-104">[EDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) og [På stedet holder](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i administrasjonssenteret for Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff3d2-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="ff3d2-105">Cmdleter for Exchange Online PowerShell som støtter in-Place eDiscovery og på stedet holder.</span><span class="sxs-lookup"><span data-stu-id="ff3d2-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="ff3d2-106">(Disse cmdletene er samlet identifisert som \*-MailboxSearch cmdleter.) Dette inkluderer følgende cmdleter:</span><span class="sxs-lookup"><span data-stu-id="ff3d2-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="ff3d2-107">Søk i ny postboks</span><span class="sxs-lookup"><span data-stu-id="ff3d2-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="ff3d2-108">Start postbokssøk</span><span class="sxs-lookup"><span data-stu-id="ff3d2-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="ff3d2-109">Stopp-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ff3d2-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="ff3d2-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ff3d2-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="ff3d2-111">Cmdleten [Søk postboks](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ff3d2-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="ff3d2-112">Følgende operasjoner i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="ff3d2-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="ff3d2-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff3d2-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="ff3d2-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff3d2-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="ff3d2-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff3d2-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="ff3d2-116">Office 365 Avansert eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="ff3d2-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="ff3d2-117">**Tidslinje for pensjonering**:</span><span class="sxs-lookup"><span data-stu-id="ff3d2-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="ff3d2-118">1. april 2020: Du kan ikke opprette nye søk og sperrer, men du kan fortsatt kjøre, redigere og slette eksisterende søk på egen risiko.</span><span class="sxs-lookup"><span data-stu-id="ff3d2-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="ff3d2-119">Microsoft Support støtter ikke lenger in-place eDiscovery & holder i EAC.</span><span class="sxs-lookup"><span data-stu-id="ff3d2-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="ff3d2-120">1. juli 2020: In-Place eDiscovery & Har funksjonalitet i EAC vil bli plassert i en skrivebeskyttet modus.</span><span class="sxs-lookup"><span data-stu-id="ff3d2-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="ff3d2-121">Dette betyr at du bare kan fjerne eksisterende søk og sperrer.</span><span class="sxs-lookup"><span data-stu-id="ff3d2-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="ff3d2-122">Hvis du vil ha **mer informasjon, kan du se**:</span><span class="sxs-lookup"><span data-stu-id="ff3d2-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="ff3d2-123">Overføre eldre eDiscovery-søk og holder til Microsoft 365-samsvarssenteret</span><span class="sxs-lookup"><span data-stu-id="ff3d2-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="ff3d2-124">Pensjonering av eldre eDiscovery-verktøy</span><span class="sxs-lookup"><span data-stu-id="ff3d2-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="ff3d2-125">Vanlige spørsmål om eDiscovery og på stedet holder</span><span class="sxs-lookup"><span data-stu-id="ff3d2-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



