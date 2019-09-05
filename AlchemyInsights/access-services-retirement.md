---
title: Avgang av tilgang til tjenester
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747793"
---
# <a name="access-services-retirement"></a><span data-ttu-id="d9a25-102">Avgang av tilgang til tjenester</span><span class="sxs-lookup"><span data-stu-id="d9a25-102">Access services retirement</span></span>

<span data-ttu-id="d9a25-103">Som vi opprinnelig annonsert i MC97576, i mars 2017, og fortsatte å kommunisere det siste året Access Services blir pensjonert fra Office 365.</span><span class="sxs-lookup"><span data-stu-id="d9a25-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="d9a25-104">Den neste fasen i denne prosessen vil være fjerning av Access Web databaser som bruker SharePoint-lister som underliggende datalagring.</span><span class="sxs-lookup"><span data-stu-id="d9a25-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="d9a25-105">**Hvordan påvirker dette meg?**</span><span class="sxs-lookup"><span data-stu-id="d9a25-105">**How does this affect me?**</span></span>

<span data-ttu-id="d9a25-106">Starter juni 2019, vil vi stoppe opprettelsen av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende programmer innen april 2020.</span><span class="sxs-lookup"><span data-stu-id="d9a25-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="d9a25-107">**Hva må jeg gjøre for å forberede meg på denne endringen?**</span><span class="sxs-lookup"><span data-stu-id="d9a25-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="d9a25-108">Vi oppfordrer deg til å opprette en overgangsplan for organisasjonens Access Web databaser.</span><span class="sxs-lookup"><span data-stu-id="d9a25-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="d9a25-109">Administratorer kan bruke [program skanneren for SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-appene som områdene bruker.</span><span class="sxs-lookup"><span data-stu-id="d9a25-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="d9a25-110">Det er flere måter å overføre Access Web databaser data:</span><span class="sxs-lookup"><span data-stu-id="d9a25-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="d9a25-111">Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="d9a25-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="d9a25-112">Vi anbefaler også at du utforsker Microsoft PowerApps som en alternativ plattform for å opprette forretningsløsninger uten kode for nett-og mobilenheter.</span><span class="sxs-lookup"><span data-stu-id="d9a25-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>