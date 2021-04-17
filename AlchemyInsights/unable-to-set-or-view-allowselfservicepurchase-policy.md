---
title: Kan ikke angi eller vise AllowSelfServicePurchase-policyen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826100"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="e5d93-102">Kan ikke angi eller vise AllowSelfServicePurchase-policyen</span><span class="sxs-lookup"><span data-stu-id="e5d93-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="e5d93-103">Når du prøver å angi eller vise AllowSelfServicePurchase-policyen, får du følgende feilmelding:</span><span class="sxs-lookup"><span data-stu-id="e5d93-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="e5d93-104">*HandleError: Kan ikke hente produktpolicy med PolicyId 'AllowSelfServicePurchase', ErrorMessage – Den underliggende tilkoblingen ble lukket: Det oppstod en uventet feil under sending.*</span><span class="sxs-lookup"><span data-stu-id="e5d93-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="e5d93-105">Dette kan skyldes en eldre versjon av Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="e5d93-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="e5d93-106">Hvis du vil koble til MSCommerce-tjenesten, må du bruke TLS 1.2 eller større.</span><span class="sxs-lookup"><span data-stu-id="e5d93-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="e5d93-107">Prøv følgende trinn for å aktivere/sette TLS-protokollen til 1.2, bekrefte og prøve på nytt.</span><span class="sxs-lookup"><span data-stu-id="e5d93-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="e5d93-108">I PowerShell-ledeteksten (PS C: skriver du inn følgende kommando for å angi \) TLS-protokollen til versjon 1.2:</span><span class="sxs-lookup"><span data-stu-id="e5d93-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="e5d93-109">Bekreft TLS-protokollen(e) som er i bruk, med følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="e5d93-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="e5d93-110">Forsøk kommandoene Hent eller Oppdater etter behov.</span><span class="sxs-lookup"><span data-stu-id="e5d93-110">Retry the Get or Update commands as needed.</span></span>

