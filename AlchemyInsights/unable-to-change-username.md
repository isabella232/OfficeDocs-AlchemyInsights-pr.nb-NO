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
# <a name="unable-to-change-username"></a><span data-ttu-id="7e3d7-102">Kan ikke endre brukernavn</span><span class="sxs-lookup"><span data-stu-id="7e3d7-102">Unable to change UserName</span></span>

<span data-ttu-id="7e3d7-103">I noen tilfeller overføres ikke UPN -endringer (UserPrincipalName) til skyen.</span><span class="sxs-lookup"><span data-stu-id="7e3d7-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="7e3d7-104">Du kan få valideringsfeil i Office 365-portalen eller ikke kan endre brukernavnet eller e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="7e3d7-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="7e3d7-105">Hvis du vil løse dette problemet, kan du manuelt angi UserPrincipalName ved hjelp av denne PowerShell-kommandoen.</span><span class="sxs-lookup"><span data-stu-id="7e3d7-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="7e3d7-106">**Eksempel: Gi nytt navn til en bruker**</span><span class="sxs-lookup"><span data-stu-id="7e3d7-106">**Example: Rename a user**</span></span>

<span data-ttu-id="7e3d7-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="7e3d7-107">PowerShellCopy</span></span>

<span data-ttu-id="7e3d7-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="7e3d7-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="7e3d7-109">Denne kommandoen gir nytt navn davidc@contoso.com til davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="7e3d7-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="7e3d7-110">Hvis du vil ha mer informasjon, kan du se [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="7e3d7-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>