---
title: Feilsøke sikkerhetstipset for gjenkjenning av svindelkontroller
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834740"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="e8fa8-102">Feilsøke sikkerhetstipset for gjenkjenning av svindelkontroller</span><span class="sxs-lookup"><span data-stu-id="e8fa8-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="e8fa8-103">Hvis du får et sikkerhetstips som sier «Avsenderen mislyktes med å oppdage svindel og kanskje ikke er den de ser ut til å være», kan avsenderen ikke sende enten DKIM- eller SPF-godkjenningskontroller.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="e8fa8-104">Den beste metoden for å løse dette er at avsenderen kan godkjenne seg selv.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="e8fa8-105">Hvis avsenderen sender på dine vegne, må du godkjenne dem ved å legge til avsenderens IP-adresse i SPF-posten.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="e8fa8-106">Se [Feilsøke det røde (mistenkelige) sikkerhetstipset for](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) gjenkjenning av svindel for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="e8fa8-107">Her er noen andre koblinger som kan hjelpe deg:</span><span class="sxs-lookup"><span data-stu-id="e8fa8-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="e8fa8-108">Slik bruker Microsoft rammeverket for avsenderpolicy (SPF) til å forhindre forfalsling</span><span class="sxs-lookup"><span data-stu-id="e8fa8-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="e8fa8-109">Konfigurere SPF for å forhindre forfalsling</span><span class="sxs-lookup"><span data-stu-id="e8fa8-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
