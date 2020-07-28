---
title: Fjerne data og tørke enheter fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440460"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="a107d-102">Fjerne data og tørke enheter fra Intune</span><span class="sxs-lookup"><span data-stu-id="a107d-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="a107d-103">Eksterne handlinger for enhetssletting og enhetssletting kan brukes til å fjerne firmadata som administreres av Intune, eller til å utføre en tilbakestilling til fabrikkinnstillingene og returnere enheten til standardinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="a107d-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="a107d-104">Logg på Microsoft 365 Device Management, og gå til **Enheter**  >  **alle enheter**.</span><span class="sxs-lookup"><span data-stu-id="a107d-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="a107d-105">Velg enheten du vil tørke av.</span><span class="sxs-lookup"><span data-stu-id="a107d-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="a107d-106">Velg typen ekstern sletting du vil gjøre.</span><span class="sxs-lookup"><span data-stu-id="a107d-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="a107d-107">Avslutt sletter bare organisasjonsinformasjon, mens fullstendige slettinger gjenoppretter enheten til fabrikkinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="a107d-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="a107d-108">Velg **Ja** for å bekrefte.</span><span class="sxs-lookup"><span data-stu-id="a107d-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="a107d-109">Til slettingen er ferdig, vises handlingsstatusen Enhet som Pensjonere venter.</span><span class="sxs-lookup"><span data-stu-id="a107d-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="a107d-110">Når handlingen er fullført, ser du ikke lenger mobilenheten i listen over administrerte enheter.</span><span class="sxs-lookup"><span data-stu-id="a107d-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="a107d-111">**Merk at** Firmadata kan ikke fjernes fra enheter som er KOBLET til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a107d-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="a107d-112">Hvis du vil ha mer informasjon om effekten av handlingene Trekk tilbake og tørk, inkludert hva som beholdes og hva som slettes, kan du se [Fjerne enheter ved hjelp av tørk, trekk ut eller rulle ut enheten manuelt](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="a107d-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="a107d-113">Hvis du vil slette alle data fra en macOS-enhet, kan du se [Slette alle data fra en macOS-enhet](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="a107d-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>