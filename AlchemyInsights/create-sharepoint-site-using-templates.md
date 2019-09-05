---
title: Opprette et område i SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755317"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="c6321-102">Opprette SharePoint-områder ved hjelp av maler</span><span class="sxs-lookup"><span data-stu-id="c6321-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="c6321-103">Maler for SharePoint-områder er forhåndsbygde definisjoner som er utformet rundt et bestemt forretningsbehov.</span><span class="sxs-lookup"><span data-stu-id="c6321-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="c6321-104">Hvis du vil ha mer informasjon, se [bruke maler til å opprette ulike typer SharePoint-områder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="c6321-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="c6321-105">Her er noen vanlige problemer/løsninger i forbindelse med lagring av et område eller en liste som en mal i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c6321-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="c6321-106">**Knappen Lagre område/liste mal er ikke tilgjengelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="c6321-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="c6321-107">Administratorer må tillate egendefinert skript for å aktivere mal funksjonene.</span><span class="sxs-lookup"><span data-stu-id="c6321-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c6321-108">For detaljerte trinn, eksempler og betraktninger se</span><span class="sxs-lookup"><span data-stu-id="c6321-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="c6321-109">Tillate eller forhindre egendefinert skript</span><span class="sxs-lookup"><span data-stu-id="c6321-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="c6321-110">Kommandoen Lagre område som mal støttes ikke, og kan forårsake problemer på områder som bruker infrastruktur for SharePoint Server-publisering.</span><span class="sxs-lookup"><span data-stu-id="c6321-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="c6321-111">**Områdemalen kan ikke opprettes eller fungerer ikke som den skal**</span><span class="sxs-lookup"><span data-stu-id="c6321-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="c6321-112">Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og vil ikke aktivere.</span><span class="sxs-lookup"><span data-stu-id="c6321-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="c6321-113">Hvis funksjonen ikke er tilgjengelig for aktivering i gjeldende områdesamling, kan du ikke bruke områdemalen til å opprette et område.</span><span class="sxs-lookup"><span data-stu-id="c6321-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="c6321-114">Kontroller om noen lister eller biblioteker overskrider [terskelen for liste visningsgrense](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000 elementer, da dette kan blokkere oppretting av en områdemal.</span><span class="sxs-lookup"><span data-stu-id="c6321-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="c6321-115">Området bruker kanskje for mange ressurser, og derfor overskrider områdemalen grensen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="c6321-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="c6321-116">Det er problemer med å vise data fra en liste som bruker en oppslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="c6321-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c6321-117">Hvis du vil ha mer informasjon, kan [du se mal-generert liste viser ikke data fra den riktige oppslagslisten i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="c6321-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="c6321-118">Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du se [opprette og bruke områdemaler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="c6321-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



