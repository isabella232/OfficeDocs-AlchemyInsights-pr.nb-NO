---
title: Åpen med Explorer fungerer ikke
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713043"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="57cbd-102">Åpne med Explorer fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="57cbd-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="57cbd-103">Hvis **Åpne med Explorer** eller Vis i **Filutforsker** ikke fungerer, må du kontrollere at WebClient-tjenesten er satt til **Å kjøre** ved å følge trinnene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="57cbd-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="57cbd-104">Det kan for eksempel ta lang tid å åpne et SharePoint- eller OneDrive-bibliotek når tjenesten ikke kjører.</span><span class="sxs-lookup"><span data-stu-id="57cbd-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="57cbd-105">Skriv inn kjør i Søkeboksen i Windows, velg Kjør skrivebord-appen, skriv inn services.msc, og velg deretter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="57cbd-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="57cbd-106">Bla ned til WebClient-tjenesten, og kontroller **Status-kolonnen.**</span><span class="sxs-lookup"><span data-stu-id="57cbd-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="57cbd-107">Hvis WebClient-tjenestestatusen ikke **kjører**, dobbeltklikker du tjenesten, klikker **Start**, og deretter klikker du **OK**.</span><span class="sxs-lookup"><span data-stu-id="57cbd-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="57cbd-108">Aktiver om nødvendig tjenesten ved å velge **manuell** eller **automatisk** i **Oppstartstype-boksen.**</span><span class="sxs-lookup"><span data-stu-id="57cbd-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="57cbd-109">Hvis du vil feilsøke problemer med å åpne filutforsker, kan du se [Åpne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="57cbd-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="57cbd-110">Utforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="57cbd-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

