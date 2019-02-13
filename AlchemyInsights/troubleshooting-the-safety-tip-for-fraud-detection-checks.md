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
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29936369"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="98871-102">Feilsøking i forbindelse med safety tips for svindel-gjenkjenning kontrollerer</span><span class="sxs-lookup"><span data-stu-id="98871-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="98871-p101">Hvis du får et safety tips som sier "avsender ikke kan sjekkene våre svindel-gjenkjenning, og ikke kanskje som de ser ut til å være", og deretter avsenderen kan ikke sende enten DKIM eller SPF godkjenningskontroller. Det er den beste måten å løse dette problemet for avsenderen til å godkjenne seg selv. Hvis avsenderen sender på dine vegne, må du godkjenne dem ved å legge avsenderens IP-adressen til din SPF-post.</span><span class="sxs-lookup"><span data-stu-id="98871-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="98871-106">For mer informasjon, se [Feilsøking i forbindelse med rød (mistenkelige) safety tips for svindel-gjenkjenning kontrollerer](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="98871-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="98871-107">Her er noen andre koblinger som kan bidra til å:</span><span class="sxs-lookup"><span data-stu-id="98871-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="98871-108">Hvordan Office 365 bruker sender policy framework (SPF) til å forhindre forfalskning (spoofing)</span><span class="sxs-lookup"><span data-stu-id="98871-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="98871-109">Sette opp SPF i Office 365 for å hindre forfalskning</span><span class="sxs-lookup"><span data-stu-id="98871-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

