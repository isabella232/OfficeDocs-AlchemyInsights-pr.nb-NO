---
title: Delings policy for 618-kalender
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684239"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="712a5-102">Policy feil ved deling av en kalender</span><span class="sxs-lookup"><span data-stu-id="712a5-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="712a5-103">Gjør ett av følgende, avhengig av situasjonen:</span><span class="sxs-lookup"><span data-stu-id="712a5-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="712a5-104">Koble til Exchange Online ved hjelp av Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="712a5-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="712a5-105">Hvis du vil ha mer informasjon, kan du se [Koble til Exchange Online ved hjelp av Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="712a5-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="712a5-106">Åpne administrasjons grensesnittet for Exchange på den lokale serveren.</span><span class="sxs-lookup"><span data-stu-id="712a5-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="712a5-107">Bestemme Delings policyen som er tilordnet til brukeren.</span><span class="sxs-lookup"><span data-stu-id="712a5-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="712a5-108">Hvis du vil gjøre dette, kjører du følgende kommando og noterer policyen som returneres:</span><span class="sxs-lookup"><span data-stu-id="712a5-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="712a5-109">Oppdater Delings policyen for brukeren.</span><span class="sxs-lookup"><span data-stu-id="712a5-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="712a5-110">Dette gjør du slik:</span><span class="sxs-lookup"><span data-stu-id="712a5-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="712a5-111">Åpne administrasjons senteret for Exchange.</span><span class="sxs-lookup"><span data-stu-id="712a5-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="712a5-112">Klikk **organisasjon**, og dobbelt klikk deretter policyen som er tilordnet brukeren under **individuell deling**.</span><span class="sxs-lookup"><span data-stu-id="712a5-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="712a5-113">Dette er policyen som ble returnert i trinn 2.</span><span class="sxs-lookup"><span data-stu-id="712a5-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="712a5-114">På siden Delings regel velger du Kalender Delings nivået du vil tillate under **Angi hvilken informasjon du vil dele**. Klikk **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="712a5-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="712a5-115">Hvis du vil ha mer informasjon, kan du se [«policyen tillater ikke tildeling av tillatelser på dette nivået til én eller flere mottakere av mottaker (s) når brukeren prøver å dele kalenderen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="712a5-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
