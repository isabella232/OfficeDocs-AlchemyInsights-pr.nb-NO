---
title: Styre synkroniserte bruker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380514"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="b6cc3-102">Kan ikke angi primær e-postadresse eller endre attributtene for brukeren</span><span class="sxs-lookup"><span data-stu-id="b6cc3-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="b6cc3-103">Hvis directory-synkronisering er aktivert for ditt miljø kan ikke noen bruker- eller -attributter endres ved hjelp av administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="b6cc3-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="b6cc3-104">Hvis du vil behandle fullstendig synkroniserte brukere og alle tilhørende attributter, kan du bruke din lokale active directory-brukere og -grupper administrasjonskonsollen (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="b6cc3-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="b6cc3-105">Du kan eventuelt endre individuelle brukere eller attributter for synkroniserte brukere ved hjelp av powershell som vises i disse vanlige eksempler:</span><span class="sxs-lookup"><span data-stu-id="b6cc3-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="b6cc3-106">Sett MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b6cc3-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="b6cc3-107">Sett MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testbruker" - Etternavn "Bruker"-Tittel "Lederen"-avdelingen "T"</span><span class="sxs-lookup"><span data-stu-id="b6cc3-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="b6cc3-108">Fjern MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b6cc3-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>