---
title: Gjenopprette slettede elementer med cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493167"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="611ad-102">Gjenopprette slettede elementer med cmdlet</span><span class="sxs-lookup"><span data-stu-id="611ad-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="611ad-103">Bruk cmdleten [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) til å vise slettede elementer i postbokser.</span><span class="sxs-lookup"><span data-stu-id="611ad-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="611ad-104">Når du finner de slettede elementene, kan du bruke cmdleten [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) til å gjenopprette dem.</span><span class="sxs-lookup"><span data-stu-id="611ad-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="611ad-105">Se fullstendige detaljer i [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="611ad-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="611ad-106">Du må tilordnes rollen Eksporter for postboksimport før du kan kjøre denne cmdleten.</span><span class="sxs-lookup"><span data-stu-id="611ad-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="611ad-107">Se [Get-RecoverableItems hvis](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="611ad-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
