---
title: Lagre området eller listen som en mal
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551640"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="09dae-102">Lagre området eller listen som en mal</span><span class="sxs-lookup"><span data-stu-id="09dae-102">Save site or list as a template</span></span>

<span data-ttu-id="09dae-103">SharePoint-områdemaler er forhåndsbygde definisjoner utviklet rundt bestemte forretningsbehov.</span><span class="sxs-lookup"><span data-stu-id="09dae-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="09dae-104">Hvis du vil ha mer informasjon, se [bruke maler for å opprette ulike typer SharePoint-områder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="09dae-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="09dae-105">Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som mal i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="09dae-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="09dae-106">**Lagre område-listen mal-knappen er ikke tilgjengelig eller mangler**.</span><span class="sxs-lookup"><span data-stu-id="09dae-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="09dae-107">Administratorer må tillate egendefinert skript til å aktivere funksjonene for malen.</span><span class="sxs-lookup"><span data-stu-id="09dae-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="09dae-108">For en detaljert fremgangsmåte, eksempler og vurderinger for å se [Tillat eller forby egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="09dae-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="09dae-109">Området lagre som mal-kommandoen støttes ikke og kan forårsake problemer på områder som bruker SharePoint Server-publisering infrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="09dae-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="09dae-110">**Områdemalen kan ikke opprettes eller fungerer ikke riktig**</span><span class="sxs-lookup"><span data-stu-id="09dae-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="09dae-111">Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , og vil ikke aktivere.</span><span class="sxs-lookup"><span data-stu-id="09dae-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="09dae-112">Hvis funksjonen ikke er tilgjengelig for å aktivere i gjeldende områdesamling, kan du ikke bruke malen webområde til å opprette et område.</span><span class="sxs-lookup"><span data-stu-id="09dae-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="09dae-113">Kontroller Hvis eventuelle lister eller biblioteker overskrider [Terskelen for listevisning grensen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) av 5000 varer dette kan hindre opprettelsen av en områdemal.</span><span class="sxs-lookup"><span data-stu-id="09dae-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="09dae-114">Området som bruker for mange ressurser, og derfor områdemalen overskrider grensen på 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="09dae-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="09dae-115">Det er problemer med å vise data fra en liste som bruker en oppslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="09dae-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="09dae-116">Hvis du vil ha mer informasjon, kan du se [mal-genererte listen ikke viser dataene fra den riktige oppslagslisten i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="09dae-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="09dae-117">Vennligst referanse, [opprette og bruke maler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)for mer detaljert informasjon om vanlige problemer og løsninger.</span><span class="sxs-lookup"><span data-stu-id="09dae-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

