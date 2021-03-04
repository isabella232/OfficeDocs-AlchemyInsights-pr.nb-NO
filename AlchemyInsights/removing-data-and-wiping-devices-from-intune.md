---
title: Fjerne data og sletteenheter fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416322"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="e5821-102">Fjerne data og sletteenheter fra Intune</span><span class="sxs-lookup"><span data-stu-id="e5821-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="e5821-103">Eksterne handlinger for fjerning av enheter og enhetsutsletting kan brukes til å fjerne firmadata som administreres av Intune, eller til å utføre tilbakestilling til fabrikkinnstillinger og returnere enheten til standardinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="e5821-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="e5821-104">Logg på Microsoft 365 Device Management, og gå til **Enheter** > **Alle enheter**.</span><span class="sxs-lookup"><span data-stu-id="e5821-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="e5821-105">Velg enheten du vil fjerne.</span><span class="sxs-lookup"><span data-stu-id="e5821-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="e5821-106">Velg hvilken type ekstern sletting du vil utføre.</span><span class="sxs-lookup"><span data-stu-id="e5821-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="e5821-107">Tilbaketrekking sletter bare organisasjonsinformasjon, mens total sletting gjenoppretter enheten til fabrikkinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="e5821-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="e5821-108">Velg **Ja** for å bekrefte.</span><span class="sxs-lookup"><span data-stu-id="e5821-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="e5821-109">Inntil slettingen er ferdig, vises Enhetens handlingsstatus som *Tilbaketrekking venter*.</span><span class="sxs-lookup"><span data-stu-id="e5821-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="e5821-110">Når handlingen er fullført, ser du ikke lenger den mobile enheten i listen over administrerte enheter.</span><span class="sxs-lookup"><span data-stu-id="e5821-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="e5821-111">Firmadata kan ikke fjernes fra enheter SOM ER KOBLET TIL Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5821-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="e5821-112">Hvis du vil ha detaljert informasjon om effekten av handlingene Tilbaketrekking og Sletting, inkludert hva som beholdes og hva som slettes, kan du se følgende dokumentasjon:</span><span class="sxs-lookup"><span data-stu-id="e5821-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="e5821-113">[Fjern enheter ved hjelp av sletting, fjerning eller manuell avregistrering av enheten](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="e5821-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="e5821-114">Slik sletter du bare bedriftsdata fra Intune-administrerte apper</span><span class="sxs-lookup"><span data-stu-id="e5821-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="e5821-115">[Slett alle data fra en macOS-enhet](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="e5821-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>