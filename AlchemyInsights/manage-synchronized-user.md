---
title: Behandle synkroniserte brukere
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451409"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Kan ikke angi primær e-postadresse, endre bruker attributter eller fjerne/slette en synkronisert bruker

Hvis katalog synkronisering er aktivert for miljøet, kan ikke enkelte User-eller Object-attributter endres ved hjelp av administrasjons senteret for Microsoft 365.

Hvis du vil administrere synkroniserte brukere og alle tilhørende attributter, bruker du lokale Active Directory-brukere og grupper administrasjons konsoll (Adsiedit. msc).  

Alternativt kan du endre individuelle brukere eller attributter for synkroniserte brukere ved bruk av PowerShell, for eksempel vist i disse vanlige eksemplene:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
