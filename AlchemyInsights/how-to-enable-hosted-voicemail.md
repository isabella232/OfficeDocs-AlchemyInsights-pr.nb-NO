---
title: Slik aktiverer du telefoni, talepost
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679159"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="882ad-102">Slik aktiverer du telefoni, talepost</span><span class="sxs-lookup"><span data-stu-id="882ad-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="882ad-103">Hvis du vil aktivere talepost, må **HostedVoicemail** være satt til $True.</span><span class="sxs-lookup"><span data-stu-id="882ad-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="882ad-104">**HostedVoicemail** -egenskapen for brukeren som bruker Remote POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="882ad-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="882ad-105">Hvis du vil ha mer informasjon om å koble til RPS, kan du se [Microsoft Teams PowerShell-oversikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for mer informasjon om å koble til RPS.</span><span class="sxs-lookup"><span data-stu-id="882ad-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="882ad-106">Teams-administratoren bør være logget på Remote PowerShell for Teams.</span><span class="sxs-lookup"><span data-stu-id="882ad-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="882ad-107">Fra PowerShell-lede tekst team administrator kan kjøre **Set-csuser User@contoso.com-HostedVoiceMail $True** der SIP-URIen er for den aktuelle brukeren.</span><span class="sxs-lookup"><span data-stu-id="882ad-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="882ad-108">Endringer i policyer kan ha opptil 24 timer å replisere.</span><span class="sxs-lookup"><span data-stu-id="882ad-108">Changes to policies can take up to 24 hours to replicate.</span></span>