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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750011"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="0c523-102">Søke etter og slette e-postmeldinger i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="0c523-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="0c523-103">Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="0c523-103">Follow these steps:</span></span>

1. <span data-ttu-id="0c523-104">Hvis du ikke er global administrator, må kontoen legges til **i rollegruppen for eDiscovery Manager** eller administrasjonsrollen for samsvarssøk for å søke etter **meldinger.**</span><span class="sxs-lookup"><span data-stu-id="0c523-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="0c523-105">Hvis du vil slette meldinger, må du bli med i rollegruppen **organisasjonsbehandling** eller rollen søk og **tøm behandling.**</span><span class="sxs-lookup"><span data-stu-id="0c523-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="0c523-106">Tillatelser til disse rollene tilordnes i [sikkerhetssenteret & samsvarssenteret.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="0c523-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="0c523-107">[Opprett et innholdssøk for](https://docs.microsoft.com/office365/securitycompliance/content-search) å finne meldingen du vil slette.</span><span class="sxs-lookup"><span data-stu-id="0c523-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="0c523-108">[Koble til PowerShell & sikkerhets- og samsvarssenteret.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0c523-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="0c523-109">Hvis du bruker MFA, kan du se disse instruksjonene: Koble til [Sikkerhetssenter & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) ved hjelp av godkjenning med flere faktorer</span><span class="sxs-lookup"><span data-stu-id="0c523-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="0c523-110">Slett meldingen: Kjør `New-ComplianceSearchAction` cmdleten for å slette meldingen.</span><span class="sxs-lookup"><span data-stu-id="0c523-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="0c523-111">Slettede meldinger flyttes til en brukers gjenopprettelige elementer-mappe.</span><span class="sxs-lookup"><span data-stu-id="0c523-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="0c523-112">Hvis du vil ha en eksempelkommando, [kan du se Trinn 3: Slette meldingen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="0c523-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
