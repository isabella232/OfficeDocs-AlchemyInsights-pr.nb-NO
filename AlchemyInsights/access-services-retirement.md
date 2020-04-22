---
title: Tilgang til pensjonering av tjenester
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687267"
---
# <a name="access-services-retirement"></a><span data-ttu-id="ae8a3-102">Tilgang til pensjonering av tjenester</span><span class="sxs-lookup"><span data-stu-id="ae8a3-102">Access services retirement</span></span>

<span data-ttu-id="ae8a3-103">Som vi opprinnelig annonserte i MC97576, i mars 2017, og fortsatte å kommunisere i løpet av det siste året Access Services blir pensjonert.</span><span class="sxs-lookup"><span data-stu-id="ae8a3-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="ae8a3-104">Den neste fasen i denne prosessen vil være fjerning av Access Web-databaser som bruker SharePoint-lister som underliggende datalagring.</span><span class="sxs-lookup"><span data-stu-id="ae8a3-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="ae8a3-105">**Hvordan påvirker dette meg?**</span><span class="sxs-lookup"><span data-stu-id="ae8a3-105">**How does this affect me?**</span></span>

<span data-ttu-id="ae8a3-106">Fra juni 2019 vil vi stoppe opprettingen av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende apper innen april 2020.</span><span class="sxs-lookup"><span data-stu-id="ae8a3-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="ae8a3-107">**Hva må jeg gjøre for å forberede meg til denne endringen?**</span><span class="sxs-lookup"><span data-stu-id="ae8a3-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="ae8a3-108">Vi oppfordrer deg til å opprette en overgangsplan for organisasjonens Access-webdatabaser.</span><span class="sxs-lookup"><span data-stu-id="ae8a3-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="ae8a3-109">Administratorer kan bruke [SharePoint Access-appskanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-appene som nettsteder bruker.</span><span class="sxs-lookup"><span data-stu-id="ae8a3-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="ae8a3-110">Du kan overføre data for Access-webdatabaser på flere måter:</span><span class="sxs-lookup"><span data-stu-id="ae8a3-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="ae8a3-111">Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="ae8a3-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="ae8a3-112">Vi anbefaler også å utforske Microsoft PowerApps som en alternativ plattform for å opprette no-code forretningsløsninger for web og mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="ae8a3-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>