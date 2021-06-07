---
title: Behandle nettseminarregistrering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793913"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="ff44a-102">Behandle nettseminarregistrering</span><span class="sxs-lookup"><span data-stu-id="ff44a-102">Manage webinar registration</span></span>

<span data-ttu-id="ff44a-103">Du administrerer hvem som kan registrere seg Teams webinarer ved å Teams Powershell-kommandoer.</span><span class="sxs-lookup"><span data-stu-id="ff44a-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="ff44a-104">Hvis du vil Teams Powershell, [kan du Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="ff44a-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="ff44a-105">Som standard *er WhoCanRegister* aktivert og satt til **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="ff44a-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="ff44a-106">Hvis du vil tillate at alle, inkludert anonyme brukere, kan registrere seg, må du angi møtepolicyen til **Alle** ved hjelp av Powershell-kommandoen:</span><span class="sxs-lookup"><span data-stu-id="ff44a-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="ff44a-107">**Obs!** Hvis anonym sammenføyning er deaktivert i møteinnstillingene, kan ikke anonyme brukere bli med i nettseminarer.</span><span class="sxs-lookup"><span data-stu-id="ff44a-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="ff44a-108">Hvis du vil lære mer og aktivere denne innstillingen, kan du se [Behandle møteinnstillinger i Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ff44a-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="ff44a-109">Hvis du vil deaktivere møteregistrering, setter du *AllowMeetingRegistration til* **False**.</span><span class="sxs-lookup"><span data-stu-id="ff44a-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="ff44a-110">Hvis du vil lære mer om hvordan du konfigurerer hvem som kan registrere seg for nettseminarer, kan du se Konfigurere hvem som [kan registrere seg for nettseminarer](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="ff44a-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="ff44a-111">Hvis du vil ha mer informasjon om innstillinger for Microsoft-lister, kan [du se Kontrollere innstillinger for Microsoft-lister](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="ff44a-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
