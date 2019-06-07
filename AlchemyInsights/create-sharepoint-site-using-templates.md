---
title: Opprette et område i SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753716"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="3e954-102">Opprette SharePoint-områder ved hjelp av maler</span><span class="sxs-lookup"><span data-stu-id="3e954-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="3e954-103">SharePoint-områdemaler er forhåndsbygde definisjoner utviklet rundt bestemte forretningsbehov.</span><span class="sxs-lookup"><span data-stu-id="3e954-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="3e954-104">Hvis du vil ha mer informasjon, se [bruke maler for å opprette ulike typer SharePoint-områder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="3e954-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="3e954-105">Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som mal i Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="3e954-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="3e954-106">**Lagre område-listen mal-knappen er ikke tilgjengelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="3e954-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="3e954-107">Administratorer må tillate egendefinert skript til å aktivere funksjonene for malen.</span><span class="sxs-lookup"><span data-stu-id="3e954-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="3e954-108">Detaljert fremgangsmåte, eksempler og vurderinger i</span><span class="sxs-lookup"><span data-stu-id="3e954-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="3e954-109">Tillate eller forhindre egendefinert skript</span><span class="sxs-lookup"><span data-stu-id="3e954-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="3e954-110">Området lagre som mal-kommandoen støttes ikke og kan forårsake problemer på områder som bruker SharePoint Server-publisering infrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="3e954-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="3e954-111">Områdemalen kan ikke opprettes eller fungerer ikke riktig.</span><span class="sxs-lookup"><span data-stu-id="3e954-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="3e954-112">Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , og vil ikke aktivere.</span><span class="sxs-lookup"><span data-stu-id="3e954-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="3e954-113">Hvis funksjonen ikke er tilgjengelig for å aktivere i gjeldende områdesamling, kan du ikke bruke malen webområde til å opprette et område.</span><span class="sxs-lookup"><span data-stu-id="3e954-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="3e954-114">Kontroller Hvis eventuelle lister eller biblioteker overskrider [Terskelen for listevisning grensen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) av 5000 varer dette kan hindre opprettelsen av en områdemal.</span><span class="sxs-lookup"><span data-stu-id="3e954-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="3e954-115">Området som bruker for mange ressurser, og derfor områdemalen overskrider grensen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="3e954-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="3e954-116">Det er problemer med å vise data fra en liste som bruker en oppslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="3e954-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="3e954-117">Hvis du vil ha mer informasjon, kan du se [mal-genererte listen ikke viser dataene fra den riktige oppslagslisten i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="3e954-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="3e954-118">For mer detaljert informasjon om vanlige problemer og løsninger, se [opprette og bruke maler for webområder](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="3e954-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



