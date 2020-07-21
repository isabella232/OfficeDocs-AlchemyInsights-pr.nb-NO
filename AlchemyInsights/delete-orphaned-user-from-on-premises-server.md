---
title: Slette foreldreløse brukere fra lokal server
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198581"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="e4f2a-102">Slette foreldreløse brukere fra lokal server</span><span class="sxs-lookup"><span data-stu-id="e4f2a-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="e4f2a-103">Hvis du vil fjerne en foreldreløs bruker, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="e4f2a-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="e4f2a-104">Tvinge katalogsynkronisering ved å følge instruksjonene i [Hva er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="e4f2a-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="e4f2a-105">Hvis du vil kontrollere katalogsynkronisering, kan du se [Hva er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="e4f2a-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="e4f2a-106">Hvis synkronisering fungerer på riktig måte, men slettingen av Active Directory-objekt ikke overføres til Azure AD, fjerner du det foreldreløse objektet manuelt ved hjelp av en av følgende Azure Active Directory-modul for Windows PowerShell-cmdleter:</span><span class="sxs-lookup"><span data-stu-id="e4f2a-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="e4f2a-107">Fjern MsolContact</span><span class="sxs-lookup"><span data-stu-id="e4f2a-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="e4f2a-108">Fjern MsolGroup</span><span class="sxs-lookup"><span data-stu-id="e4f2a-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="e4f2a-109">Fjern MsolUser</span><span class="sxs-lookup"><span data-stu-id="e4f2a-109">Remove-MsolUser</span></span>

    <span data-ttu-id="e4f2a-110">Hvis du for eksempel vil fjerne foreldreløse bruker-ID-john.smith@contoso.com, som opprinnelig ble opprettet ved hjelp av katalogsynkronisering, kjører du cmdleten:</span><span class="sxs-lookup"><span data-stu-id="e4f2a-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="e4f2a-111">Fjern MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="e4f2a-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>