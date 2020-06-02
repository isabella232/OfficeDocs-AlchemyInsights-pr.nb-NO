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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511985"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="71be5-102">Kan ikke slette elementer</span><span class="sxs-lookup"><span data-stu-id="71be5-102">Unable to delete items</span></span>

<span data-ttu-id="71be5-103">Oppbevaringspolicyer kan føre til dette, du må enten deaktivere eller utelate respektive sperre som forårsaker dette problemet.</span><span class="sxs-lookup"><span data-stu-id="71be5-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="71be5-104">Når en oppbevaringspolicy eller hold er fjernet, kan det ta opptil 24 timer før endringen trer i kraft.</span><span class="sxs-lookup"><span data-stu-id="71be5-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="71be5-105">Kontroller at det ikke finnes et oppsett [for oppbevaringspolicy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) på varen.</span><span class="sxs-lookup"><span data-stu-id="71be5-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="71be5-106">Området kan ha overskredet lagringsgrensen, øke [områdekvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) og slette elementet.</span><span class="sxs-lookup"><span data-stu-id="71be5-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="71be5-107">Kontroller at elementet ikke er [sjekket ut](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.</span><span class="sxs-lookup"><span data-stu-id="71be5-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="71be5-108">Til slutt kan administratorer bruke [SharePoint-mønstre og -praksiser](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som inneholder et bibliotek med PowerShell-kommandoer som lar deg utføre komplekse administrasjonshandlinger, for eksempel tvinge sletting av vanskelige elementer.</span><span class="sxs-lookup"><span data-stu-id="71be5-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="71be5-109">Fjern PNP-fil</span><span class="sxs-lookup"><span data-stu-id="71be5-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="71be5-110">Fjern PNP-mappe</span><span class="sxs-lookup"><span data-stu-id="71be5-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="71be5-111">Fjerne PNP-listeelement</span><span class="sxs-lookup"><span data-stu-id="71be5-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="71be5-112">Fjern PNP-liste</span><span class="sxs-lookup"><span data-stu-id="71be5-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="71be5-113">Fjerne PNP-felt (kolonne)</span><span class="sxs-lookup"><span data-stu-id="71be5-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)