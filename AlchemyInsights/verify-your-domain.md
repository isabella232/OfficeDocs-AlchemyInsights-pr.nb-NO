---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710452"
---
# <a name="verify-your-domain"></a><span data-ttu-id="6bfbb-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="6bfbb-102">Verify your domain</span></span>

 <span data-ttu-id="6bfbb-103">**Posten har sannsynligvis ikke oppdatert på Internett.**</span><span class="sxs-lookup"><span data-stu-id="6bfbb-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="6bfbb-104">Det tar vanligvis bare noen minutter før vi kan se den nye oppføringen, men noen ganger kan det ta så lenge som noen timer.</span><span class="sxs-lookup"><span data-stu-id="6bfbb-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="6bfbb-105">Hvis du har ventet så lenge allerede, dobbeltsjekk at du har kopiert og limt inn den nøyaktige verdien i TXT-bekreftelsesposten hos DNS-verten.</span><span class="sxs-lookup"><span data-stu-id="6bfbb-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="6bfbb-106">Et vanlig problem er ikke å inkludere «MS=»-delen av oppføringen.</span><span class="sxs-lookup"><span data-stu-id="6bfbb-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="6bfbb-107">Vi trenger disse også!</span><span class="sxs-lookup"><span data-stu-id="6bfbb-107">We need that too!</span></span>

- <span data-ttu-id="6bfbb-108">Hos enkelte DNS-verter må du ta et ekstra trinn for å lagre sonefilen (der DNS-oppføringen lagres) slik at den oppdateres på Internett.</span><span class="sxs-lookup"><span data-stu-id="6bfbb-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="6bfbb-109">Kontroller at du har lagret endringene, slik at Microsoft kan se og bekrefte oppføringen.</span><span class="sxs-lookup"><span data-stu-id="6bfbb-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
