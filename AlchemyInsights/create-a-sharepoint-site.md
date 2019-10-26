---
title: Opprette et SharePoint-område
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738206"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="2d2c9-102">Opprette et SharePoint-område</span><span class="sxs-lookup"><span data-stu-id="2d2c9-102">Create a SharePoint site</span></span>

<span data-ttu-id="2d2c9-103">Du kan se følgende for informasjon om opprettelse av SharePoint-område:</span><span class="sxs-lookup"><span data-stu-id="2d2c9-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="2d2c9-104">[Behandle områder i det nye administrasjonssenteret for SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Finn ut mer om alternativer for områdeoppretting, blant annet hvordan du oppretter et klassisk område eller et teamområde som ikke inneholder en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="2d2c9-105">[Opprette et gruppeområde i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Lær hvordan du oppretter et gruppeområde.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="2d2c9-106">[Opprette et område for kommunikasjon i SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Finn ut hvordan du oppretter et kommunikasjons område.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="2d2c9-107">[Behandle områder i det nye administrasjonssenteret for SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Lær hvordan du oppretter et klassisk område eller et gruppeområde som ikke inkluderer en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="2d2c9-108">[! Tips</span><span class="sxs-lookup"><span data-stu-id="2d2c9-108">[!Tips]</span></span>
> - <span data-ttu-id="2d2c9-109">Du kan ikke opprette et område med samme URL-adresse for et eksisterende område.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="2d2c9-110">Hvis du slettet et område og ønsker å bruke URL-adressen på nytt, er det mulig at det slettede området fortsatt finnes under **Slettede områder**.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="2d2c9-111">Hvis du vil administrere slettede områder, ser du [slette et område](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="2d2c9-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="2d2c9-112">Hvis du vil fjerne et område med PowerShell fullstendig, kan du se eksemplet på [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="2d2c9-113">Noen brukere vil kanskje ikke kunne opprette et område.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="2d2c9-114">Se [administrere områdeoppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="2d2c9-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="2d2c9-115">Dens ' mulig byggetomta fremgår stakk for **skaper** lengere enn ventet.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="2d2c9-116">Hvis det har gått mer enn 24 timer siden du først så dette problemet, kan du logge en support billett.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2d2c9-117">I mange tilfeller er vi allerede jobber med en løsning.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2d2c9-118">Vennligst gi oss minst 24 timer for å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="2d2c9-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="2d2c9-119">Hvis du må opprette et nytt gruppeområde som ikke inneholder en Office 365-gruppe,</span><span class="sxs-lookup"><span data-stu-id="2d2c9-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


