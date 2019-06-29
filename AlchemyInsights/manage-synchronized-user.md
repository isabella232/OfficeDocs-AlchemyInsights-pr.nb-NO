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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Kan ikke angi primær e-postadresse eller endre attributtene for brukeren

Hvis directory-synkronisering er aktivert for ditt miljø kan ikke noen bruker- eller -attributter endres ved hjelp av administrasjonssenteret.
Hvis du vil behandle fullstendig synkroniserte brukere og alle tilhørende attributter, kan du bruke din lokale active directory-brukere og -grupper administrasjonskonsollen (adsiedit.msc).  

Du kan eventuelt endre individuelle brukere eller attributter for synkroniserte brukere ved hjelp av powershell som vises i disse vanlige eksempler: 
- Sett MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Sett MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testbruker" - Etternavn "Bruker"-Tittel "Lederen"-avdelingen "T"
- Fjern MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com