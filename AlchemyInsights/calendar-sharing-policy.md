---
title: 618 Retningslinjer for deling av kalender
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373008"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="31638-102">Policyfeil ved deling av en kalender</span><span class="sxs-lookup"><span data-stu-id="31638-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="31638-103">Gjør ett av følgende, avhengig av situasjonen:</span><span class="sxs-lookup"><span data-stu-id="31638-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="31638-104">Koble til Exchange Online ved hjelp av Ekstern PowerShell.</span><span class="sxs-lookup"><span data-stu-id="31638-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="31638-105">Hvis du vil ha mer informasjon, kan du se [Koble til Exchange Online ved hjelp av Ekstern PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="31638-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="31638-106">Åpne Exchange Management Shell på den lokale serveren.</span><span class="sxs-lookup"><span data-stu-id="31638-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="31638-107">Bestem delingspolicyen som er tilordnet til brukeren.</span><span class="sxs-lookup"><span data-stu-id="31638-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="31638-108">Hvis du vil gjøre dette, kjører du følgende kommando og noterer policyen som returneres:</span><span class="sxs-lookup"><span data-stu-id="31638-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="31638-109">Oppdater delingspolicyen for brukeren.</span><span class="sxs-lookup"><span data-stu-id="31638-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="31638-110">Hvis du vil gjøre dette, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="31638-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="31638-111">Åpne administrasjonssenteret for Exchange.</span><span class="sxs-lookup"><span data-stu-id="31638-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="31638-112">Klikk **Organisasjon**, og dobbeltklikk deretter policyen som er tilordnet til brukeren under **Individuell deling**.</span><span class="sxs-lookup"><span data-stu-id="31638-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="31638-113">Dette er policyen som ble returnert i trinn 2.</span><span class="sxs-lookup"><span data-stu-id="31638-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="31638-114">Velg kalenderdelingsnivået du vil tillate, under Angi **hvilken informasjon du vil dele**. klikk **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="31638-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="31638-115">Hvis du vil ha mer informasjon, kan du se: ["Policyen tillater ikke tildeling av tillatelser på dette nivået til én eller flere av mottakeren(e)"-feil når brukeren prøver å dele kalenderen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="31638-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
