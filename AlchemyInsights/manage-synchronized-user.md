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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan ikke angi primær e-postadresse, endre brukerattributter eller fjerne/slette en synkronisert bruker

Hvis katalogsynkronisering er aktivert for miljøet, kan ikke enkelte bruker- eller objektattributter endres ved hjelp av administrasjonssenteret for Microsoft 365.

Hvis du vil administrere synkroniserte brukere og alle attributtene deres fullt ut, bruker du lokale active directory-brukere og gruppeadministrasjonskonsoll (adsiedit.msc).  

Du kan også endre individuelle brukere eller attributter for synkroniserte brukere ved hjelp av powershell, for eksempel vist i disse vanlige eksemplene: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
