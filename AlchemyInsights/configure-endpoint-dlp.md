---
title: Konfigurere endepunkt DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555554"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="59c82-102">Konfigurere endepunkt DLP</span><span class="sxs-lookup"><span data-stu-id="59c82-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="59c82-103">Microsoft Endpoint DLP lar deg utvide DLP-beskyttelse og overvåkingskapasitet til sensitiv informasjon på Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="59c82-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="59c82-104">Når enheter er innebygd i enhetsadministrasjon, kan du opprette DLP-policyer for å håndheve beskyttelseshandlinger på elementer.</span><span class="sxs-lookup"><span data-stu-id="59c82-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="59c82-105">Aktivitetsutforskeren kan brukes til å overvåke aktivitet for sensitive elementer.</span><span class="sxs-lookup"><span data-stu-id="59c82-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="59c82-106">Hvis du vil ha mer informasjon, kan du se [Innføringsenheter i enhetsbehandling](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="59c82-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="59c82-107">Slik kommer du i gang med endepunkt DLP:</span><span class="sxs-lookup"><span data-stu-id="59c82-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="59c82-108">Kontroller at du har riktig SKU/abonnementslisens.</span><span class="sxs-lookup"><span data-stu-id="59c82-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="59c82-109">Hvis du vil ha mer informasjon, kan du se [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="59c82-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="59c82-110">Kontroller tillatelsene som kreves for å aktivere enhetsbehandling, få tilgang til introduksjonssiden eller slå på/av enhetsovervåking.</span><span class="sxs-lookup"><span data-stu-id="59c82-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="59c82-111">Hvis du vil ha mer informasjon, kan du se [Tillatelser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="59c82-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="59c82-112">Innebygde enheter i enhetsbehandling ved å følge prosedyren for introduksjonsenheter.</span><span class="sxs-lookup"><span data-stu-id="59c82-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="59c82-113">Hvis du mangler alternativet Enhets introduksjon (forhåndsvisning) under **Samsvarsinnstillinger**for M365 , bekrefter du at du har den riktige lisensen og tillatelsene som det refereres til ovenfor.</span><span class="sxs-lookup"><span data-stu-id="59c82-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="59c82-114">Hvis du vil ha mer informasjon, kan du se [Onboarding-enheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="59c82-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="59c82-115">Opprett DLP-policyer for å beskytte sensitive elementer.</span><span class="sxs-lookup"><span data-stu-id="59c82-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="59c82-116">Hvis du vil ha mer informasjon, kan du se [Scenarier for Endepunkt DLP-policy](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="59c82-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="59c82-117">Hvis du vil ha mer informasjon om Microsoft Endpoint DLP, kan du se [Lære om microsoft 365 Endpoint data tap forebygging (forhåndsvisning)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="59c82-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>