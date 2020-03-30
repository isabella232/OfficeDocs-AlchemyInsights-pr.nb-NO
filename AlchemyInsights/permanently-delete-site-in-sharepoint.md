---
title: Permanent slette et nettsted i SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955244"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="b41bd-102">Permanent slette et nettsted i SharePoint</span><span class="sxs-lookup"><span data-stu-id="b41bd-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="b41bd-103">Hvis du vil bruke en URL-adresse fra et slettet nettsted (til å opprette et nettsted) på nytt, eller for å slette et nettsted permanent fordi det ikke lenger er i bruk, kan du bruke **slette permanent** i det nye administrasjonssenteret for SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b41bd-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="b41bd-104">Gå til [Slettede nettsteder-siden i det nye administrasjons senteret for SharePoint,](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) og logge på med en konto som har administratortillatelser for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="b41bd-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="b41bd-105">Velg et nettsted i venstre kolonne.</span><span class="sxs-lookup"><span data-stu-id="b41bd-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="b41bd-106">Klikk på **Slett Permanent**.</span><span class="sxs-lookup"><span data-stu-id="b41bd-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="b41bd-107">**Merk**: man kan ikke slette gruppetilkoblede områder fra det nye administrasjonssenteret for SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b41bd-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="b41bd-108">[Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) må brukes i stedet.</span><span class="sxs-lookup"><span data-stu-id="b41bd-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="b41bd-109">Hvis du vil ha mer informasjon, se i [slette et nettsted permanent](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="b41bd-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
