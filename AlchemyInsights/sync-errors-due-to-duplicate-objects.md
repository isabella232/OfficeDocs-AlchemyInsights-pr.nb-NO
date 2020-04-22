---
title: 902 (Synkroniser feil på grunn av dupliserte objekter)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767143"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="00759-102">Synkronisere feil på grunn av dupliserte objekter</span><span class="sxs-lookup"><span data-stu-id="00759-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="00759-103">Du kan få en av følgende feilmeldinger når katalogsynkronisering er ferdig i Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="00759-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="00759-104">Kan ikke oppdatere dette objektet i Microsoft Online Services fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede er knyttet til et annet objekt i den lokale katalogen.</span><span class="sxs-lookup"><span data-stu-id="00759-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="00759-105">Det finnes allerede et synkronisert objekt med samme proxy-adresse i Microsoft Online Services-katalogen.</span><span class="sxs-lookup"><span data-stu-id="00759-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="00759-106">Kan ikke oppdatere dette objektet fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede er knyttet til et annet objekt i de lokale katalogtjenestene: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="00759-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="00759-107">Hvis du vil identifisere og løse problemet, laster du ned og kjører [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="00759-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="00759-108">Hvis du vil ha mer informasjon, kan du se [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="00759-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
