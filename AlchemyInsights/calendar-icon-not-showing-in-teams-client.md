---
title: Kalenderikon som ikke vises i Teams-klienten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819962"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="6135c-102">Kalenderikon som ikke vises i Teams-klienten</span><span class="sxs-lookup"><span data-stu-id="6135c-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="6135c-103">Kalenderfanen i Teams krever tilgang til en Exchange-postboks via Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="6135c-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="6135c-104">Exchange-postboksen kan være Tilkoblet eller Lokal.</span><span class="sxs-lookup"><span data-stu-id="6135c-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="6135c-105">For brukere på Internett som ikke kan se Kalenderfanen, må du kontrollere at de [er lisensiert for en Exchange Online-postboks og at postboksen er aktivert](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="6135c-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="6135c-106">Hvis brukeren har en gyldig postboks i Exchange Online, men fremdeles ikke kan se kalenderfanen, har du kanskje et nettverks problem.</span><span class="sxs-lookup"><span data-stu-id="6135c-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="6135c-107">Bruk [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) og Kjør **Microsoft Exchange Web Services (EWS) tilkoblingstester** for den berørte brukeren.</span><span class="sxs-lookup"><span data-stu-id="6135c-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="6135c-108">Til slutt sjekker du [Teams-appene – Policyer for appoppsett](https://admin.teams.microsoft.com/policies/app-setup) for å sikre at kalenderappen ikke har blitt fjernet fra policyen som brukes for brukeren (mest sannsynlig er den **Global (organisasjonsomfattende standard)**.</span><span class="sxs-lookup"><span data-stu-id="6135c-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="6135c-109">Hvis brukerne dine befinner seg lokalt, må du bekrefte at hybridkonfigurasjonen er OK.</span><span class="sxs-lookup"><span data-stu-id="6135c-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="6135c-110">Bruk [Veiviseren for hybridkonfigurasjon](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) for å feilsøke.</span><span class="sxs-lookup"><span data-stu-id="6135c-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="6135c-111">Vær obs på at [Teams krever Exchange 2016 CU3 eller nyere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="6135c-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
