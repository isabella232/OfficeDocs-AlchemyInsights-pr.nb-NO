---
title: Problemer med å fjerne en avbords- eller utgangsenhet fra enhetsbeholdningen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564343"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="705e3-102">Problemer med å fjerne en avbords- eller utgangsenhet fra enhetsbeholdningen</span><span class="sxs-lookup"><span data-stu-id="705e3-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="705e3-103">Microsoft Defender for endpoint tillater for øyeblikket ikke manuelt fjerning av enhetsposten for en avbords- eller utgangsenhet fra enhetslageret.</span><span class="sxs-lookup"><span data-stu-id="705e3-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="705e3-104">Av sikkerhetsgrunner forblir enheten i portalen som en historisk post i opptil 180 dager.</span><span class="sxs-lookup"><span data-stu-id="705e3-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="705e3-105">Enhetsdataene slettes imidlertid i henhold til den konfigurerte oppbevaringsperioden.</span><span class="sxs-lookup"><span data-stu-id="705e3-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="705e3-106">**Obs!** En avbords- eller uttrykket enhet bytter automatisk til **Inaktiv** tilstand etter sju dager.</span><span class="sxs-lookup"><span data-stu-id="705e3-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="705e3-107">I tillegg er ikke enheter som er aktive de siste 30 dagene, med i dataene som gjenspeiler organisasjonens Håndtering av trusler og sikkerhetsproblemer eksponeringsresultat eller Microsoft Secure Score for Devices.</span><span class="sxs-lookup"><span data-stu-id="705e3-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="705e3-108">Hvis du fremdeles ikke vil se enkelte enheter i enhetslagervisning, kan du prøve å plassere en enhetskode for å filtrere ut enheten som er utestengt fra Enhetslager-visningen.</span><span class="sxs-lookup"><span data-stu-id="705e3-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="705e3-109">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="705e3-109">For more information, see:</span></span>

[<span data-ttu-id="705e3-110">Eksterne enheter fra Microsoft Defender for endepunkttjenesten</span><span class="sxs-lookup"><span data-stu-id="705e3-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="705e3-111">Eksponeringspoengsum i Håndtering av trusler og sikkerhetsproblemer</span><span class="sxs-lookup"><span data-stu-id="705e3-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="705e3-112">Løse usunne sensorer i Microsoft Defender for endepunkt</span><span class="sxs-lookup"><span data-stu-id="705e3-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="705e3-113">Slik bruker du merking effektivt (del 1)</span><span class="sxs-lookup"><span data-stu-id="705e3-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="705e3-114">Slik bruker du merking effektivt (del 2)</span><span class="sxs-lookup"><span data-stu-id="705e3-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="705e3-115">Slik bruker du merking effektivt (del 3)</span><span class="sxs-lookup"><span data-stu-id="705e3-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




