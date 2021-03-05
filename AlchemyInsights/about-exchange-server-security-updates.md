---
title: Sikkerhetsoppdateringer for Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481949"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="264e9-102">Sikkerhetsoppdateringer for Exchange Server</span><span class="sxs-lookup"><span data-stu-id="264e9-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="264e9-103">Microsoft har utgitt en serie med kritiske sikkerhetsoppdateringer for Exchange Server lokalt.</span><span class="sxs-lookup"><span data-stu-id="264e9-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="264e9-104">De berørte serverversjonene er alle oppdateringsnivåer for Exchange Server 2010, 2013, 2016 og 2019.</span><span class="sxs-lookup"><span data-stu-id="264e9-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="264e9-105">Exchange Online påvirkes IKKE, men hvis du har noen lokale Exchange-servere på grunn av hybridkonfigurasjon, er de potensielt sårbare.</span><span class="sxs-lookup"><span data-stu-id="264e9-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="264e9-106">Hvis du vil oppdatere de lokale serverne, må du kjøre minst følgende versjoner av Exchange:</span><span class="sxs-lookup"><span data-stu-id="264e9-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="264e9-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="264e9-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="264e9-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="264e9-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="264e9-109">Exchange Server 2016 CU 19 eller CU 18</span><span class="sxs-lookup"><span data-stu-id="264e9-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="264e9-110">Exchange Server 2019 CU 8 eller CU 7</span><span class="sxs-lookup"><span data-stu-id="264e9-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="264e9-111">Se følgende kunngjøring om plasseringen av løsninger: [Utgitt: Sikkerhetsoppdateringer for Exchange Server 2021 mars 2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="264e9-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="264e9-112">**Viktige merknader:**</span><span class="sxs-lookup"><span data-stu-id="264e9-112">**Important notes:**</span></span>

<span data-ttu-id="264e9-113">Installasjon av oppdateringer vil ikke fungere hvis de lokale serverne ikke kjører nødvendige Exchange-versjoner, i henhold til listen ovenfor.</span><span class="sxs-lookup"><span data-stu-id="264e9-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="264e9-114">Hvis du installerer oppdateringer manuelt, kan du lese delen «Kjente problemer» i oppdatering av KB-artikler for viktig informasjon.</span><span class="sxs-lookup"><span data-stu-id="264e9-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="264e9-115">Sikkerhetsoppdateringer MÅ kjøres fra hevet CMD/PowerShell-ledetekst!</span><span class="sxs-lookup"><span data-stu-id="264e9-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
