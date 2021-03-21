---
title: Problemer med å innlemme maskiner i Microsoft Defender for endepunkter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901576"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="82c9a-102">Problemer med å innlemme maskiner i Microsoft Defender for endepunkter</span><span class="sxs-lookup"><span data-stu-id="82c9a-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="82c9a-103">Du kan ha problemer med å innlemme maskiner i MDE-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="82c9a-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="82c9a-104">Hvis du har tilgang til sluttbruker-maskinen, følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="82c9a-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="82c9a-105">Last ned den siste forhåndsversjonen av diagnoseverktøyet [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="82c9a-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="82c9a-106">Høyreklikk **MDEClientAnalyzer.cmd** og velg “Kjør som administrator”.</span><span class="sxs-lookup"><span data-stu-id="82c9a-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="82c9a-107">Følg veiledningen som blir foreslått i **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="82c9a-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="82c9a-108">For mer fyldige logger, se gjennom undermappen som ble opprettet med navn **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="82c9a-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="82c9a-109">Hvis du trenger ytterligere veiledning, kan du kontakte [kundestøtte for Microsoft Defender for endepunkt](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) og stille til rådighet filen MDEClientAnalyzerResult.zip for analyse.</span><span class="sxs-lookup"><span data-stu-id="82c9a-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
