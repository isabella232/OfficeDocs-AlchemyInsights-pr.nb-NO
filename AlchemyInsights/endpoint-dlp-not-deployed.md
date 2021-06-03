---
title: Endepunkt-DLP ikke distribuert til brukerens enhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731590"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="34bf2-102">Endepunkt-DLP ikke distribuert til brukerens enhet</span><span class="sxs-lookup"><span data-stu-id="34bf2-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="34bf2-103">Hvis DLP-innstillingen (Endpoint Data Loss Prevention) ikke er brukt på en brukers enhet, må du bekrefte at du oppfyller disse kravene:</span><span class="sxs-lookup"><span data-stu-id="34bf2-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="34bf2-104">Windows 10 x64 bygg 1809 eller nyere er installert på enheten.</span><span class="sxs-lookup"><span data-stu-id="34bf2-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="34bf2-105">Klientversjon 4.18.2009.7 eller nyere for skadelig programvare er installert.</span><span class="sxs-lookup"><span data-stu-id="34bf2-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="34bf2-106">Enheten er **en av** disse:</span><span class="sxs-lookup"><span data-stu-id="34bf2-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="34bf2-107">Azure Active Directory (Azure AD) ble med</span><span class="sxs-lookup"><span data-stu-id="34bf2-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="34bf2-108">Hybrid Azure AD ble med</span><span class="sxs-lookup"><span data-stu-id="34bf2-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="34bf2-109">AAD registrert</span><span class="sxs-lookup"><span data-stu-id="34bf2-109">AAD registered</span></span>

- <span data-ttu-id="34bf2-110">Hvis du vil gjennomføre policyhandlinger, må du kontrollere at Microsoft Chromium Edge-nettleseren er installert på endepunktenheten.</span><span class="sxs-lookup"><span data-stu-id="34bf2-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="34bf2-111">Hvis du vil ha flere krav til distribusjon av endepunkt-DLP, kan du se Komme i gang med hindring av tap [av endepunktdata.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="34bf2-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>