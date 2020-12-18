---
title: Problemer med automatisk synkronisering av enhets registrering i Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714829"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="e01d6-102">Problemer med automatisk synkronisering av enhets registrering i Apple</span><span class="sxs-lookup"><span data-stu-id="e01d6-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="e01d6-103">«Vi har oppdaget at du har ett eller flere ADE-eller DEP-tokener som er i en feil tilstand.</span><span class="sxs-lookup"><span data-stu-id="e01d6-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="e01d6-104">Hvis feil tilstanden er løst for hvert berørte token, vil ikke ADE-funksjonaliteten fungere for samme ".</span><span class="sxs-lookup"><span data-stu-id="e01d6-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="e01d6-105">Denne feilen kan være analyser på en rekke måter, inkludert:</span><span class="sxs-lookup"><span data-stu-id="e01d6-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="e01d6-106">Enheter kan ikke synkroniseres fra ABM/ASM til Intune</span><span class="sxs-lookup"><span data-stu-id="e01d6-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="e01d6-107">Registrerings profil tilordninger kan mislykkes</span><span class="sxs-lookup"><span data-stu-id="e01d6-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="e01d6-108">Det kan hende at enheter ikke full fører at ADE-registreringen ble fullført</span><span class="sxs-lookup"><span data-stu-id="e01d6-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="e01d6-109">Se etter synkroniserings feilen som ble rapportert i Intune-konsollen under **enheter > registrere enheter > Apples registrering > registrerings program-tokener** og se gjennom følgende dokumentasjon for å se mulige Utbedring:</span><span class="sxs-lookup"><span data-stu-id="e01d6-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="e01d6-110">ABM/ASM Sync-feil for iOS/iPadOS og macOS automatiserte tokener for enhets registrering</span><span class="sxs-lookup"><span data-stu-id="e01d6-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
