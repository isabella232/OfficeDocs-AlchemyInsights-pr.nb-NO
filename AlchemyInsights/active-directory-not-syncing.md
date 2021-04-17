---
title: Active Directory synkroniseres ikke
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822860"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="3adea-102">Active Directory synkroniseres ikke</span><span class="sxs-lookup"><span data-stu-id="3adea-102">Active Directory not syncing</span></span>

<span data-ttu-id="3adea-103">Hvis du mottar synkroniseringsfeil, for eksempel «ingen nylig synkronisering», eller legger merke til at statusen for katalogsynkronisering i administrasjonsportalen for Office sier «Sist synkronisert for mer enn 3 dager siden», kan det være at AADConnect har feil innstillinger eller utilstrekkelige tillatelser til å utføre en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="3adea-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="3adea-104">Hvis du installerer AADConnect på nytt ved hjelp av hurtiginnstillinger, kan dette løse problemet raskt:</span><span class="sxs-lookup"><span data-stu-id="3adea-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="3adea-105">[Last ned den nyeste versjonen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="3adea-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="3adea-106">[Følg instruksjonene for ekspressinstallasjon](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="3adea-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="3adea-107">Hvis du vil ha mer informasjon om AADConnect-tjenestekontoer, kan du se [Azure AD Connect: Kontoer og tillatelser](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="3adea-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
