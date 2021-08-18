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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114787"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan ikke angi primær e-postadresse, endre brukerattributter eller fjerne/slette en synkronisert bruker

Hvis katalogsynkronisering er aktivert for miljøet, kan ikke enkelte bruker- eller objektattributter endres ved hjelp av Administrasjonssenter for Microsoft 365.

Hvis du vil administrere synkroniserte brukere og alle attributtene fullstendig, kan du bruke de lokale active directory-brukerne og administrasjonskonsollen for grupper (adsiedit.msc).  

Du kan også endre enkeltbrukere eller attributter for synkroniserte brukere ved hjelp av powershell, for eksempel vist i disse vanlige eksemplene:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
