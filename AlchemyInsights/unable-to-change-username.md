---
title: Kan ikke endre brukernavn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440292"
---
# <a name="unable-to-change-username"></a>Kan ikke endre brukernavn

I noen tilfeller overføres ikke UPN -endringer (UserPrincipalName) til skyen. Du kan få valideringsfeil i Office 365-portalen eller ikke kan endre brukernavnet eller e-postadressen. Hvis du vil løse dette problemet, kan du manuelt angi UserPrincipalName ved hjelp av denne PowerShell-kommandoen.

**Eksempel: Gi nytt navn til en bruker**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Denne kommandoen gir nytt navn davidc@contoso.com til davidchew@contoso.com.

Hvis du vil ha mer informasjon, kan du se [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).