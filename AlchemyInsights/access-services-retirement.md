---
title: Avgang ved pensjon for Access services
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973936"
---
# <a name="access-services-retirement"></a><span data-ttu-id="4ec49-102">Avgang ved pensjon for Access services</span><span class="sxs-lookup"><span data-stu-id="4ec49-102">Access services retirement</span></span>

<span data-ttu-id="4ec49-103">Vi opprinnelig annonsert i MC97576, i mars 2017, og fortsatte å kommunisere over det siste året er tilgang til tjenester som Pensjonert fra Office 365.</span><span class="sxs-lookup"><span data-stu-id="4ec49-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="4ec49-104">Den neste fasen i denne prosessen blir fjerning av Access Web-databaser som bruker SharePoint-lister som deres underliggende datalageret.</span><span class="sxs-lookup"><span data-stu-id="4ec49-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="4ec49-105">Hvordan påvirker det meg?</span><span class="sxs-lookup"><span data-stu-id="4ec49-105">How does this affect me?</span></span>

<span data-ttu-id="4ec49-106">Fra juni 2019, vil vi stoppe oppretting av nye Access-databaser i SharePoint Online og avslutte tjenesten og eventuelle gjenværende apps April 2020.</span><span class="sxs-lookup"><span data-stu-id="4ec49-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="4ec49-107">Hva må jeg gjøre for å forberede meg for denne endringen?</span><span class="sxs-lookup"><span data-stu-id="4ec49-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="4ec49-108">Vi oppfordrer deg til å lage en overgang plan for organisasjonens Access-databaser for web.</span><span class="sxs-lookup"><span data-stu-id="4ec49-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="4ec49-109">Administratorer kan bruke [SharePoint-Access app skanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) til å få en oversikt over Access-programmer som bruker områder.</span><span class="sxs-lookup"><span data-stu-id="4ec49-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="4ec49-110">Det finnes flere måter å overføre data fra Access web databaser:</span><span class="sxs-lookup"><span data-stu-id="4ec49-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="4ec49-111">Importerer til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="4ec49-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="4ec49-112">Vi anbefaler også utforske Microsoft PowerApps som en alternativ plattform til å opprette løsninger uten kode business for web og mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="4ec49-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>