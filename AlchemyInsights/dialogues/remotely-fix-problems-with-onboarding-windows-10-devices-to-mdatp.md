---
title: Løse problemer eksternt med å onboarde Windows 10-enheter til Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694851"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="a8c1d-102">Løse problemer eksternt med å onboarde Windows 10-enheter til Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a8c1d-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="a8c1d-103">Hvis du har tilgang til den eksterne datamaskinen, følger du disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="a8c1d-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="a8c1d-104">Last ned [diagnoseverktøyet for Client Connectivity Analyzer.](https://go.microsoft.com/fwlink/?linkid=2143466)</span><span class="sxs-lookup"><span data-stu-id="a8c1d-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="a8c1d-105">Pakk ut og kjør MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="a8c1d-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="a8c1d-106">Finn diagnoseloggen i mappen MDATPClientAnalyzerResult, som er den samme mappen der verktøyet Analyzer ble lastet ned.</span><span class="sxs-lookup"><span data-stu-id="a8c1d-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="a8c1d-107">Se gjennom loggfilen for å finne problemer med tilkoblingen eller Proxy-innstillingene på Internett MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="a8c1d-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="a8c1d-108">Hvis du vil ha mer informasjon, [kan du se Problemer med påbordingsmaskiner.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="a8c1d-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
