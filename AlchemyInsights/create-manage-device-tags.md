---
title: Opprette og behandle enhetskoder eller grupper
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731670"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="1d939-102">Opprette og behandle enhetskoder eller grupper</span><span class="sxs-lookup"><span data-stu-id="1d939-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="1d939-103">Legg til koder på enheter for å opprette en logisk gruppetilhørighet.</span><span class="sxs-lookup"><span data-stu-id="1d939-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="1d939-104">Enhetskoder støtter riktig tilordning av nettverket, slik at du kan legge ved forskjellige koder for å registrere kontekst og aktivere dynamisk listeoppretting som en del av en hendelse.</span><span class="sxs-lookup"><span data-stu-id="1d939-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="1d939-105">Koder kan brukes som et filter i Listevisning for enheter eller til å gruppere enheter.</span><span class="sxs-lookup"><span data-stu-id="1d939-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="1d939-106">Hvis du vil ha mer informasjon om enhetsgruppering, kan [du se Opprette og behandle enhetskoder](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="1d939-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="1d939-107">Du kan legge til koder på enheter ved å:</span><span class="sxs-lookup"><span data-stu-id="1d939-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="1d939-108">Bruke portalen</span><span class="sxs-lookup"><span data-stu-id="1d939-108">Using the portal</span></span>

- <span data-ttu-id="1d939-109">Angi en registernøkkelverdi</span><span class="sxs-lookup"><span data-stu-id="1d939-109">Setting a registry key value</span></span>
 
<span data-ttu-id="1d939-110">**Obs!** Det kan være ventetid mellom når en kode legges til på en enhet og tilgjengeligheten på enhetslisten og enhetssiden.</span><span class="sxs-lookup"><span data-stu-id="1d939-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="1d939-111">Hvis du vil legge til enhetskoder ved hjelp av API, kan du [se Legge til eller fjerne API-koder for enheter](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="1d939-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="1d939-112">Legge til og behandle enhetskoder ved hjelp av portalen</span><span class="sxs-lookup"><span data-stu-id="1d939-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="1d939-113">Velg enheten du vil administrere koder på.</span><span class="sxs-lookup"><span data-stu-id="1d939-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="1d939-114">Du kan velge eller søke etter en enhet fra en av følgende visninger:</span><span class="sxs-lookup"><span data-stu-id="1d939-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="1d939-115">**Instrumentbord for sikkerhetsoperasjoner** Velg enhetsnavnet fra delen Øverste enheter med aktive varsler.</span><span class="sxs-lookup"><span data-stu-id="1d939-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="1d939-116">**Varslingskø** – Velg enhetsnavnet ved siden av enhetsikonet fra varslingskøen.</span><span class="sxs-lookup"><span data-stu-id="1d939-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="1d939-117">**Enhetsliste** – Velg enhetsnavnet fra listen over enheter.</span><span class="sxs-lookup"><span data-stu-id="1d939-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="1d939-118">**Søkeboks** – Velg Enhet fra rullegardinmenyen, og skriv inn navnet på enheten.</span><span class="sxs-lookup"><span data-stu-id="1d939-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="1d939-119">Du kan også gå til varselsiden gjennom fil- og IP-visningene.</span><span class="sxs-lookup"><span data-stu-id="1d939-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="1d939-120">Velg **Behandle koder** fra raden med svarhandlinger.</span><span class="sxs-lookup"><span data-stu-id="1d939-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="1d939-121">Skriv inn for å finne eller opprette koder.</span><span class="sxs-lookup"><span data-stu-id="1d939-121">Type to find or create tags.</span></span>

<span data-ttu-id="1d939-122">Koder legges til i enhetsvisningen og gjenspeiles i Enhetsliste-visningen.</span><span class="sxs-lookup"><span data-stu-id="1d939-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="1d939-123">Du kan deretter bruke Koder-filteret til å se den relevante listen over enheter.</span><span class="sxs-lookup"><span data-stu-id="1d939-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="1d939-124">Hvis du vil ha mer informasjon, [kan du se Opprette og behandle enhetskoder](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="1d939-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>