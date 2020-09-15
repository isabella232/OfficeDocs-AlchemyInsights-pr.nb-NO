---
title: Åpne med Explorer fungerer ikke
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694465"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="a7c28-102">Åpne med Explorer fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="a7c28-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="a7c28-103">Hvis **Åpne med Utforsker** eller **Vis i fil Utforsker** ikke fungerer, kan du ikke sørge for at WebClient-tjenesten er satt til å **kjøre** ved å følge Fremgangs måten nedenfor.</span><span class="sxs-lookup"><span data-stu-id="a7c28-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="a7c28-104">Det kan for eksempel gå lang tid å åpne et SharePoint-eller OneDrive-bibliotek når tjenesten ikke kjører.</span><span class="sxs-lookup"><span data-stu-id="a7c28-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="a7c28-105">Skriv inn Kjør i Windows Search-boksen, velg Kjør skrive bords-appen, Skriv inn Services. msc, og velg deretter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a7c28-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="a7c28-106">Rull ned til WebClient-tjenesten, og kontroller **status** -kolonnen.</span><span class="sxs-lookup"><span data-stu-id="a7c28-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="a7c28-107">Hvis tjeneste statusen WebClient ikke **kjører**, dobbelt klikker du tjenesten, klikker **Start**og deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="a7c28-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="a7c28-108">Aktiver tjenesten, hvis nødvendig, ved å velge enten **manuell** eller **automatisk** i boksen **oppstarts type** .</span><span class="sxs-lookup"><span data-stu-id="a7c28-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a7c28-109">Hvis du vil feilsøke problemer med å åpne i fil Utforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="a7c28-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="a7c28-110">Utforsk synkronisering som et bedre alternativ: [synkronisere SharePoint-filer med den nye synkroniserings klienten for OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a7c28-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

