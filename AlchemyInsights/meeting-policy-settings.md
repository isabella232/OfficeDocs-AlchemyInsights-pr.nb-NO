---
title: Innstillinger for møte policy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627583"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="4a350-102">Administrere møte policyer i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4a350-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="4a350-103">Møte policyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere for møter som planlegges av brukere i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="4a350-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="4a350-104">Det kan hende at enkelte funksjoner i møte policyer ikke implementeres i Teams Administrasjonssenter ennå (disse kalles «kommer snart» i dokumentasjonen).</span><span class="sxs-lookup"><span data-stu-id="4a350-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="4a350-105">I dette tilfellet, eller hvis du får en feilmelding som "vi kan ikke oppdatere policyen akkurat nå, men prøv igjen senere" i administrasjonssenteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre møte policyer for Teams.</span><span class="sxs-lookup"><span data-stu-id="4a350-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="4a350-106">Hvis du vil ha mer informasjon om møte policyer, kan du se følgende ressurser:</span><span class="sxs-lookup"><span data-stu-id="4a350-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="4a350-107">Hvis du vil lære om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [administrere møte policyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="4a350-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="4a350-108">Hvis du vil gjøre policyendringer ved hjelp av PowerShell-cmdleter, kan du se [Teams PowerShell oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="4a350-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="4a350-109">Du må bruke [Skype for Business PowerShell-modul](https://www.microsoft.com/download/details.aspx?id=39366) for Teams møte policyer.</span><span class="sxs-lookup"><span data-stu-id="4a350-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="4a350-110">Se [dokumentasjonen \*-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="4a350-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="4a350-111">**Merk:** Det kan ta opptil 24 timer for policyendringer trer i kraft for brukerne.</span><span class="sxs-lookup"><span data-stu-id="4a350-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="4a350-112">Det er ikke sikkert du kan gjøre endringer i nylig opprettede policyer umiddelbart. vente i 4 timer og forsøke å endre en nyopprettet policy på nytt.</span><span class="sxs-lookup"><span data-stu-id="4a350-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="4a350-113">Hvis du fortsatt har problemer, kan du prøve PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4a350-113">If you're still having problems, try PowerShell.</span></span>  