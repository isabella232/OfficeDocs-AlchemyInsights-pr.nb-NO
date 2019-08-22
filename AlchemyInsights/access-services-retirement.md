---
title: Avgang ved pensjon for Access services
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495760"
---
# <a name="access-services-retirement"></a><span data-ttu-id="27341-102">Avgang ved pensjon for Access services</span><span class="sxs-lookup"><span data-stu-id="27341-102">Access services retirement</span></span>

<span data-ttu-id="27341-103">Vi opprinnelig annonsert i MC97576, i mars 2017, og fortsatte å kommunisere over det siste året er tilgang til tjenester som Pensjonert fra Office 365.</span><span class="sxs-lookup"><span data-stu-id="27341-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="27341-104">Den neste fasen i denne prosessen blir fjerning av Access Web-databaser som bruker SharePoint-lister som deres underliggende datalageret.</span><span class="sxs-lookup"><span data-stu-id="27341-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="27341-105">**Hvordan påvirker det meg?**</span><span class="sxs-lookup"><span data-stu-id="27341-105">**How does this affect me?**</span></span>

<span data-ttu-id="27341-106">Fra juni 2019, vil vi stoppe oppretting av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende apps April 2020.</span><span class="sxs-lookup"><span data-stu-id="27341-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="27341-107">**Hva må jeg gjøre for å forberede meg for denne endringen?**</span><span class="sxs-lookup"><span data-stu-id="27341-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="27341-108">Vi oppfordrer deg til å lage en overgang plan for organisasjonens Access-databaser for web.</span><span class="sxs-lookup"><span data-stu-id="27341-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="27341-109">Administratorer kan bruke [SharePoint-Access app skanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til å få en oversikt over Access-programmer som bruker områder.</span><span class="sxs-lookup"><span data-stu-id="27341-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="27341-110">Det finnes flere måter å overføre data fra Access web databaser:</span><span class="sxs-lookup"><span data-stu-id="27341-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="27341-111">Importerer til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="27341-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="27341-112">Vi anbefaler også utforske Microsoft PowerApps som en alternativ plattform til å opprette løsninger uten kode business for web og mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="27341-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>