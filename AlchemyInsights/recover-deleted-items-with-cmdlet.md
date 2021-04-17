---
title: Gjenopprette slettede elementer med cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835820"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="24909-102">Gjenopprette slettede elementer med cmdlet</span><span class="sxs-lookup"><span data-stu-id="24909-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="24909-103">Bruk [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet til å vise slettede elementer i postbokser.</span><span class="sxs-lookup"><span data-stu-id="24909-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="24909-104">Når du har funnet de slettede elementene, kan du bruke [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet å gjenopprette dem.</span><span class="sxs-lookup"><span data-stu-id="24909-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="24909-105">Se alle detaljene i [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="24909-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="24909-106">Du må være tildelt en rolle for import og eksport av postboks før du kan kjøre cmdlet.</span><span class="sxs-lookup"><span data-stu-id="24909-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="24909-107">Se [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="24909-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
