---
title: Begrense tilgang en sharepoint eller onedrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715893"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b87bb-102">Begrense tilgang en sharepoint eller onedrive</span><span class="sxs-lookup"><span data-stu-id="b87bb-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b87bb-103">I SharePoint og OneDrive begrenser du tilgangen til elementer som filer, mapper og lister ved å gi tilgang bare til grupper eller enkeltpersoner du vil ha tilgang til.</span><span class="sxs-lookup"><span data-stu-id="b87bb-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="b87bb-104">Som standard arves tillatelser i SharePoint fra høyere opp i hierarkiet.</span><span class="sxs-lookup"><span data-stu-id="b87bb-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="b87bb-105">Så en fil arver tillatelsene fra mappen, som arver tillatelsene fra biblioteket, som arver tillatelsene fra området.</span><span class="sxs-lookup"><span data-stu-id="b87bb-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="b87bb-106">Du kan dele på et høyere nivå (for eksempel ved å dele et helt område) og deretter bryte arv hvis du ikke vil dele alle elementene på området.</span><span class="sxs-lookup"><span data-stu-id="b87bb-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="b87bb-107">Vi anbefaler imidlertid ikke dette fordi det gjør det mer komplisert og forvirrende å opprettholde tillatelsene i fremtiden.</span><span class="sxs-lookup"><span data-stu-id="b87bb-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="b87bb-108">Her er hva du kan gjøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="b87bb-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="b87bb-109">Hvis du for eksempel vil dele alt innholdet i en mappe, bortsett fra én fil i den, flytter du filen til en ny plassering som ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="b87bb-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="b87bb-110">Hvis du har to undermapper i en mappe, og du vil dele én undermappe med gruppe A og B og bare gi gruppe A tilgang til den andre undermappen, deler du den overordnede mappen med gruppe A og legger til gruppe B i den første undermappen.</span><span class="sxs-lookup"><span data-stu-id="b87bb-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="b87bb-111">Slutte å dele en fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="b87bb-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

