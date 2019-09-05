---
title: Feilsøke problemer med åpne med Explorer
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742742"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="2a2e1-102">Løs problemer med åpne med Explorer</span><span class="sxs-lookup"><span data-stu-id="2a2e1-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="2a2e1-103">Løs vanlige problemer med å åpne et dokumentbibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer** :</span><span class="sxs-lookup"><span data-stu-id="2a2e1-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="2a2e1-104">Bruk Internet Explorer 10 eller 11 for Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="2a2e1-105">**Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a2e1-106">**Åpne med Explorer** er deaktivert i alle nettlesere unntatt Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a2e1-107">**Åpne med Explorer** er ikke tilgjengelig i den moderne opplevelsen for SharePoint-biblioteker.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="2a2e1-108">Bruk **visning i Filutforsker** i stedet.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="2a2e1-109">Velg **Vis alternativer** \> **-visning i Filutforsker**.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="2a2e1-110">Utsikt inne arkiv utforske er ikke forenlig med Microsoft kant, Google Chrome, gi avskjed og andre.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a2e1-111">**Visning i Filutforsker** i bare tilgjengelig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a2e1-112">Kontroller at WebClient-tjenesten kjører.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="2a2e1-113">Skriv Kjør i søkeboksen i Windows, velg Kjør skrivebordsprogrammet, Skriv inn Services. msc, og trykk deretter ENTER.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="2a2e1-114">Bla ned til WebClient-tjenesten, og kontroller at **status** -kolonnen viser "running".</span><span class="sxs-lookup"><span data-stu-id="2a2e1-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="2a2e1-115">Hvis den ikke gjør det, dobbeltklikker du tjenesten, klikker **Start**, og deretter klikker du **OK**.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2a2e1-116">(Du må kanskje først aktivere tjenesten ved å velge enten **manuell** eller **automatisk** i boksen **Oppstartstype** .)</span><span class="sxs-lookup"><span data-stu-id="2a2e1-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2a2e1-117">Det er nyttig å åpne et bibliotek i Filutforsker hvis du må kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi at du synkroniserer det.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="2a2e1-118">Hvis du vil feilsøke problemer som åpnes i Filutforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="2a2e1-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2a2e1-119">Hvis du vil ha informasjon om hvordan du konfigurerer synkronisering, kan [du se synkronisere SharePoint-filer med den nye OneDrive Sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2a2e1-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="2a2e1-120">Se artikkelen [hvordan du bruker kommandoen "åpne med Explorer" til å feilsøke problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

