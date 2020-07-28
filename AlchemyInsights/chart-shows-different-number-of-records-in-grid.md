---
title: Diagrammet viser forskjellig antall poster i rutenettet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439956"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="e4fef-102">Diagrammet viser forskjellig antall poster i rutenettet</span><span class="sxs-lookup"><span data-stu-id="e4fef-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="e4fef-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="e4fef-103">**Symptom**</span></span>

<span data-ttu-id="e4fef-104">For diagram på instrumentbordsiden, når du klikker på diagrammet "..." og klikk på "Vis poster", navigerer du til rutenettsiden for å se alle postene. Noen ganger endres antall oppføringer.</span><span class="sxs-lookup"><span data-stu-id="e4fef-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="e4fef-105">**Årsak**</span><span class="sxs-lookup"><span data-stu-id="e4fef-105">**Cause**</span></span>

<span data-ttu-id="e4fef-106">Dette skyldes forskjellen mellom visninger mellom diagrammet på den opprinnelige instrumentbordsiden og diagrammet på hjemmesiden for rutenettet.</span><span class="sxs-lookup"><span data-stu-id="e4fef-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="e4fef-107">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="e4fef-107">**Solution**</span></span>

1. <span data-ttu-id="e4fef-108">Kontroller visningen fra den opprinnelige siden og visningen i rutenettet for å se om de er forskjellige.</span><span class="sxs-lookup"><span data-stu-id="e4fef-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="e4fef-109">Endre visningen i rutenettet slik at den samsvarer med visningen på den opprinnelige siden.</span><span class="sxs-lookup"><span data-stu-id="e4fef-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="e4fef-110">Hvis den riktige visningen ikke blir funnet, betyr det vanligvis at visningen ikke er aktivert i apputforming.</span><span class="sxs-lookup"><span data-stu-id="e4fef-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="e4fef-111">Gå til apputforming av den bestemte appen, velg enheten og visningene, sjekk visningen du vil aktivere, lagre, publisere og lukke.</span><span class="sxs-lookup"><span data-stu-id="e4fef-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="e4fef-112">Oppdater siden.</span><span class="sxs-lookup"><span data-stu-id="e4fef-112">Refresh the page.</span></span>