---
title: Kan ikke slette elementer i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049526"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="98ca9-102">Kan ikke slette elementer</span><span class="sxs-lookup"><span data-stu-id="98ca9-102">Unable to delete items</span></span>

<span data-ttu-id="98ca9-103">Har du problemer med å slette SharePoint-elementer?</span><span class="sxs-lookup"><span data-stu-id="98ca9-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="98ca9-104">Kontroller alltid at du har de [nødvendige tillatelsene](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) til å slette elementet, eller at en [administrator for områdesamling](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) prøver å fjerne elementet.</span><span class="sxs-lookup"><span data-stu-id="98ca9-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="98ca9-105">Kontroller at det ikke finnes et oppsett for [oppbevaringspolicy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) for elementet.</span><span class="sxs-lookup"><span data-stu-id="98ca9-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="98ca9-106">Kontroller at elementet ikke er [sjekket ut](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.</span><span class="sxs-lookup"><span data-stu-id="98ca9-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="98ca9-107">Administratorer kan bruke SharePoint- [mønstre og-metoder](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som inneholder et bibliotek med PowerShell-kommandoer som gjør det mulig å utføre kompliserte administrasjons handlinger, for eksempel tvinge sletting av sta elementer.</span><span class="sxs-lookup"><span data-stu-id="98ca9-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="98ca9-108">Fjern PNP-fil</span><span class="sxs-lookup"><span data-stu-id="98ca9-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="98ca9-109">Fjern PNP-mappe</span><span class="sxs-lookup"><span data-stu-id="98ca9-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="98ca9-110">Fjern PNP listeelement</span><span class="sxs-lookup"><span data-stu-id="98ca9-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="98ca9-111">Fjern PNP-liste</span><span class="sxs-lookup"><span data-stu-id="98ca9-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="98ca9-112">Fjern PNP-felt (kolonne)</span><span class="sxs-lookup"><span data-stu-id="98ca9-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)