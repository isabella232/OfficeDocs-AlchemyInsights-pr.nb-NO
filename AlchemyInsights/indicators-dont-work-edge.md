---
title: Indikatorer fungerer ikke ved hjelp av Edge-nettleseren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676461"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="ca52d-102">Indikatorer fungerer ikke ved hjelp av Edge-nettleseren</span><span class="sxs-lookup"><span data-stu-id="ca52d-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="ca52d-103">Når du har opprettet en indikator, innfris den ikke av Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="ca52d-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="ca52d-104">Hvis du vil ha mer informasjon, kan du se Opprette [indikatorer for NETTADRESSER og nettadresser/domener.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="ca52d-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="ca52d-105">Trinn 1: Sikre følgende</span><span class="sxs-lookup"><span data-stu-id="ca52d-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="ca52d-106">Kontroller at indikatoren er riktig (ingen skrivefeil i IP/URL, riktig handling, de riktige RBAC-gruppene).</span><span class="sxs-lookup"><span data-stu-id="ca52d-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="ca52d-107">Vent minst 2 timer etter at du har opprettet indikatoren for å ta hensyn til eventuell ventetid.</span><span class="sxs-lookup"><span data-stu-id="ca52d-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="ca52d-108">Bekreft at systemet(e) er installert på Microsoft Defender for endepunkt.</span><span class="sxs-lookup"><span data-stu-id="ca52d-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="ca52d-109">Kontroller at systemet(e) kan kommunisere med skyen.</span><span class="sxs-lookup"><span data-stu-id="ca52d-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="ca52d-110">Kontroller at Smartscreen er aktivert og tilgjengelig ved å gå til [testnettstedet](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="ca52d-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="ca52d-111">Trinn 2: Feilsøke det potensielle problemet</span><span class="sxs-lookup"><span data-stu-id="ca52d-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="ca52d-112">Kontroller at klienten oppfyller kravene.</span><span class="sxs-lookup"><span data-stu-id="ca52d-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="ca52d-113">Hvis du vil ha mer informasjon, kan du se Opprette [indikatorer for NETTADRESSER og nettadresser/domener](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="ca52d-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="ca52d-114">Kontroller at du kjører den nyeste versjonen av Edge-nettleseren.</span><span class="sxs-lookup"><span data-stu-id="ca52d-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="ca52d-115">Hvis du vil finne ut den nyeste versjonen, kan du se Finne ut hvilken [versjon av Microsoft Edge du har](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="ca52d-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="ca52d-116">Start Edge-nettleseren på nytt.</span><span class="sxs-lookup"><span data-stu-id="ca52d-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="ca52d-117">Gå til nettstedet der du har satt opp en indikator.</span><span class="sxs-lookup"><span data-stu-id="ca52d-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="ca52d-118">Hvis nettstedet ikke vises som forventet, fortsetter du til trinn 3.</span><span class="sxs-lookup"><span data-stu-id="ca52d-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="ca52d-119">Trinn 3: Samle inn data</span><span class="sxs-lookup"><span data-stu-id="ca52d-119">Step 3: Collect data</span></span>

- <span data-ttu-id="ca52d-120">Samle **inn MDEClientAnalyzer-diagnosedata.**</span><span class="sxs-lookup"><span data-stu-id="ca52d-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="ca52d-121">Hvis du vil ha instruksjoner, kan du se Problemer [med introduksjonsmaskiner til Microsoft Defender for endepunkt](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="ca52d-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="ca52d-122">Hvis du er komfortabel med å installere og samle en Fiddler-sporing, kan du se [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="ca52d-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="ca52d-123">Hvis du foretrekker veiledning fra Microsoft Kundestøtte, velger du Støtte-ikonet nedenfor for å åpne en støttesak.</span><span class="sxs-lookup"><span data-stu-id="ca52d-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
