---
title: Micro-forsinkelser eller -begrensning i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702135"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="f5819-102">Micro-forsinkelser eller -begrensning i Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="f5819-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="f5819-103">Du kan se «Micro-forsinkelse i bruk»-advarsler eller forsinkelser når du kjører skript og cmdleter i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f5819-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="f5819-104">Her er noen forslag til hvordan du løser dette:</span><span class="sxs-lookup"><span data-stu-id="f5819-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="f5819-105">Kjør diagnosen vår for å slappe av leierens PowerShell-begrensningspolicyer.</span><span class="sxs-lookup"><span data-stu-id="f5819-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="f5819-106">Denne løsningen løser problemet for de fleste.</span><span class="sxs-lookup"><span data-stu-id="f5819-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="f5819-107">Hvis problemet fremdeles ikke er løst, kan [du bruke Exchange Online v2 PowerShell-modulen](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), som inneholder CMDleter som er basert på REST API og er betydelig mer performant.</span><span class="sxs-lookup"><span data-stu-id="f5819-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="f5819-108">Dette kan være en flott løsning for mange Get-CMDleter som brukes ofte.</span><span class="sxs-lookup"><span data-stu-id="f5819-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="f5819-109">Hvis du trenger å bruke CMDleter som ikke dekkes i v2-modulen, kan du se Kjøre [PowerShell-cmdleter for](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)et stort antall brukere i Office 365 , som snakker om hvordan du kommer deg rundt Begrensninger for PowerShell-begrensning i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f5819-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
