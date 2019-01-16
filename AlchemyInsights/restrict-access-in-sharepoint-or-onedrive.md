---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303298"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="c85d8-102">Begrense tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="c85d8-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="c85d8-p101">I SharePoint og OneDrive kan begrense du tilgangen til elementer, for eksempel filer, mapper og lister ved å gi tilgang bare til grupper eller enkeltpersoner som du vil ha tilgang. Som standard tillatelsene i SharePoint, som er arvet fra høyere opp i hierarkiet. Så arver en fil tillatelser fra mappen, som arver tillatelser fra biblioteket, som arver tillatelser fra området.</span><span class="sxs-lookup"><span data-stu-id="c85d8-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="c85d8-p102">Du kan dele på et høyere nivå (som ved å dele et helt område) og deretter bryte arvingen for, hvis du ikke vil dele alle elementer på området. Men anbefaler vi ikke dette fordi det er å vedlikeholde tillatelser for mer komplekse og forvirrende i fremtiden. Her er hva du kan gjøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="c85d8-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="c85d8-109">Hvis du for eksempel vil dele alt innholdet i en mappe med unntak av én fil i det, kan du flytte filen til en ny plassering som ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="c85d8-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="c85d8-110">Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og tillate bare A gruppetilgang til den andre undermappen, dele den overordnede mappen med gruppe A og legge til gruppe B i den første undermappen.</span><span class="sxs-lookup"><span data-stu-id="c85d8-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="c85d8-111">Avslutte deling av en fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="c85d8-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

