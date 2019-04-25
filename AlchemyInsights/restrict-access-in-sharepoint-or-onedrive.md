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
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383880"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="5af35-102">Begrense tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="5af35-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="5af35-103">I SharePoint og OneDrive kan begrense du tilgangen til elementer, for eksempel filer, mapper og lister ved å gi tilgang bare til grupper eller enkeltpersoner som du vil ha tilgang.</span><span class="sxs-lookup"><span data-stu-id="5af35-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="5af35-104">Som standard tillatelsene i SharePoint, som er arvet fra høyere opp i hierarkiet.</span><span class="sxs-lookup"><span data-stu-id="5af35-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="5af35-105">Så arver en fil tillatelser fra mappen, som arver tillatelser fra biblioteket, som arver tillatelser fra området.</span><span class="sxs-lookup"><span data-stu-id="5af35-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="5af35-106">Du kan dele på et høyere nivå (som ved å dele et helt område) og deretter bryte arvingen for, hvis du ikke vil dele alle elementer på området.</span><span class="sxs-lookup"><span data-stu-id="5af35-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="5af35-107">Men anbefaler vi ikke dette fordi det er å vedlikeholde tillatelser for mer komplekse og forvirrende i fremtiden.</span><span class="sxs-lookup"><span data-stu-id="5af35-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="5af35-108">Her er hva du kan gjøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="5af35-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="5af35-109">Hvis du for eksempel vil dele alt innholdet i en mappe med unntak av én fil i det, kan du flytte filen til en ny plassering som ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="5af35-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="5af35-110">Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og tillate bare A gruppetilgang til den andre undermappen, dele den overordnede mappen med gruppe A og legge til gruppe B i den første undermappen.</span><span class="sxs-lookup"><span data-stu-id="5af35-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="5af35-111">Avslutte deling av en fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="5af35-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

