---
title: Konfigurere hindring av datatap for endepunkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657938"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="614f4-102">Konfigurere hindring av datatap for endepunkt</span><span class="sxs-lookup"><span data-stu-id="614f4-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="614f4-103">Hindring av datatap for Microsoft endepunkt gir deg mulighet for å utvide beskyttelse og overvåking av hindring av datatap for sensitiv informasjon på Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="614f4-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="614f4-104">Etter at enheter er pålastet i enhetsbehandling, kan du opprette policyer for hindring av datatap for å tvinge frem beskyttende handlinger på elementer.</span><span class="sxs-lookup"><span data-stu-id="614f4-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="614f4-105">Aktivitetsutforsker kan brukes til å overvåke aktivitet for sensitive elementer.</span><span class="sxs-lookup"><span data-stu-id="614f4-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="614f4-106">For mer informasjon, se [Pålasting av enheter i enhetsbehandling](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="614f4-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="614f4-107">For å komme i gang med hindring av datatap for endepunkt:</span><span class="sxs-lookup"><span data-stu-id="614f4-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="614f4-108">Kontroller at du har den nødvendige SKU/abonnementlisensieringen.</span><span class="sxs-lookup"><span data-stu-id="614f4-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="614f4-109">For mer informasjon, se [SKU/abonnementlisensiering](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="614f4-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="614f4-110">Kontroller tillatelsene som er nødvendige for å aktivere enhetsbehandling, få tilgang til pålastingssiden, eller aktivere/deaktivere enhetsovervåking.</span><span class="sxs-lookup"><span data-stu-id="614f4-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="614f4-111">Hvis du vil ha mer informasjon, kan du se [Tillatelser](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="614f4-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="614f4-112">Pålast enheter i enhetsbehandling ved å følge prosedyren for pålasting av enheter.</span><span class="sxs-lookup"><span data-stu-id="614f4-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="614f4-113">Hvis du vil ha mer informasjon, kan du se [Pålasting av enheter](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="614f4-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="614f4-114">Opprett policyer for hindring av datatap for å beskytte sensitive elementer.</span><span class="sxs-lookup"><span data-stu-id="614f4-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="614f4-115">For informasjon, se [Scenarier for policy for hindring av datatap for endepunkt](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="614f4-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="614f4-116">For mer informasjon om hindring av datatap for endepunkter, se [Lær om hindring av datatap for Microsoft 365-endepunkt (forhåndsversjon)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="614f4-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="614f4-117">**Viktige trinn for datainnsamling hvis du trenger støtte:**</span><span class="sxs-lookup"><span data-stu-id="614f4-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="614f4-118">Last [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="614f4-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="614f4-119">Kjør verktøyet som administrator fra cmd-vinduet:</span><span class="sxs-lookup"><span data-stu-id="614f4-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="614f4-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="614f4-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="614f4-121">Når du blir bedt om det med Angi antall minutter for å samle inn **sporinger:** angir du hvor mange minutter som kreves for å kjøre scenarioet.</span><span class="sxs-lookup"><span data-stu-id="614f4-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="614f4-122">Kjør scenarioet.</span><span class="sxs-lookup"><span data-stu-id="614f4-122">Run the scenario.</span></span>

<span data-ttu-id="614f4-123">Samle inn zip-filutdataene du vil gi til kundestøtterepresentanten.</span><span class="sxs-lookup"><span data-stu-id="614f4-123">Collect the Zip file output to give to the Support agent.</span></span>
