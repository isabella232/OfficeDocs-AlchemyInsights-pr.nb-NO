---
title: Behandle synkronisert bruker
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823976"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan ikke angi primær e-postadresse, endre brukerattributter eller fjerne/slette en synkronisert bruker

Hvis katalogsynkronisering er aktivert for miljøet, kan ikke enkelte bruker- eller objektattributter endres ved hjelp av administrasjonssenteret for Microsoft 365.

Hvis du vil administrere synkroniserte brukere og alle attributtene fullstendig, kan du bruke de lokale active directory-brukerne og administrasjonskonsollen for grupper (adsiedit.msc).  

Du kan også endre enkeltbrukere eller attributter for synkroniserte brukere ved hjelp av powershell, for eksempel vist i disse vanlige eksemplene:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
