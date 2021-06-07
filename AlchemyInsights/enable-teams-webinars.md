---
title: Aktivere Teams webinarer
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793784"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="a594c-102">Aktivere Teams webinarer</span><span class="sxs-lookup"><span data-stu-id="a594c-102">Enable Teams Webinars</span></span>

<span data-ttu-id="a594c-103">Webinarer er aktivert som standard.</span><span class="sxs-lookup"><span data-stu-id="a594c-103">Webinars are enabled by default.</span></span> <span data-ttu-id="a594c-104">Du kan administrere hvem som kan planlegge og registrere seg for Teams webinarer ved å Teams PowerShell-kommandoer.</span><span class="sxs-lookup"><span data-stu-id="a594c-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="a594c-105">Alle brukere som kan opprette et møte, kan også opprette et nettseminarmøte.</span><span class="sxs-lookup"><span data-stu-id="a594c-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="a594c-106">Hvis du vil administrere hvem som kan planlegge Teams webinarer, bruker du *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="a594c-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="a594c-107">Som standard *er WhoCanRegister* aktivert og satt til **Alle**.</span><span class="sxs-lookup"><span data-stu-id="a594c-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="a594c-108">Hvis du vil deaktivere møteregistrering, setter du *AllowMeetingRegistration til* **False**.</span><span class="sxs-lookup"><span data-stu-id="a594c-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="a594c-109">Hvis du vil endre disse innstillingene, må du [installere Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="a594c-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="a594c-110">Møtepolicyer håndheves også på Teams webinarer.</span><span class="sxs-lookup"><span data-stu-id="a594c-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="a594c-111">Hvis for eksempel anonym sammenføyning er deaktivert i møteinnstillingene, kan anonyme brukere ikke bli med i nettseminarer.</span><span class="sxs-lookup"><span data-stu-id="a594c-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="a594c-112">Hvis du vil lære mer om hvordan du konfigurerer hvem som kan registrere seg for nettseminarer, kan du se Konfigurere hvem som [kan registrere seg for nettseminarer](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="a594c-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="a594c-113">Hvis du vil ha mer informasjon om innstillinger for Microsoft-lister, kan [du se Kontrollere innstillinger for Microsoft-lister](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="a594c-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>