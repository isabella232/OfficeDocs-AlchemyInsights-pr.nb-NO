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
ms.custom: ''
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d215f3af0cf4b46b12c8cb51a9572adb00f354e4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30766357"
---
# <a name="verify-your-domain"></a><span data-ttu-id="896a8-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="896a8-102">Verify your domain</span></span>

 <span data-ttu-id="896a8-103">**Posten oppdatert sannsynligvis ikke over Internett.**</span><span class="sxs-lookup"><span data-stu-id="896a8-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="896a8-104">Det tar vanligvis bare noen minutter før vi kan se den nye oppføringen, men noen ganger kan det ta så lenge som noen timer.</span><span class="sxs-lookup"><span data-stu-id="896a8-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="896a8-105">Hvis du har ventet som allerede lenge, bør du dobbeltsjekke at du har kopiert og limt inn den nøyaktige verdien i kontrollen registreringen på DNS-verten.</span><span class="sxs-lookup"><span data-stu-id="896a8-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="896a8-106">Et vanlig problem er ikke å inkludere «MS=»-delen av oppføringen.</span><span class="sxs-lookup"><span data-stu-id="896a8-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="896a8-107">Vi trenger disse også!</span><span class="sxs-lookup"><span data-stu-id="896a8-107">We need that too!</span></span>
    
- <span data-ttu-id="896a8-108">Hos enkelte DNS-verter må du ta et ekstra trinn for å lagre sonefilen (der DNS-oppføringen lagres) slik at den oppdateres på Internett.</span><span class="sxs-lookup"><span data-stu-id="896a8-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="896a8-109">Kontroller at du har lagret endringene slik at Office 365 kan se og bekrefte oppføringen.</span><span class="sxs-lookup"><span data-stu-id="896a8-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

