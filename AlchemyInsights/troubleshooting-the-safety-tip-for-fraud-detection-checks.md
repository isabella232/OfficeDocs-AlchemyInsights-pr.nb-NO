---
title: Feilsøking i forbindelse med safety tips for svindel-gjenkjenning kontrollerer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353258"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="7558a-102">Feilsøking i forbindelse med safety tips for svindel-gjenkjenning kontrollerer</span><span class="sxs-lookup"><span data-stu-id="7558a-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="7558a-103">Hvis du får et safety tips som sier "avsender ikke kan sjekkene våre svindel-gjenkjenning, og ikke kanskje som de ser ut til å være", og deretter avsenderen kan ikke sende enten DKIM eller SPF godkjenningskontroller.</span><span class="sxs-lookup"><span data-stu-id="7558a-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="7558a-104">Det er den beste måten å løse dette problemet for avsenderen til å godkjenne seg selv.</span><span class="sxs-lookup"><span data-stu-id="7558a-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="7558a-105">Hvis avsenderen sender på dine vegne, må du godkjenne dem ved å legge avsenderens IP-adressen til din SPF-post.</span><span class="sxs-lookup"><span data-stu-id="7558a-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="7558a-106">For mer informasjon, se [Feilsøking i forbindelse med rød (mistenkelige) safety tips for svindel-gjenkjenning kontrollerer](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="7558a-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="7558a-107">Her er noen andre koblinger som kan bidra til å:</span><span class="sxs-lookup"><span data-stu-id="7558a-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="7558a-108">Hvordan Office 365 bruker sender policy framework (SPF) til å forhindre forfalskning (spoofing)</span><span class="sxs-lookup"><span data-stu-id="7558a-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="7558a-109">Sette opp SPF i Office 365 for å forhindre forfalskning (spoofing)</span><span class="sxs-lookup"><span data-stu-id="7558a-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
