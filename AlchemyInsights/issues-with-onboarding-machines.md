---
title: Problemer med introduksjonsmaskiner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141655"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="5cc38-102">Problemer med introduksjonsmaskiner</span><span class="sxs-lookup"><span data-stu-id="5cc38-102">Issues with onboarding machines</span></span>

<span data-ttu-id="5cc38-103">Du kan ha problemer med introduksjonsmaskiner til MDATP-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="5cc38-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="5cc38-104">Hvis du har tilgang til sluttbrukermaskinen, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="5cc38-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="5cc38-105">Last ned diagnoseverktøyet [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="5cc38-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="5cc38-106">Pakk ut og kjør MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="5cc38-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="5cc38-107">Finn diagnoseloggen i mappen MDATPClientAnalyzerResult, den samme mappen der Analyzer-verktøyet lastes ned.</span><span class="sxs-lookup"><span data-stu-id="5cc38-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="5cc38-108">Se gjennom loggfilen, MDATPClientAnalyzer.txt, for å finne problemer med tilkoblings- eller Internett-proxy-innstillinger.</span><span class="sxs-lookup"><span data-stu-id="5cc38-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>