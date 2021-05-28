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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696967"
---
# <a name="11-call-recording"></a><span data-ttu-id="ea332-102">1:1 samtaleopptak</span><span class="sxs-lookup"><span data-stu-id="ea332-102">1:1 call recording</span></span>

<span data-ttu-id="ea332-103">Hvis **Start innspilling-knappen** er nedtonet i et 1:1-anrop, må du endre policyinnstillingene for den berørte brukeren.</span><span class="sxs-lookup"><span data-stu-id="ea332-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="ea332-104">Fra og med 31. mai 2021 begynner vi å bruke en ny Teams Policy for anrop *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="ea332-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="ea332-105">Før denne endringen kontrolleres 1:1-samtaleinnspillingen av *AllowCloudRecording* Teams møtepolicyen.</span><span class="sxs-lookup"><span data-stu-id="ea332-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="ea332-106">Denne endringen er dokumentert i meldingssenterinnlegget: [(Oppdatert) 01:01](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Innføring i policy for innspilling av anrop .</span><span class="sxs-lookup"><span data-stu-id="ea332-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="ea332-107">*AllowCloudRecordingForCalls*   alternativet for anropspolicy er satt **til $False** som standard.</span><span class="sxs-lookup"><span data-stu-id="ea332-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="ea332-108">Hvis du foretrekker å blokkere alle brukere fra å spille inn 1:1-anrop, trenger du ikke å gjøre noe.</span><span class="sxs-lookup"><span data-stu-id="ea332-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="ea332-109">Hvis du vil aktivere samtaleopptak for alle brukere i 1:1-anrop, bruker Teams PowerShell til å kjøre følgende cmdlet:</span><span class="sxs-lookup"><span data-stu-id="ea332-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="ea332-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="ea332-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="ea332-111">Du kan også opprette en ny policy og angi **-AllowCloudRecordingForCalls** til å $true og tilordne denne policyen til brukerne. </span><span class="sxs-lookup"><span data-stu-id="ea332-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="ea332-112">Hvis du vil ha mer informasjon, kan [du se 1:1 Policykontroller for innspilling av anrop er (nesten!) Her](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="ea332-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
