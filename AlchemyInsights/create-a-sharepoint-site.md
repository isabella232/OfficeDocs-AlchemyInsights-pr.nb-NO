---
title: Opprette et SharePoint-område
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770864"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="bb066-102">Opprette et SharePoint-område</span><span class="sxs-lookup"><span data-stu-id="bb066-102">Create a SharePoint site</span></span>

<span data-ttu-id="bb066-103">Opprett eller administrer områder fra [aktive områder](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) i administrasjonssenteret for SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bb066-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="bb066-104">Hvis du vil ha mer informasjon, kan du se [Administrere områder i det nye administrasjonssenteret for SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bb066-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="bb066-105">Tips:</span><span class="sxs-lookup"><span data-stu-id="bb066-105">Tips:</span></span>

- <span data-ttu-id="bb066-106">Du **kan ikke** opprette et område med samme URL-adresse for et eksisterende område.</span><span class="sxs-lookup"><span data-stu-id="bb066-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="bb066-107">Hvis du har slettet et nettsted og ønsker å bruke URL-adressen på nytt, er det mulig at det slettede området fortsatt finnes under [Slettede områder](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="bb066-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="bb066-108">Nettstedet må slettes permanent for å bruke URL-adressen på nytt.</span><span class="sxs-lookup"><span data-stu-id="bb066-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="bb066-109">Hvis du vil fjerne et område med Powershell fullstendig, kan du se cmdleten [Fjern SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="bb066-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="bb066-110">Noen brukere kan kanskje ikke opprette et område.</span><span class="sxs-lookup"><span data-stu-id="bb066-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="bb066-111">[Se Administrere områdeoppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bb066-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="bb066-112">Det er mulig at nettstedet vises fast på **Å opprette** lenger enn forventet.</span><span class="sxs-lookup"><span data-stu-id="bb066-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="bb066-113">Hvis mer enn 24 timer har gått siden du først så dette problemet, kan du logge en støttebillett.</span><span class="sxs-lookup"><span data-stu-id="bb066-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="bb066-114">I mange tilfeller jobber vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="bb066-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="bb066-115">Vennligst gi oss minst 24 timer for å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="bb066-115">Please give us at least 24 hours to complete a solution.</span></span>
