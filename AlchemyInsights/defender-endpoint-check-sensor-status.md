---
title: Kontrollsensorstatus for Defender-endepunkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676342"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="82d82-102">Kontrollsensorstatus for Defender-endepunkt</span><span class="sxs-lookup"><span data-stu-id="82d82-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="82d82-103">Flisen **Enheter med sensorproblemer** er plassert på instrumentbordet for sikkerhetsoperasjoner.</span><span class="sxs-lookup"><span data-stu-id="82d82-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="82d82-104">Denne flisen gir informasjon om den enkelte enhetens mulighet til å gi sensordata og kommunisere med Defender for endpoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="82d82-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="82d82-105">Den rapporterer hvor mange enheter som krever oppmerksomhet og hjelper deg med å identifisere problematiske enheter og iverksette tiltak for å løse kjente problemer.</span><span class="sxs-lookup"><span data-stu-id="82d82-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="82d82-106">To statusindikatorer på flisen gir informasjon om antall enheter som ikke rapporterer riktig til tjenesten:</span><span class="sxs-lookup"><span data-stu-id="82d82-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="82d82-107">**Feilkonfigurert** Enheter som kanskje delvis rapporterer sensordata til Defender for Endpoint-tjenesten, og som kan ha konfigurasjonsfeil som må rettes opp.</span><span class="sxs-lookup"><span data-stu-id="82d82-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="82d82-108">**Inaktiv** Enheter som har sluttet å rapportere til Defender for endepunkttjenesten i mer enn sju dager den siste måneden.</span><span class="sxs-lookup"><span data-stu-id="82d82-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="82d82-109">Når du klikker en av gruppene, dirigerer du til Enheter-listen, filtrert i henhold til valgene dine.</span><span class="sxs-lookup"><span data-stu-id="82d82-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="82d82-110">I Enheter-listen kan du filtrere tilstandsstatuslisten etter følgende status:</span><span class="sxs-lookup"><span data-stu-id="82d82-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="82d82-111">**Aktiv** Enheter som aktivt rapporterer til Defender for endepunkttjenesten.</span><span class="sxs-lookup"><span data-stu-id="82d82-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="82d82-112">**Feilkonfigurert** Enheter som delvis rapporterer sensordata til Defender for endpoint-tjenesten, men som har konfigurasjonsfeil som må rettes opp.</span><span class="sxs-lookup"><span data-stu-id="82d82-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="82d82-113">Feilkonfigurerte enheter kan ha enten én eller en kombinasjon av følgende problemer:</span><span class="sxs-lookup"><span data-stu-id="82d82-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="82d82-114">Ingen sensordata – Enheter har sluttet å sende sensordata.</span><span class="sxs-lookup"><span data-stu-id="82d82-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="82d82-115">Begrensede varsler kan utløses fra enheten.</span><span class="sxs-lookup"><span data-stu-id="82d82-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="82d82-116">Nedsatt kommunikasjon – Muligheten til å kommunisere med enheten er nedsatt.</span><span class="sxs-lookup"><span data-stu-id="82d82-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="82d82-117">Sending av filer for dyp analyse, blokkering av filer, isolering av enhet fra nettverket og andre handlinger som krever kommunikasjon med enheten, fungerer kanskje ikke.</span><span class="sxs-lookup"><span data-stu-id="82d82-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="82d82-118">**Inaktiv** Enheter som har sluttet å rapportere til Defender for endepunkttjenesten.</span><span class="sxs-lookup"><span data-stu-id="82d82-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="82d82-119">Du kan laste ned hele listen i CSV-format ved hjelp av Eksporter-funksjonen.</span><span class="sxs-lookup"><span data-stu-id="82d82-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="82d82-120">Hvis du vil ha mer informasjon, kan du se Kontrollere tilstanden til [sensoren i Microsoft Defender for endepunkt](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="82d82-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="82d82-121">Hvis du vil ha mer informasjon om hva som førte til at en enhet var inaktiv eller feilkonfigurert, kan du se Reparere usunne sensorer i [Microsoft Defender for endepunkt](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="82d82-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
