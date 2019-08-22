---
title: Åpne med Explorer fungerer ikke
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538490"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="03564-102">Åpne med Explorer fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="03564-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="03564-103">Hvis **Åpne med Explorer** eller **visningen i File Explorer** ikke virker Kontroller WebClient-tjenesten er satt til å **kjøre** ved å følge trinnene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="03564-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="03564-104">For eksempel kan det ta lang tid å åpne et SharePoint eller OneDrive bibliotek når tjenesten ikke kjører.</span><span class="sxs-lookup"><span data-stu-id="03564-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="03564-105">I Windows søk-boksen, Skriv inn run, velger du Kjør desktop app, Skriv inn services.msc og deretter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="03564-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="03564-106">Rull ned til WebClient-tjenesten, og kontroller **Status** -kolonnen.</span><span class="sxs-lookup"><span data-stu-id="03564-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="03564-107">Hvis statusen for WebClient-tjenesten ikke er **kjører**, Dobbeltklikk tjenesten, klikk **Start**, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="03564-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="03564-108">Aktiver tjenesten, hvis det er nødvendig, ved å velge enten **Manuell** eller **automatisk** i boksen **Oppstartstype** .</span><span class="sxs-lookup"><span data-stu-id="03564-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="03564-109">Hvis du vil feilsøke problemer med å åpne i File Explorer, kan du se [åpen i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="03564-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="03564-110">Utforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="03564-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

