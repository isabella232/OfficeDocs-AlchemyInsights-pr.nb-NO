---
title: Arkiv post boksen er nesten full
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974409"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="0d723-102">Arkiv post boksen er nesten full</span><span class="sxs-lookup"><span data-stu-id="0d723-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="0d723-103">Hvis brukeren mottar advarselen, **Arkiv post boksen er nesten full**, eller du må øke størrelsen på arkiv post boksen, her er noen tips:</span><span class="sxs-lookup"><span data-stu-id="0d723-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="0d723-104">Hvis brukeren er tilordnet en Exchange Online-plan 1, oppgraderer du til **Exchange Online plan 2** -lisensen for å øke størrelsen fra 50 GB til 100 GB.</span><span class="sxs-lookup"><span data-stu-id="0d723-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="0d723-105">Hvis brukeren allerede er tilordnet ett av følgende: **Exchange Online plan 2** eller en Exchange Online-plan 1 med et Exchange Online arkiverings tillegg, bruker du Fremgangs måten nedenfor for å aktivere automatisk justering av arkivering:.</span><span class="sxs-lookup"><span data-stu-id="0d723-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="0d723-106">[Koble til Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="0d723-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="0d723-107">Kjør følgende unifiedgroup for brukeren:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="0d723-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="0d723-108">Kjør følgende unifiedgroup for å bekrefte at den er aktivert for brukeren:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="0d723-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="0d723-109">Hvis du vil ha mer informasjon, se:</span><span class="sxs-lookup"><span data-stu-id="0d723-109">For more information see:</span></span>

- [<span data-ttu-id="0d723-110"> Aktiver ubegrenset arkivering – hjelp for administratorer – samsvar med Microsoft 365 | Microsoft-dokumenter</span><span class="sxs-lookup"><span data-stu-id="0d723-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="0d723-111">Begrensninger på Exchange Online – tjeneste beskrivelser | Microsoft-dokumenter</span><span class="sxs-lookup"><span data-stu-id="0d723-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="0d723-112">Oppgrader til en annen forretnings plan | Microsoft-dokumenter</span><span class="sxs-lookup"><span data-stu-id="0d723-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

