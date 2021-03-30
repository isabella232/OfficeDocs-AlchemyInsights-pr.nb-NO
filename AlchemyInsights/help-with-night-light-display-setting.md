---
title: Hjelp med skjerminnstillingen for kveldslys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404667"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="47488-102">Hjelp med skjerminnstillingen for kveldslys</span><span class="sxs-lookup"><span data-stu-id="47488-102">Help with the night light display setting</span></span>

<span data-ttu-id="47488-103">Hvis du vil lære mer om skjerminnstillinger for kveldstid, kan du se Angi [skjerm for kveldstid i Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="47488-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="47488-104">Hvis alternativene for kveldslys er nedtonet i Innstillinger, kontrollerer du skjermdriveren:</span><span class="sxs-lookup"><span data-stu-id="47488-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="47488-105">Klikk søkeboksen på oppgavelinjen, og skriv **inn Enhetsbehandling**, og velg deretter **Enhetsbehandling** i søkeresultatene.</span><span class="sxs-lookup"><span data-stu-id="47488-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="47488-106">Utvid **skjermkort**.</span><span class="sxs-lookup"><span data-stu-id="47488-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="47488-107">Funksjonen for kveldslys er dessverre ikke tilgjengelig hvis enheten bruker en DisplayLink-driver eller en Grunnleggende skjermdriver.</span><span class="sxs-lookup"><span data-stu-id="47488-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="47488-108">Funksjonen for kveldslys bruker nylig grafikkteknologi, så du må kanskje oppdatere skjermdriveren:</span><span class="sxs-lookup"><span data-stu-id="47488-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="47488-109">Se etter oppdateringer ved å gå til **Start**  >  **innstillinger**  >  **Oppdater & Sikkerhetsoppdatering** for  >  **Windows Update**  >  **Se etter oppdateringer**.</span><span class="sxs-lookup"><span data-stu-id="47488-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="47488-110">ELLER</span><span class="sxs-lookup"><span data-stu-id="47488-110">OR</span></span>

- <span data-ttu-id="47488-111">Gå til maskinvareprodusentens støttenettsted for å laste ned og installere de nyeste skjermdriverne manuelt.</span><span class="sxs-lookup"><span data-stu-id="47488-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="47488-112">Tilbakestille kveldslyset i registeret</span><span class="sxs-lookup"><span data-stu-id="47488-112">Reset night light in the registry</span></span>

<span data-ttu-id="47488-113">Hvis oppdatering av skjermdriveren ikke fungerte, må du kanskje tilbakestille kveldslyset i registeret.</span><span class="sxs-lookup"><span data-stu-id="47488-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="47488-114">**Forsiktig:** Dette feilsøkingstrinnet anbefales bare for avanserte brukere.</span><span class="sxs-lookup"><span data-stu-id="47488-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="47488-115">Det kan oppstå alvorlige problemer hvis du endrer registeret feil.</span><span class="sxs-lookup"><span data-stu-id="47488-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="47488-116">For ekstra beskyttelse bør du sikkerhetskopiere registeret før du endrer det, slik at du kan gjenopprette det hvis det oppstår problemer.</span><span class="sxs-lookup"><span data-stu-id="47488-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="47488-117">Skriv inn **regedit** i søkeboksen, og velg deretter **Registerredigering** i søkeresultatene.</span><span class="sxs-lookup"><span data-stu-id="47488-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="47488-118">Gå til følgende registernøkkel:</span><span class="sxs-lookup"><span data-stu-id="47488-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="47488-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="47488-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="47488-120">Eksporter og slett deretter følgende undernøkkel:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="47488-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="47488-121">Eksporter og slett deretter følgende undernøkkel:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="47488-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="47488-122">Start Windows på nytt, og kontroller om alternativene for kveldslys er tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="47488-122">Restart Windows and verify if the night light options are available.</span></span>


