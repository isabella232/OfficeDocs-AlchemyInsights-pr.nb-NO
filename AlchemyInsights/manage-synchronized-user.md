---
title: Behandle synkronisert bruker
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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407359"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="f58af-102">Kan ikke angi primær e-postadresse, endre brukerattributter eller fjerne/slette en synkronisert bruker</span><span class="sxs-lookup"><span data-stu-id="f58af-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="f58af-103">Hvis katalogsynkronisering er aktivert for miljøet, kan ikke enkelte bruker- eller objektattributter endres ved hjelp av administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f58af-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="f58af-104">Hvis du vil administrere synkroniserte brukere og alle attributtene deres fullt ut, bruker du lokale active directory-brukere og gruppeadministrasjonskonsoll (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="f58af-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="f58af-105">Du kan også endre individuelle brukere eller attributter for synkroniserte brukere ved hjelp av powershell, for eksempel vist i disse vanlige eksemplene:</span><span class="sxs-lookup"><span data-stu-id="f58af-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
