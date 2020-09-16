---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720691"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="52766-102">Begrense tilgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="52766-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="52766-103">I SharePoint og OneDrive begrenser du tilgang til elementer som filer, mapper og lister ved å gi tilgang bare til grupper eller enkelt personer du vil ha tilgang til.</span><span class="sxs-lookup"><span data-stu-id="52766-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="52766-104">Tillatelser i SharePoint arves som standard fra høyere opp i hierarkiet.</span><span class="sxs-lookup"><span data-stu-id="52766-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="52766-105">Så en fil arver tillatelsene fra mappen, som arver tillatelsene fra biblioteket, som arver tillatelsene fra området.</span><span class="sxs-lookup"><span data-stu-id="52766-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="52766-106">Du kan dele på et høyere nivå (for eksempel ved å dele et helt nettsted) og deretter bryte arv hvis du ikke vil dele alle elementene på området.</span><span class="sxs-lookup"><span data-stu-id="52766-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="52766-107">Vi anbefaler imidlertid ikke dette fordi det gjør det enklere å vedlikeholde tillatelsene mer komplisert og forvirrende i fremtiden.</span><span class="sxs-lookup"><span data-stu-id="52766-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="52766-108">Dette kan du gjøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="52766-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="52766-109">Hvis du for eksempel vil dele alt innholdet i en mappe bortsett fra én fil i den, flytter du filen til en ny plassering som ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="52766-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="52766-110">Hvis du har to under mapper i en mappe, og du vil dele én under mappe med grupper A og B og bare gi gruppen tilgang til den andre under mappen, kan du dele den overordnede mappen med grupper A og legge til gruppe B i den første under mappen.</span><span class="sxs-lookup"><span data-stu-id="52766-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="52766-111">Stoppe deling av en fil eller mappe </span><span class="sxs-lookup"><span data-stu-id="52766-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

