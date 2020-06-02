---
title: Feilsøke sikkerhetstipset for kontroller for oppdagelse av svindel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504992"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="5034a-102">Feilsøke sikkerhetstipset for kontroller for oppdagelse av svindel</span><span class="sxs-lookup"><span data-stu-id="5034a-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="5034a-103">Hvis du får et sikkerhetstips som sier "Avsenderen mislyktes våre svindel deteksjon sjekker og kan ikke være den de ser ut til å være", så avsenderen ikke klarte å passere enten DKIM eller SPF godkjenning sjekker.</span><span class="sxs-lookup"><span data-stu-id="5034a-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="5034a-104">Den beste metoden for å løse dette er for avsenderen å autorisere seg selv.</span><span class="sxs-lookup"><span data-stu-id="5034a-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="5034a-105">Hvis avsenderen sender på dine vegne, må du autorisere dem ved å legge til avsenderens IP-adresse i SPF-posten din.</span><span class="sxs-lookup"><span data-stu-id="5034a-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="5034a-106">Se [Feilsøke det røde (mistenkelige) sikkerhetstipset for svindeldeteksjonskontroller](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="5034a-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="5034a-107">Her er noen andre koblinger som kan hjelpe:</span><span class="sxs-lookup"><span data-stu-id="5034a-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="5034a-108">Hvordan Microsoft bruker rammeverket for avsenderpolicy (SPF) til å hindre etterligning</span><span class="sxs-lookup"><span data-stu-id="5034a-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="5034a-109">Konfigurere SPF for å forhindre etterligning</span><span class="sxs-lookup"><span data-stu-id="5034a-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
