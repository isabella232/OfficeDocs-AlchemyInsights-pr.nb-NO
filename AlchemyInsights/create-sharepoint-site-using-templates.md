---
title: Opprette et område i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732242"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="06b0a-102">Opprette SharePoint-nettsteder ved hjelp av maler</span><span class="sxs-lookup"><span data-stu-id="06b0a-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="06b0a-103">Muligheten til å lagre et område som en mal støttes ikke med moderne kommunikasjons-eller gruppe nett steder.</span><span class="sxs-lookup"><span data-stu-id="06b0a-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="06b0a-104">Hvis du vil ha mer informasjon om bruk av maler, kan du se [Lagre, laste ned og laste opp et SharePoint-område som en mal](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)</span><span class="sxs-lookup"><span data-stu-id="06b0a-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="06b0a-105">Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som en mal i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="06b0a-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="06b0a-106">**Knappen Lagre område/liste mal er ikke tilgjengelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="06b0a-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="06b0a-107">Administratorer må tillate egen definert skript for å aktivere mal funksjonene.</span><span class="sxs-lookup"><span data-stu-id="06b0a-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="06b0a-108">For detaljerte trinn kan du se eksempler og hensyn.</span><span class="sxs-lookup"><span data-stu-id="06b0a-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="06b0a-109">Tillate eller forhindre egen definert skript</span><span class="sxs-lookup"><span data-stu-id="06b0a-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="06b0a-110">Kommandoen Lagre område som mal støttes ikke og kan føre til problemer på områder som bruker publiserings infrastrukturen for SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="06b0a-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="06b0a-111">**Nettsteds malen kan ikke opprettes eller fungerer ikke som den skal**</span><span class="sxs-lookup"><span data-stu-id="06b0a-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="06b0a-112">Det kan hende at malen mangler en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og ikke aktiveres.</span><span class="sxs-lookup"><span data-stu-id="06b0a-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="06b0a-113">Hvis funksjonen ikke er tilgjengelig for aktivering i gjeldende område samling, kan du ikke bruke nettsteds malen til å opprette et område.</span><span class="sxs-lookup"><span data-stu-id="06b0a-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="06b0a-114">Kontroller om alle lister eller biblioteker overskrider [terskel verdien for liste visnings grensen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer siden dette kan blokkere oppretting av en nettsteds mal.</span><span class="sxs-lookup"><span data-stu-id="06b0a-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="06b0a-115">Nettstedet bruker kanskje for mange ressurser, og derfor overskrider nettsteds malen grensen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="06b0a-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="06b0a-116">Det er problemer med å vise data fra en liste som bruker en oppslags Kol onnen.</span><span class="sxs-lookup"><span data-stu-id="06b0a-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="06b0a-117">Hvis du vil ha mer informasjon, kan du se [mal gener ert liste viser ikke data fra den riktige oppslags listen i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="06b0a-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="06b0a-118">Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du merke av for [Opprett og bruk nettsteds maler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="06b0a-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



