---
title: Bruke Giphy i Teams-samtaler
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982503"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="8c47c-102">Bruke Giphy i Teams-samtaler</span><span class="sxs-lookup"><span data-stu-id="8c47c-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="8c47c-103">Giphy tilgang i Teams chat er aktivert som standard.</span><span class="sxs-lookup"><span data-stu-id="8c47c-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="8c47c-104">Som administrator kan du kontrollere om Giphy er tilgjengelig for brukere ved [å angi en meldings policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) og sørge for at **Bruk giphy i samtaler** er **aktivert**.</span><span class="sxs-lookup"><span data-stu-id="8c47c-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="8c47c-105">Hvis GIF-en ikke fungerer som forventet i Teams-samtaler, må du bekrefte:</span><span class="sxs-lookup"><span data-stu-id="8c47c-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="8c47c-106">[Meldings policyen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) må tillate giphy.</span><span class="sxs-lookup"><span data-stu-id="8c47c-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="8c47c-107">Slik kontrollerer du ved å bruke PowerShell-cmdleter:</span><span class="sxs-lookup"><span data-stu-id="8c47c-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="8c47c-108">Kontroller at du kan [administrere Teams med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="8c47c-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="8c47c-109">Kjør PowerShell-kommandoen [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) , og kontroller at **AllowGiphy** er satt til **True**.</span><span class="sxs-lookup"><span data-stu-id="8c47c-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="8c47c-110">Hvis **AllowGiphy** er satt til **False** , kjører du følgende PowerShell-kommando [Sett-CsTeamsMessagingPolicy-Identity global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="8c47c-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="8c47c-111">[Valg frie tilkoblede opplevelser](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) må være aktivert for å tillate tilgang til Giphy-URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="8c47c-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="8c47c-112">Hvis du har flere Teams meldings policyer konfigurert for leieren din, kan du bestemme identiteten til policyen som er tilordnet den berørte brukeren med PowerShell-kommandoen [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Velg TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="8c47c-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
