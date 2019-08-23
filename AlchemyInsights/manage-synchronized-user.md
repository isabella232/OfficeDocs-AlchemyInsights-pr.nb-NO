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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542007"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="3e8eb-102">Kan ikke angi primær e-postadresse eller endre attributtene for brukeren</span><span class="sxs-lookup"><span data-stu-id="3e8eb-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="3e8eb-103">Hvis directory-synkronisering er aktivert for ditt miljø, kan ikke noen bruker- eller -attributter endres ved hjelp av Microsoft 365 administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="3e8eb-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="3e8eb-104">Hvis du vil behandle fullstendig synkroniserte brukere og alle tilhørende attributter, kan du bruke din lokale active directory-brukere og -grupper administrasjonskonsollen (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="3e8eb-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="3e8eb-105">Du kan eventuelt endre individuelle brukere eller attributter for synkroniserte brukere ved hjelp av powershell som vises i disse vanlige eksempler:</span><span class="sxs-lookup"><span data-stu-id="3e8eb-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="3e8eb-106">Sett MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="3e8eb-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="3e8eb-107">Sett MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testbruker" - Etternavn "Bruker"-Tittel "Lederen"-avdelingen "T"</span><span class="sxs-lookup"><span data-stu-id="3e8eb-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="3e8eb-108">Fjern MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="3e8eb-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>