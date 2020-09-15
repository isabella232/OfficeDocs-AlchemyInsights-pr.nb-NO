---
title: Pensjon for tilgangs tjenester
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698691"
---
# <a name="access-services-retirement"></a><span data-ttu-id="a70ad-102">Pensjon for tilgangs tjenester</span><span class="sxs-lookup"><span data-stu-id="a70ad-102">Access services retirement</span></span>

<span data-ttu-id="a70ad-103">Som det opprinnelig ble kunngjort i MC97576, i mars 2017, og fortsetter å kommunisere over det siste året Access Services blir trukket tilbake.</span><span class="sxs-lookup"><span data-stu-id="a70ad-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="a70ad-104">Den neste fasen i denne prosessen vil være fjerning av Access-webdatabaser som bruker SharePoint-lister som underliggende data lagring.</span><span class="sxs-lookup"><span data-stu-id="a70ad-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="a70ad-105">**Hvordan påvirker dette meg?**</span><span class="sxs-lookup"><span data-stu-id="a70ad-105">**How does this affect me?**</span></span>

<span data-ttu-id="a70ad-106">Fra og med juni 2019 vil vi stoppe opprettelsen av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende apper etter april 2020.</span><span class="sxs-lookup"><span data-stu-id="a70ad-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="a70ad-107">**Hva må jeg gjøre for å klargjøre for denne endringen?**</span><span class="sxs-lookup"><span data-stu-id="a70ad-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="a70ad-108">Vi oppfordrer deg til å opprette en overgangs plan for organisasjonens web databaser for tilgang.</span><span class="sxs-lookup"><span data-stu-id="a70ad-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="a70ad-109">Administratorer kan bruke [SharePoint Access app-skanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-appene som nett steder bruker.</span><span class="sxs-lookup"><span data-stu-id="a70ad-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="a70ad-110">Det finnes flere måter å overføre data i Access Web databaser på:</span><span class="sxs-lookup"><span data-stu-id="a70ad-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="a70ad-111">Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="a70ad-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="a70ad-112">Vi anbefaler også å utforske Microsoft PowerApps som en alternativ plattform for å opprette gratis bedrifts løsninger for nett og mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="a70ad-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>