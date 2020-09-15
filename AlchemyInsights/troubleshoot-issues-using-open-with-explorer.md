---
title: Feilsøke problemer ved bruk av åpne med Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659067"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="47a55-102">Løse problemer med åpne med Explorer</span><span class="sxs-lookup"><span data-stu-id="47a55-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="47a55-103">Løse vanlige problemer med å åpne et dokument bibliotek i SharePoint eller OneDrive ved hjelp av kommandoen **Åpne med Explorer** :</span><span class="sxs-lookup"><span data-stu-id="47a55-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="47a55-104">Bruk Internet Explorer 10 eller Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="47a55-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="47a55-105">**Åpne med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="47a55-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="47a55-106">**Åpne med Explorer** er deaktivert i alle nett lesere bortsett fra Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="47a55-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="47a55-107">**Åpne med Explorer** er ikke tilgjengelig i moderne opplevelse for SharePoint-biblioteker.</span><span class="sxs-lookup"><span data-stu-id="47a55-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="47a55-108">Bruk **visning i fil Utforsker** i stedet.</span><span class="sxs-lookup"><span data-stu-id="47a55-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="47a55-109">Velg **Vis alternativer** - \> **visning i fil Utforsker**.</span><span class="sxs-lookup"><span data-stu-id="47a55-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="47a55-110">Vis i fil Utforsker er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="47a55-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="47a55-111">**Vis bare i fil Utforsker** i tilgjengelig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="47a55-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="47a55-112">Kontroller at WebClient-tjenesten kjører.</span><span class="sxs-lookup"><span data-stu-id="47a55-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="47a55-113">Skriv inn Kjør i Windows Search-boksen, velg Kjør skrive bords-appen, Skriv inn Services. msc, og trykk deretter ENTER.</span><span class="sxs-lookup"><span data-stu-id="47a55-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="47a55-114">Rull ned til WebClient-tjenesten, og kontroller at **status** -kolonnen viser «kjører».</span><span class="sxs-lookup"><span data-stu-id="47a55-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="47a55-115">Hvis den ikke gjør det, dobbelt klikker du tjenesten, klikker **Start**og deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="47a55-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="47a55-116">(Du må kanskje først aktivere tjenesten ved å velge enten **manuell** eller **automatisk** i boksen **oppstarts type** .)</span><span class="sxs-lookup"><span data-stu-id="47a55-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="47a55-117">Det er praktisk å åpne et bibliotek i fil Utforsker hvis du trenger å kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbeide regelmessig i biblioteket, anbefaler vi at du synkroniserer det.</span><span class="sxs-lookup"><span data-stu-id="47a55-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="47a55-118">Hvis du vil feilsøke problemer med å åpne i fil Utforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="47a55-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="47a55-119">Hvis du vil ha informasjon om hvordan du konfigurerer synkronisering, kan du se [synkronisere SharePoint-filer med den nye synkroniserings klienten for OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="47a55-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="47a55-120">Se artikkelen [Slik bruker du kommandoen «åpne med Explorer» til å feilsøke problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="47a55-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

