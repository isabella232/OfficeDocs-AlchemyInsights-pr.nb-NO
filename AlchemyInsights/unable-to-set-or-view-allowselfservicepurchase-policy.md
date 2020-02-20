---
title: Kan ikke angi eller vise policyen AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158570"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="77554-102">Kan ikke angi eller vise policyen AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="77554-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="77554-103">Når du prøver å angi eller vise policyen AllowSelfServicePurchase, får du følgende feilmelding:</span><span class="sxs-lookup"><span data-stu-id="77554-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="77554-104">*HandleError : Kan ikke hente produktpolicy med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggende tilkoblingen ble lukket: Det oppstod en uventet feil ved sending.*</span><span class="sxs-lookup"><span data-stu-id="77554-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="77554-105">Dette kan skyldes en eldre versjon av Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="77554-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="77554-106">Hvis du vil koble til MSCommerce-tjenesten, må du bruke TLS 1.2 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="77554-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="77554-107">Prøv følgende trinn for å aktivere/sette TLS-protokollen til 1.2, kontrollere og prøve på nytt.</span><span class="sxs-lookup"><span data-stu-id="77554-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="77554-108">Ved PowerShell-ledeteksten (PS\) C: skriv inn følgende kommando for å sette TLS-protokollen til versjon 1.2:</span><span class="sxs-lookup"><span data-stu-id="77554-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="77554-109">Kontroller TLS-protokollen(e) som er i bruk, med følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="77554-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="77554-110">Prøv kommandoene Hent eller Oppdater på nytt etter behov.</span><span class="sxs-lookup"><span data-stu-id="77554-110">Retry the Get or Update commands as needed.</span></span>

