---
title: Kan ikke angi eller vise AllowSelfServicePurchase-policyen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735208"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="8c3af-102">Kan ikke angi eller vise AllowSelfServicePurchase-policyen</span><span class="sxs-lookup"><span data-stu-id="8c3af-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="8c3af-103">Når du prøver å angi eller vise AllowSelfServicePurchase-policyen, får du følgende feil melding:</span><span class="sxs-lookup"><span data-stu-id="8c3af-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="8c3af-104">*HandleError: kan ikke hente produkt policy med PolicyId ' AllowSelfServicePurchase ', ErrorMessage-den underliggende tilkoblingen ble lukket: Det oppstod en uventet feil under sendingen.*</span><span class="sxs-lookup"><span data-stu-id="8c3af-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="8c3af-105">Dette kan skyldes en eldre versjon av TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="8c3af-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="8c3af-106">Hvis du vil koble til MSCommerce-tjenesten, må du bruke TLS 1,2 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="8c3af-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="8c3af-107">Prøv følgende trinn for å aktivere/sette TLS-protokollen til 1,2, bekrefte og prøve på nytt.</span><span class="sxs-lookup"><span data-stu-id="8c3af-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="8c3af-108">I PowerShell-ledeteksten (PS C: \) Angi følgende kommando for å angi TLS-protokollen til versjon 1,2:</span><span class="sxs-lookup"><span data-stu-id="8c3af-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="8c3af-109">Kontroller hvilken TLS-protokoll som er i bruk, med følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="8c3af-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="8c3af-110">Prøv kommandoene Hent eller oppdater på nytt etter behov.</span><span class="sxs-lookup"><span data-stu-id="8c3af-110">Retry the Get or Update commands as needed.</span></span>

