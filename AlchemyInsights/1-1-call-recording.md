---
title: 1:1 samtaleopptak
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733858"
---
# <a name="11-call-recording"></a><span data-ttu-id="aebff-102">1:1 samtaleopptak</span><span class="sxs-lookup"><span data-stu-id="aebff-102">1:1 call recording</span></span>

<span data-ttu-id="aebff-103">Administratorer må nå gjøre noe for å fortsette å tillate brukere å spille inn 1:1-anrop.</span><span class="sxs-lookup"><span data-stu-id="aebff-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="aebff-104">Fra og med 12. april 2021 begynner vi å bruke et nytt alternativ for anropspolicy for Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="aebff-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="aebff-105">Funksjonene for samtaleinnspilling 1:1 kontrolleres for øyeblikket av *tillatCloudRecording-alternativet* i teams møtepolicyer.</span><span class="sxs-lookup"><span data-stu-id="aebff-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="aebff-106">Hvis brukerne har tillatelse til å spille inn Teams-møter, kan de også ta opp 1:1-samtaler.</span><span class="sxs-lookup"><span data-stu-id="aebff-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="aebff-107">Hvis du foretrekker å blokkere alle brukere fra å spille inn 1:1-samtaler, trenger du ikke å gjøre noe.</span><span class="sxs-lookup"><span data-stu-id="aebff-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="aebff-108">*AllowCloudRecordingForCalls* anropspolicyalternativ velges $False som standard.</span><span class="sxs-lookup"><span data-stu-id="aebff-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="aebff-109">Denne endringen er dokumentert i følgende meldingssenterinnlegg: (oppdatert) innføring i policy for innspilling av anrop [1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) For å angi alternativet for anropspolicy for Teams, må du bruke [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="aebff-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="aebff-110">**Slik aktiverer du samtaleopptak i 1:1-samtaler:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="aebff-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="aebff-111">**Slik deaktiverer du samtaleopptak i 1:1-samtaler:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="aebff-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

