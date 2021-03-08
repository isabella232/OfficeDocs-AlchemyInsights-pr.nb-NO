---
title: Søke etter og slette e-postmeldinger i organisasjonen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525436"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="d0873-102">Søke etter og slette e-postmeldinger i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="d0873-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="d0873-103">Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="d0873-103">Follow these steps:</span></span>

1. <span data-ttu-id="d0873-104">Hvis du ikke er global administrator, må du legge til kontoen i **rollegruppen for eDiscovery-ansvarlig** eller rollen for samsvarssøkebehandling for å søke etter **meldinger.**</span><span class="sxs-lookup"><span data-stu-id="d0873-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="d0873-105">Hvis du vil slette meldinger, må du bli med i **rollegruppen for** organisasjonsadministrasjon eller rollen Søke etter og **fjerne administrasjon.**</span><span class="sxs-lookup"><span data-stu-id="d0873-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="d0873-106">Tillatelser til disse rollene tilordnes i [sikkerhets- & samsvarssenteret.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="d0873-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="d0873-107">[Opprett et innholdssøk](https://docs.microsoft.com/office365/securitycompliance/content-search) for å finne meldingen du vil slette.</span><span class="sxs-lookup"><span data-stu-id="d0873-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="d0873-108">[Koble til Sikkerhets- &-senteret PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="d0873-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="d0873-109">Hvis du bruker MFA, kan du se disse instruksjonene: Koble til [Sikkerhets-& Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) ved hjelp av godkjenning med flere faktorer</span><span class="sxs-lookup"><span data-stu-id="d0873-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="d0873-110">Slette meldingen: Kjør `New-ComplianceSearchAction` cmdleten for å slette meldingen.</span><span class="sxs-lookup"><span data-stu-id="d0873-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="d0873-111">Slettede meldinger flyttes til en brukers mappe for gjenopprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="d0873-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="d0873-112">Hvis du vil ha en eksempelkommando, kan du se [Trinn 3: Slette meldingen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="d0873-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
