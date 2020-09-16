---
title: 902 (synkroniserings feil på grunn av dupliserte objekter)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737350"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="7370e-102">Synkroniserings feil på grunn av dupliserte objekter</span><span class="sxs-lookup"><span data-stu-id="7370e-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="7370e-103">Du kan få en av følgende feil meldinger når katalog synkronisering er fullført i Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="7370e-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="7370e-104">Kan ikke oppdatere dette objektet i Microsoft Online Services fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede kan være knyttet til et annet objekt i den lokale katalogen.</span><span class="sxs-lookup"><span data-stu-id="7370e-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="7370e-105">Det finnes allerede et synkronisert objekt med samme proxy-adresse i Microsoft Online Services-katalogen.</span><span class="sxs-lookup"><span data-stu-id="7370e-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="7370e-106">Kan ikke oppdatere dette objektet fordi følgende attributter som er knyttet til dette objektet, har verdier som allerede kan være knyttet til et annet objekt i den lokale katalog tjenesten: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7370e-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="7370e-107">Hvis du vil identifisere og løse problemet, kan du laste ned og kjøre [verktøyet for utbedring av IdFix DirSync-feil](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="7370e-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="7370e-108">Hvis du vil ha mer informasjon, kan du se [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="7370e-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
