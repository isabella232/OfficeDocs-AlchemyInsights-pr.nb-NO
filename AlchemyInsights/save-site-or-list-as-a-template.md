---
title: Lagre område eller liste som en mal
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727540"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="30c32-102">Lagre område eller liste som en mal</span><span class="sxs-lookup"><span data-stu-id="30c32-102">Save site or list as a template</span></span>

<span data-ttu-id="30c32-103">SharePoint-nettsteds maler er forhånds bygde definisjoner som er utformet rundt et bestemt forretnings behov.</span><span class="sxs-lookup"><span data-stu-id="30c32-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="30c32-104">Hvis du vil ha mer informasjon, kan du se [bruke maler til å opprette ulike typer SharePoint-nettsteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="30c32-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="30c32-105">Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som en mal i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="30c32-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="30c32-106">**Knappen Lagre område/liste mal er ikke tilgjengelig eller mangler**.</span><span class="sxs-lookup"><span data-stu-id="30c32-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="30c32-107">Administratorer må tillate egen definert skript for å aktivere mal funksjonene.</span><span class="sxs-lookup"><span data-stu-id="30c32-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="30c32-108">For detaljerte trinn kan du se eksempler og hensyn: [tillate eller forhindre egen definerte skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="30c32-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="30c32-109">Kommandoen Lagre område som mal støttes ikke og kan føre til problemer på områder som bruker publiserings infrastrukturen for SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="30c32-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="30c32-110">**Nettsteds malen kan ikke opprettes eller fungerer ikke som den skal**</span><span class="sxs-lookup"><span data-stu-id="30c32-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="30c32-111">Det kan hende at malen mangler en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og ikke aktiveres.</span><span class="sxs-lookup"><span data-stu-id="30c32-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="30c32-112">Hvis funksjonen ikke er tilgjengelig for aktivering i gjeldende område samling, kan du ikke bruke nettsteds malen til å opprette et område.</span><span class="sxs-lookup"><span data-stu-id="30c32-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="30c32-113">Kontroller om alle lister eller biblioteker overskrider [terskel verdien for liste visnings grensen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer siden dette kan blokkere oppretting av en nettsteds mal.</span><span class="sxs-lookup"><span data-stu-id="30c32-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="30c32-114">Nettstedet bruker kanskje for mange ressurser, og derfor overskrider nettsteds malen 50 megabyte (MB)-grensen.</span><span class="sxs-lookup"><span data-stu-id="30c32-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="30c32-115">Det er problemer med å vise data fra en liste som bruker en oppslags Kol onnen.</span><span class="sxs-lookup"><span data-stu-id="30c32-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="30c32-116">Hvis du vil ha mer informasjon, kan du se [mal gener ert liste viser ikke data fra den riktige oppslags listen i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="30c32-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="30c32-117">Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du [opprette og bruke nettsteds maler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="30c32-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

