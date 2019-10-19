---
title: Begrens tilgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551460"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="15462-102">Begrens tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="15462-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="15462-103">I SharePoint og OneDrive begrenser du tilgangen til elementer som filer, mapper og lister ved bare å gi tilgang til grupper eller enkeltpersoner du vil ha tilgang til.</span><span class="sxs-lookup"><span data-stu-id="15462-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="15462-104">Som standard arves tillatelser i SharePoint fra høyere opp i hierarkiet.</span><span class="sxs-lookup"><span data-stu-id="15462-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="15462-105">En fil arver derfor tillatelsene fra mappen, som arver tillatelsene fra biblioteket, som arver tillatelsene fra området.</span><span class="sxs-lookup"><span data-stu-id="15462-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="15462-106">Du kan dele på et høyere nivå (for eksempel ved å dele et helt område) og deretter bryte arv hvis du ikke vil dele alle elementene på området.</span><span class="sxs-lookup"><span data-stu-id="15462-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="15462-107">Men vi anbefaler ikke dette fordi det gjør opprettholde tillatelsene mer komplekse og forvirrende i fremtiden.</span><span class="sxs-lookup"><span data-stu-id="15462-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="15462-108">Her er hva du kan gjøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="15462-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="15462-109">Hvis du for eksempel vil dele alt innholdet i en mappe med unntak av én fil, flytter du denne filen til en ny plassering som ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="15462-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="15462-110">Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og bare gi tilgang til den andre under mappen, deler du den overordnede mappen med gruppe A og legger til gruppe B i den første under mappen.</span><span class="sxs-lookup"><span data-stu-id="15462-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="15462-111">Avslutte deling av en fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="15462-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

