---
title: Synkroniseringsfeil ved automatisk registrering av Apple-enhet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448931"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="1f865-102">Synkroniseringsfeil ved automatisk registrering av Apple-enhet</span><span class="sxs-lookup"><span data-stu-id="1f865-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="1f865-103">«Vi har oppdaget at du har ett eller flere ADE-/DEP-tokener som er i en feiltilstand.</span><span class="sxs-lookup"><span data-stu-id="1f865-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="1f865-104">Før feiltilstanden er løst for hvert berørte token, vil ikke ADE-funksjonaliteten fungere som forventet.</span><span class="sxs-lookup"><span data-stu-id="1f865-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="1f865-105">Denne feilen kan manifesteres på en rekke måter, blant annet:</span><span class="sxs-lookup"><span data-stu-id="1f865-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="1f865-106">Enheter kan ikke synkronisere fra ABM/ASM til Intune</span><span class="sxs-lookup"><span data-stu-id="1f865-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="1f865-107">Registreringsprofiltilordninger kan mislykkes</span><span class="sxs-lookup"><span data-stu-id="1f865-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="1f865-108">Det kan hende at ADE-registreringen av enheter ikke fullføres</span><span class="sxs-lookup"><span data-stu-id="1f865-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="1f865-109">Se etter synkroniseringsfeilen som ble rapportert i Intune-konsollen under >-enheter > **Apple-registreringstokener > registreringsprogram.**</span><span class="sxs-lookup"><span data-stu-id="1f865-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="1f865-110">En av de vanligste årsakene til synkroniseringsfeil er utløp av gjeldende token.</span><span class="sxs-lookup"><span data-stu-id="1f865-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="1f865-111">I mange tilfeller vil fornyelse av det berørte tokenet løse problemet.</span><span class="sxs-lookup"><span data-stu-id="1f865-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="1f865-112">Hvis ett eller flere av tokenene er utløpt, kan du se følgende dokumentasjon for å hjelpe deg med å fornye dem etter behov:</span><span class="sxs-lookup"><span data-stu-id="1f865-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="1f865-113">Fornye et token for automatisert enhetsregistrering</span><span class="sxs-lookup"><span data-stu-id="1f865-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="1f865-114">I tillegg kan du se følgende dokumentasjon for å se potensielle utbedringer for andre feil som forårsaker mislykkede tokensynkroniseringer:</span><span class="sxs-lookup"><span data-stu-id="1f865-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="1f865-115">ABM-/ASM-synkroniseringsfeil for iOS/iPadOS og macOS-tokener for automatisert enhetsregistrering</span><span class="sxs-lookup"><span data-stu-id="1f865-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="1f865-116">ABM-/ASM-synkroniseringsfeil for iOS/iPadOS og macOS-tokener for automatisert enhetsregistrering</span><span class="sxs-lookup"><span data-stu-id="1f865-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
