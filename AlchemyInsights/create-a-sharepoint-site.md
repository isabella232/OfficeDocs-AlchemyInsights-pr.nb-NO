---
title: Opprette et SharePoint-område
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806948"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="ff0cc-102">Opprette et SharePoint-område</span><span class="sxs-lookup"><span data-stu-id="ff0cc-102">Create a SharePoint site</span></span>

<span data-ttu-id="ff0cc-103">Opprette eller behandle områder fra [aktive nett steder](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) i administrasjons senteret for SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="ff0cc-104">Hvis du vil ha mer informasjon, kan du se [administrere områder i det nye administrasjons senteret for SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ff0cc-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="ff0cc-105">Råd</span><span class="sxs-lookup"><span data-stu-id="ff0cc-105">Tips:</span></span>

- <span data-ttu-id="ff0cc-106">Du **kan ikke** opprette et nettsted med den samme URL-adressen til et eksisterende nettsted.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="ff0cc-107">Hvis du har slettet et nettsted og ønsker å bruke Netta dressen på nytt, er det mulig at det slettede nettstedet fremdeles finnes under [Slettede nett steder](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="ff0cc-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="ff0cc-108">Området må slettes permanent for å bruke Netta dressen på nytt.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="ff0cc-109">Hvis du vil fjerne et nettsted med PowerShell fullstendig, kan du se eksempel på [Fjern SPSite-](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="ff0cc-110">Det kan hende at noen brukere ikke kan opprette et område.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="ff0cc-111">[Se administrere område oppretting i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ff0cc-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="ff0cc-112">Det er mulig at området ser fast ut for å **opprette** mer enn forventet.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="ff0cc-113">Hvis det har gått mer enn 24 timer siden du så dette problemet, kan du logge en støtte forespørsel.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="ff0cc-114">I mange tilfeller arbeider vi allerede med en løsning.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ff0cc-115">Gi oss minst 24 timer til å fullføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="ff0cc-115">Please give us at least 24 hours to complete a solution.</span></span>
