---
title: Åpne med Explorer fungerer ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481251"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="e8e7a-102">Åpne med Explorer fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="e8e7a-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="e8e7a-p101">Hvis **Åpne med Explorer** eller **visningen i File Explorer** ikke virker Kontroller WebClient-tjenesten er satt til å **kjøre** ved å følge trinnene nedenfor. For eksempel kan det ta lang tid å åpne et SharePoint eller OneDrive bibliotek når tjenesten ikke kjører.</span><span class="sxs-lookup"><span data-stu-id="e8e7a-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="e8e7a-105">I Windows søk-boksen, Skriv inn run, velger du Kjør desktop app, Skriv inn services.msc og deretter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e8e7a-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="e8e7a-p102">Rull ned til WebClient-tjenesten, og kontroller **Status** -kolonnen. Hvis statusen for WebClient-tjenesten ikke er **kjører**, Dobbeltklikk tjenesten, klikk **Start**, og klikk deretter **OK**. Aktiver tjenesten, hvis det er nødvendig, ved å velge enten **Manuell** eller **automatisk** i boksen **Oppstartstype** .</span><span class="sxs-lookup"><span data-stu-id="e8e7a-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e8e7a-p103">Hvis du vil feilsøke problemer med å åpne i File Explorer, kan du se [åpen i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Utforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e8e7a-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

