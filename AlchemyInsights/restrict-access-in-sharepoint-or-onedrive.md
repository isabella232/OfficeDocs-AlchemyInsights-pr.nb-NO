---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551460"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="9c161-102">Begrense tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="9c161-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="9c161-103">I SharePoint og OneDrive kan begrense du tilgangen til elementer, for eksempel filer, mapper og lister ved å gi tilgang bare til grupper eller enkeltpersoner som du vil ha tilgang.</span><span class="sxs-lookup"><span data-stu-id="9c161-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="9c161-104">Som standard tillatelsene i SharePoint, som er arvet fra høyere opp i hierarkiet.</span><span class="sxs-lookup"><span data-stu-id="9c161-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="9c161-105">Så arver en fil tillatelser fra mappen, som arver tillatelser fra biblioteket, som arver tillatelser fra området.</span><span class="sxs-lookup"><span data-stu-id="9c161-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="9c161-106">Du kan dele på et høyere nivå (som ved å dele et helt område) og deretter bryte arvingen for, hvis du ikke vil dele alle elementer på området.</span><span class="sxs-lookup"><span data-stu-id="9c161-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="9c161-107">Men anbefaler vi ikke dette fordi det er å vedlikeholde tillatelser for mer komplekse og forvirrende i fremtiden.</span><span class="sxs-lookup"><span data-stu-id="9c161-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="9c161-108">Her er hva du kan gjøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="9c161-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="9c161-109">Hvis du for eksempel vil dele alt innholdet i en mappe med unntak av én fil i det, kan du flytte filen til en ny plassering som ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="9c161-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="9c161-110">Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og tillate bare A gruppetilgang til den andre undermappen, dele den overordnede mappen med gruppe A og legge til gruppe B i den første undermappen.</span><span class="sxs-lookup"><span data-stu-id="9c161-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="9c161-111">Avslutte deling av en fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="9c161-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

