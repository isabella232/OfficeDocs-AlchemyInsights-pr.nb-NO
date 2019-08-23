---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
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
ms.openlocfilehash: 3dd96a9731cfd75882dd3bb397005b19d471c882
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531368"
---
# <a name="verify-your-domain"></a><span data-ttu-id="f8110-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="f8110-102">Verify your domain</span></span>

 <span data-ttu-id="f8110-103">**Posten oppdatert sannsynligvis ikke over Internett.**</span><span class="sxs-lookup"><span data-stu-id="f8110-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="f8110-104">Det tar vanligvis bare noen minutter før vi kan se den nye oppføringen, men noen ganger kan det ta så lenge som noen timer.</span><span class="sxs-lookup"><span data-stu-id="f8110-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="f8110-105">Hvis du har ventet som allerede lenge, bør du dobbeltsjekke at du har kopiert og limt inn den nøyaktige verdien i kontrollen registreringen på DNS-verten.</span><span class="sxs-lookup"><span data-stu-id="f8110-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="f8110-106">Et vanlig problem er ikke å inkludere «MS=»-delen av oppføringen.</span><span class="sxs-lookup"><span data-stu-id="f8110-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="f8110-107">Vi trenger disse også!</span><span class="sxs-lookup"><span data-stu-id="f8110-107">We need that too!</span></span>

- <span data-ttu-id="f8110-108">Hos enkelte DNS-verter må du ta et ekstra trinn for å lagre sonefilen (der DNS-oppføringen lagres) slik at den oppdateres på Internett.</span><span class="sxs-lookup"><span data-stu-id="f8110-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="f8110-109">Kontroller at du har lagret endringene slik at Office 365 kan se og bekrefte oppføringen.</span><span class="sxs-lookup"><span data-stu-id="f8110-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
