---
title: Opprette et område i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770432"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="5461f-102">Opprette SharePoint-områder ved hjelp av maler</span><span class="sxs-lookup"><span data-stu-id="5461f-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="5461f-103">Muligheten til å lagre et nettsted som en mal støttes ikke med moderne kommunikasjons- eller gruppeområder.</span><span class="sxs-lookup"><span data-stu-id="5461f-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="5461f-104">Hvis du vil ha mer informasjon om hvordan du bruker maler, kan du se [Lagre, laste ned og laste opp et SharePoint-område som en mal](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="5461f-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="5461f-105">Her er noen vanlige problemer/løsninger for lagring av et område eller en liste som en mal i Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="5461f-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="5461f-106">**Lagre område-/listemal-knappen er ikke tilgjengelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="5461f-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="5461f-107">Administratorer må tillate egendefinert skript for å aktivere malfunksjonene.</span><span class="sxs-lookup"><span data-stu-id="5461f-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="5461f-108">For detaljerte trinn, eksempler og vurderinger, se</span><span class="sxs-lookup"><span data-stu-id="5461f-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="5461f-109">Tillat eller forhindre egendefinert skript</span><span class="sxs-lookup"><span data-stu-id="5461f-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="5461f-110">Kommandoen Lagre område som mal støttes ikke, og kan forårsake problemer på områder som bruker infrastrukturen for Publisering av SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="5461f-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="5461f-111">**Områdemalen kan ikke opprettes eller fungerer ikke på riktig måte**</span><span class="sxs-lookup"><span data-stu-id="5461f-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="5461f-112">Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke.</span><span class="sxs-lookup"><span data-stu-id="5461f-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="5461f-113">Hvis funksjonen ikke er tilgjengelig for å aktivere i gjeldende områdesamling, kan du ikke bruke områdemalen til å opprette et område.</span><span class="sxs-lookup"><span data-stu-id="5461f-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="5461f-114">Kontroller om lister eller biblioteker overskrider grenseterskelen for [listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer, da dette kan blokkere oppretting av en områdemal.</span><span class="sxs-lookup"><span data-stu-id="5461f-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="5461f-115">Området kan bruke for mange ressurser, og derfor overskrider områdemalen 50 MB grensen.</span><span class="sxs-lookup"><span data-stu-id="5461f-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="5461f-116">Det er problemer med å vise data fra en liste som bruker en oppslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="5461f-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="5461f-117">Hvis du vil ha mer informasjon, kan du se [Malgenerert liste viser ikke data fra riktig oppslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="5461f-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="5461f-118">Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du sjekke [Opprette og bruke nettstedsmaler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="5461f-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



