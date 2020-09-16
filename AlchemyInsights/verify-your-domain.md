---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734315"
---
# <a name="verify-your-domain"></a><span data-ttu-id="e05de-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="e05de-102">Verify your domain</span></span>

 <span data-ttu-id="e05de-103">**Posten er sannsynligvis ikke oppdatert på Internet t.**</span><span class="sxs-lookup"><span data-stu-id="e05de-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="e05de-104">Det tar vanligvis bare noen minutter før vi kan se den nye oppføringen, men noen ganger kan det ta så lenge som noen timer.</span><span class="sxs-lookup"><span data-stu-id="e05de-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="e05de-105">Hvis du har ventet at lenge allerede, må du dobbeltsjekke at du har kopiert og limt inn den nøyaktige verdien i oppføringen for TXT-bekreftelsen hos DNS-verten.</span><span class="sxs-lookup"><span data-stu-id="e05de-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="e05de-106">Et vanlig problem er ikke å inkludere «MS=»-delen av oppføringen.</span><span class="sxs-lookup"><span data-stu-id="e05de-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="e05de-107">Vi trenger disse også!</span><span class="sxs-lookup"><span data-stu-id="e05de-107">We need that too!</span></span>

- <span data-ttu-id="e05de-108">Hos enkelte DNS-verter må du ta et ekstra trinn for å lagre sonefilen (der DNS-oppføringen lagres) slik at den oppdateres på Internett.</span><span class="sxs-lookup"><span data-stu-id="e05de-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="e05de-109">Kontroller at du har lagret endringene slik at Microsoft kan se og bekrefte posten.</span><span class="sxs-lookup"><span data-stu-id="e05de-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
