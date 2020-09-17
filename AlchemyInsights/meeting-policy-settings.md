---
title: Innstillinger for møte policy
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794343"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="9b8f7-102">Behandle møte policyer i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9b8f7-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="9b8f7-103">**Obs! det kan ha opptil 24 timer før policy endringer trer i kraft for brukere.**</span><span class="sxs-lookup"><span data-stu-id="9b8f7-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="9b8f7-104">Det kan hende du ikke kan gjøre endringer i nylig opprettede policyer umiddelbart. Vent 4 timer, og prøv å endre en nylig opprettet policy på nytt.</span><span class="sxs-lookup"><span data-stu-id="9b8f7-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="9b8f7-105">Møte policyer brukes til å kontrollere funksjonene som er tilgjengelige for møte deltakere for møter som er planlagt av brukere i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="9b8f7-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="9b8f7-106">Noen funksjoner for møte policyer er kanskje ikke implementert i administrasjons senteret for Teams ennå (disse er merket "kommer snart" i dokumentasjonen).</span><span class="sxs-lookup"><span data-stu-id="9b8f7-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="9b8f7-107">I dette tilfellet, hvis du får en feil melding om at vi ikke kan oppdatere policyen, men prøv den på nytt senere i administrasjons senteret for Microsoft Teams, anbefaler vi at du bruker PowerShell til å opprette eller endre teamets møte retnings linjer.</span><span class="sxs-lookup"><span data-stu-id="9b8f7-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="9b8f7-108">Hvis du vil ha mer informasjon om møte policyer, kan du se følgende ressurser:</span><span class="sxs-lookup"><span data-stu-id="9b8f7-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="9b8f7-109">Hvis du vil lære om hvordan du oppretter policyer, gjør endringer og tilordner brukere til policyen, kan du se [Behandle møte policyer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="9b8f7-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="9b8f7-110">Se [Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)for å gjøre policy endringer ved hjelp av PowerShell-cmdleter.</span><span class="sxs-lookup"><span data-stu-id="9b8f7-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="9b8f7-111">Du må bruke [Skype for Business PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) for Teams-policyer.</span><span class="sxs-lookup"><span data-stu-id="9b8f7-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="9b8f7-112">Se gjennom [dokumentasjonen for \*-CsTeamsMeetingPolicy-cmdleten](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="9b8f7-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

