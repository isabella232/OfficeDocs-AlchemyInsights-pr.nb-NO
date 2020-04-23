---
title: Feilsøke problemer ved hjelp av Åpne med Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759701"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="a760a-102">Løse problemer med Åpne med Explorer</span><span class="sxs-lookup"><span data-stu-id="a760a-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="a760a-103">Løse vanlige problemer med å åpne et dokumentbibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer:**</span><span class="sxs-lookup"><span data-stu-id="a760a-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="a760a-104">Bruk Internet Explorer 10 eller Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="a760a-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="a760a-105">**Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="a760a-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a760a-106">**Åpen med Explorer** er deaktivert i alle nettlesere unntatt Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a760a-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="a760a-107">**Åpen med Explorer** er ikke tilgjengelig i den moderne opplevelsen for SharePoint-biblioteker.</span><span class="sxs-lookup"><span data-stu-id="a760a-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="a760a-108">Bruk **vis i Filutforsker** i stedet.</span><span class="sxs-lookup"><span data-stu-id="a760a-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="a760a-109">Velg **Vis alternativer** \> **Vis i Filutforsker**.</span><span class="sxs-lookup"><span data-stu-id="a760a-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="a760a-110">Visning i Filutforsker er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="a760a-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a760a-111">**Vis i Filutforsker** på tilgjengelig bare i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a760a-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="a760a-112">Kontroller at WebClient-tjenesten kjører.</span><span class="sxs-lookup"><span data-stu-id="a760a-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="a760a-113">Skriv inn kjør i Søkeboksen i Windows, velg Kjør skrivebord-appen, skriv inn services.msc, og trykk deretter Enter.</span><span class="sxs-lookup"><span data-stu-id="a760a-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="a760a-114">Rull ned til WebClient-tjenesten, og kontroller at **Status-kolonnen** viser "Kjører".</span><span class="sxs-lookup"><span data-stu-id="a760a-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="a760a-115">Hvis den ikke gjør det, dobbeltklikker du tjenesten, klikker **Start**, og deretter klikker du **OK**.</span><span class="sxs-lookup"><span data-stu-id="a760a-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="a760a-116">(Du må kanskje aktivere tjenesten først ved å velge **manuell** eller **automatisk** i **oppstartstype-boksen.)**</span><span class="sxs-lookup"><span data-stu-id="a760a-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a760a-117">Det er nyttig å åpne et bibliotek i Filutforsker hvis du må kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi at du synkroniserer det.</span><span class="sxs-lookup"><span data-stu-id="a760a-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="a760a-118">Hvis du vil feilsøke problemer med å åpne filutforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="a760a-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="a760a-119">Hvis du vil ha informasjon om hvordan du konfigurerer synkronisering, kan du se [Synkronisere SharePoint-filer med den nye OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a760a-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="a760a-120">Se artikkelen [Slik bruker du kommandoen "Åpne med Explorer" til å feilsøke problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="a760a-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

