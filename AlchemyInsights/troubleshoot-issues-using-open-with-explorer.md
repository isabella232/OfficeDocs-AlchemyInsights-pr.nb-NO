---
title: Feilsøke problemer med å bruke åpne med Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 6e67c2916e0c5739f6126064d45e175a7fd6f8d4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500224"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="dceda-102">Løs problemer med åpne med Explorer</span><span class="sxs-lookup"><span data-stu-id="dceda-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="dceda-103">Løs vanlige problemer med å åpne et dokumentbibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer** :</span><span class="sxs-lookup"><span data-stu-id="dceda-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="dceda-104">Bruke Internet Explorer 10 eller 11 for Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="dceda-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="dceda-105">**Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="dceda-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="dceda-106">**Åpne med Explorer** er deaktivert i alle lesere bortsett fra Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="dceda-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="dceda-107">**Åpne med Explorer** er ikke tilgjengelig i den moderne opplevelsen for SharePoint-biblioteker.</span><span class="sxs-lookup"><span data-stu-id="dceda-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="dceda-108">Bruk **visningen i File Explorer** i stedet.</span><span class="sxs-lookup"><span data-stu-id="dceda-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="dceda-109">Velg **Alternativer for** \> **visning i Filutforsker**.</span><span class="sxs-lookup"><span data-stu-id="dceda-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="dceda-110">Vis i File Explorer, er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="dceda-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="dceda-111">**Vis i Filutforsker** i bare tilgjengelig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="dceda-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="dceda-112">Kontroller at WebClient-tjenesten kjører.</span><span class="sxs-lookup"><span data-stu-id="dceda-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="dceda-113">I Windows søk-boksen, Skriv inn run, velger Kjør stasjonær programmet, Skriv inn services.msc og trykk deretter Enter.</span><span class="sxs-lookup"><span data-stu-id="dceda-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="dceda-114">Rull ned til WebClient-tjenesten, og kontroller at **Status** -kolonnen viser "Som kjører."</span><span class="sxs-lookup"><span data-stu-id="dceda-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="dceda-115">Hvis ikke, Dobbeltklikk tjenesten, klikk **Start**, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="dceda-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="dceda-116">(Du må kanskje først aktivere tjenesten ved å velge enten **Manuell** eller **automatisk** i boksen **Oppstartstype** .)</span><span class="sxs-lookup"><span data-stu-id="dceda-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="dceda-117">Åpne et bibliotek i Filutforsker er nyttig hvis du skal kopiere eller flytte flere filer og mapper når, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi synkroniserer den.</span><span class="sxs-lookup"><span data-stu-id="dceda-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="dceda-118">Hvis du vil feilsøke problemer med å åpne i File Explorer, kan du se [åpen i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="dceda-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="dceda-119">For informasjon om hvordan du definerer synkronisering, kan du se [Synkroniser SharePoint-filer med den nye OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="dceda-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="dceda-120">Se [hvordan du bruker kommandoen "Åpne med Explorer" til å feilsøke problemer i SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) -artikkelen for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="dceda-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

