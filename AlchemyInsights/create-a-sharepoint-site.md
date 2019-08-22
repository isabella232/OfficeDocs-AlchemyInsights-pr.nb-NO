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
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515816"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="70ff8-102">Opprette et SharePoint-område</span><span class="sxs-lookup"><span data-stu-id="70ff8-102">Create a SharePoint site</span></span>

<span data-ttu-id="70ff8-103">Du kan se følgende informasjon om oppretting av SharePoint-område:</span><span class="sxs-lookup"><span data-stu-id="70ff8-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="70ff8-104">[Administrere områder i den nye SharePoint-administrasjonssenteret](https://docs.microsoft.com/sharepoint/manage-site-creation): Lær mer om alternativer for oppretting av området, inkludert hvordan du oppretter et klassisk område eller et Team-område som ikke inneholder en Office 365-gruppen.</span><span class="sxs-lookup"><span data-stu-id="70ff8-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="70ff8-105">[Opprett et teamområde i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Lær hvordan du oppretter et gruppeområde.</span><span class="sxs-lookup"><span data-stu-id="70ff8-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="70ff8-106">[Opprett et område for kommunikasjon i SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Lær hvordan du oppretter et område for kommunikasjon.</span><span class="sxs-lookup"><span data-stu-id="70ff8-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="70ff8-107">[Administrere områder i den nye SharePoint-administrasjonssenteret](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Lær hvordan du oppretter et klassisk område eller et gruppeområde som ikke omfatter en gruppe for Office 365.</span><span class="sxs-lookup"><span data-stu-id="70ff8-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Tips]
> - <span data-ttu-id="70ff8-109">Du kan ikke opprette et område med samme URL-adressen for et eksisterende område.</span><span class="sxs-lookup"><span data-stu-id="70ff8-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="70ff8-110">Hvis du har slettet et område, og er som ønsker å bruke URL-adressen på nytt, er det mulig det slettede området fremdeles finnes under **områder slettet**.</span><span class="sxs-lookup"><span data-stu-id="70ff8-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="70ff8-111">Slette områder, kan du se [slette et område](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)til å behandle.</span><span class="sxs-lookup"><span data-stu-id="70ff8-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="70ff8-112">For å fullstendig fjerne et område med Powershell, kan du se eksemplet [Fjern-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) -cmdleten.</span><span class="sxs-lookup"><span data-stu-id="70ff8-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="70ff8-113">Noen brukere kan ikke opprette et område.</span><span class="sxs-lookup"><span data-stu-id="70ff8-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="70ff8-114">Se [Behandle områdeoppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="70ff8-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="70ff8-115">Det er mulig, vises området sitter fast på **opprette** lengre tid enn forventet.</span><span class="sxs-lookup"><span data-stu-id="70ff8-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="70ff8-116">Hvis det har gått mer enn 24 timer etter at du først så dette problemet, logger du deg en support billett.</span><span class="sxs-lookup"><span data-stu-id="70ff8-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="70ff8-117">I mange tilfeller kan arbeider vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="70ff8-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="70ff8-118">Gi oss minst 24 timer å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="70ff8-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="70ff8-119">Hvis du vil opprette et nytt teamområde som ikke inneholder en Office 365-gruppen</span><span class="sxs-lookup"><span data-stu-id="70ff8-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


