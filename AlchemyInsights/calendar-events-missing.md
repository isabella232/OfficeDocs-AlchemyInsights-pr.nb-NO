---
title: Kalenderhendelser mangler eller oppdateres ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837386"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="1de73-102">Kalenderhendelser mangler eller oppdateres ikke</span><span class="sxs-lookup"><span data-stu-id="1de73-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="1de73-103">Hvis kalenderelementer mangler eller ikke oppdateres, begynner du med å se på elementantallet i kalendermappeegenskapene i Outlook:</span><span class="sxs-lookup"><span data-stu-id="1de73-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="1de73-104">Høyreklikk på den berørte **brukerkalendermappen,** og velg deretter **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="1de73-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="1de73-105">Velg **Synkronisering-fanen.**</span><span class="sxs-lookup"><span data-stu-id="1de73-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="1de73-106">Hvis elementantallet ikke er det samme mellom Server-mappen og Den frakoblede mappen:</span><span class="sxs-lookup"><span data-stu-id="1de73-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="1de73-107">Merk **Kalender-mappen.**</span><span class="sxs-lookup"><span data-stu-id="1de73-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="1de73-108">Gå til **Send** / **mottak-fanen,** og velg deretter **Oppdater mappe**.</span><span class="sxs-lookup"><span data-stu-id="1de73-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="1de73-109">Hvis kalenderen fremdeles ikke oppdateres eller hendelser mangler, kan du laste ned verktøyet for kalenderkontroll for Outlook fra [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=28786).</span><span class="sxs-lookup"><span data-stu-id="1de73-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="1de73-110">Finn ut om det er mer enn 5000 elementer i kalendermappen, da dette kan føre til symptomer, for eksempel kalendermøter som ikke er oppdatert eller møtefeil.</span><span class="sxs-lookup"><span data-stu-id="1de73-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="1de73-111">Hvis du vil ha mer informasjon, kan du se Ytelsesproblemer i Outlook når det er for mange elementer eller mapper i en [bufret modus OST- eller PST-fil](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span><span class="sxs-lookup"><span data-stu-id="1de73-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>