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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402442"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="42256-102">Konfigurere hindring av datatap for endepunkt</span><span class="sxs-lookup"><span data-stu-id="42256-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="42256-103">Hindring av datatap for Microsoft endepunkt gir deg mulighet for å utvide beskyttelse og overvåking av hindring av datatap for sensitiv informasjon på Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="42256-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="42256-104">Etter at enheter er pålastet i enhetsbehandling, kan du opprette policyer for hindring av datatap for å tvinge frem beskyttende handlinger på elementer.</span><span class="sxs-lookup"><span data-stu-id="42256-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="42256-105">Aktivitetsutforsker kan brukes til å overvåke aktivitet for sensitive elementer.</span><span class="sxs-lookup"><span data-stu-id="42256-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="42256-106">For mer informasjon, se [Pålasting av enheter i enhetsbehandling](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="42256-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="42256-107">For å komme i gang med hindring av datatap for endepunkt:</span><span class="sxs-lookup"><span data-stu-id="42256-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="42256-108">Kontroller at du har den nødvendige SKU/abonnementlisensieringen.</span><span class="sxs-lookup"><span data-stu-id="42256-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="42256-109">For mer informasjon, se [SKU/abonnementlisensiering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="42256-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="42256-110">Kontroller tillatelsene som er nødvendige for å aktivere enhetsbehandling, få tilgang til pålastingssiden, eller aktivere/deaktivere enhetsovervåking.</span><span class="sxs-lookup"><span data-stu-id="42256-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="42256-111">Hvis du vil ha mer informasjon, kan du se [Tillatelser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="42256-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="42256-112">Pålast enheter i enhetsbehandling ved å følge prosedyren for pålasting av enheter.</span><span class="sxs-lookup"><span data-stu-id="42256-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="42256-113">Hvis du mangler alternativet pålasting av enheter (forhåndsversjon) under **Innstillinger** for M365-samsvar, bekreft at du har den nødvendige lisensen og tillatelser som referert over.</span><span class="sxs-lookup"><span data-stu-id="42256-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="42256-114">Hvis du vil ha mer informasjon, kan du se [Pålasting av enheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="42256-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="42256-115">Opprett policyer for hindring av datatap for å beskytte sensitive elementer.</span><span class="sxs-lookup"><span data-stu-id="42256-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="42256-116">For informasjon, se [Scenarier for policy for hindring av datatap for endepunkt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="42256-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="42256-117">For mer informasjon om hindring av datatap for endepunkter, se [Lær om hindring av datatap for Microsoft 365-endepunkt (forhåndsversjon)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="42256-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="42256-118">**Viktige trinn for datainnsamling hvis du trenger støtte:**</span><span class="sxs-lookup"><span data-stu-id="42256-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="42256-119">Last ned forhåndsversjon av MDATP Client Analyzer fra [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="42256-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="42256-120">Kjør verktøyet som administrator fra cmd-vinduet:</span><span class="sxs-lookup"><span data-stu-id="42256-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="42256-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="42256-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="42256-122">Når du blir bedt om “Skriv inn antall minutter for innsamling av spor: “, skriv inn antall minutter som trengs for å kjøre scenariet</span><span class="sxs-lookup"><span data-stu-id="42256-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="42256-123">Kjør scenariet</span><span class="sxs-lookup"><span data-stu-id="42256-123">Run the scenario</span></span>

<span data-ttu-id="42256-124">Samle inn Zip-fil-utdata som skal gis til kundestøtterepresentanten.</span><span class="sxs-lookup"><span data-stu-id="42256-124">Collect the Zip file output to be given to the Support agent.</span></span>
