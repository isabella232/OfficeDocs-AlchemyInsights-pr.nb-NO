---
title: Bruke alternativet for fingeravtrykksopplåsing i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796686"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="006b3-102">Bruke alternativet for fingeravtrykksopplåsing i Windows 10</span><span class="sxs-lookup"><span data-stu-id="006b3-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="006b3-103">**Aktivere Windows Hello-fingeravtrykk**</span><span class="sxs-lookup"><span data-stu-id="006b3-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="006b3-104">Hvis du vil låse opp Windows 10 ved hjelp av fingeravtrykk, må du konfigurere Windows Hello-fingeravtrykk ved å legge til (la Windows lære å gjenkjenne) minst én finger.</span><span class="sxs-lookup"><span data-stu-id="006b3-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="006b3-105">Gå til **Innstillinger > kontoer > påloggingsalternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="006b3-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="006b3-106">Tilgjengelige påloggingsalternativer vises.</span><span class="sxs-lookup"><span data-stu-id="006b3-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="006b3-107">For eksempel,</span><span class="sxs-lookup"><span data-stu-id="006b3-107">For example:</span></span>

    ![Påloggingsalternativer.](media/sign-in-options.png)

2. <span data-ttu-id="006b3-109">Klikk eller trykk **Windows Hello Fingeravtrykk**, og klikk deretter **Konfigurer**.</span><span class="sxs-lookup"><span data-stu-id="006b3-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="006b3-110">Klikk Kom i gang i installasjonsvinduet **for** Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="006b3-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="006b3-111">Fingeravtrykkssensoren aktiveres, og du blir bedt om å plassere fingeren på sensoren:</span><span class="sxs-lookup"><span data-stu-id="006b3-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Fingeravtrykkssensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="006b3-113">Følg instruksjonene, som vil be deg om å skanne fingeren gjentatte ganger.</span><span class="sxs-lookup"><span data-stu-id="006b3-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="006b3-114">Når dette er fullført, kan du legge til andre fingre som du kanskje vil bruke til pålogging.</span><span class="sxs-lookup"><span data-stu-id="006b3-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="006b3-115">Neste gang du logger på Windows 10, kan du bruke fingeravtrykket til å gjøre dette.</span><span class="sxs-lookup"><span data-stu-id="006b3-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="006b3-116">**Windows Hello Fingerprint er ikke tilgjengelig som et påloggingsalternativ**</span><span class="sxs-lookup"><span data-stu-id="006b3-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="006b3-117">Hvis Windows Hello Fingerprint ikke vises som et alternativ i Påloggingsalternativer , betyr det at Windows ikke er klar over fingeravtrykksleseren/skanneren som er koblet til PC-en, eller at en systempolicy hindrer bruken (hvis for eksempel **PC-en** administreres av arbeidsplassen).</span><span class="sxs-lookup"><span data-stu-id="006b3-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="006b3-118">Slik feilsøker du:</span><span class="sxs-lookup"><span data-stu-id="006b3-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="006b3-119">Velg **Start-knappen** på oppgavelinjen, og søk etter **Enhetsbehandling**.</span><span class="sxs-lookup"><span data-stu-id="006b3-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="006b3-120">Klikk eller trykk for å åpne **Enhetsbehandling**.</span><span class="sxs-lookup"><span data-stu-id="006b3-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="006b3-121">Utvid Biometriske enheter i Enhetsbehandling ved å klikke vinkeltegn.</span><span class="sxs-lookup"><span data-stu-id="006b3-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriske enheter.](media/biometric-devices.png)

4. <span data-ttu-id="006b3-123">Fingeravtrykksskanneren skal være oppført som en biometrisk enhet, for eksempel Synaptics WBDI-skanner:</span><span class="sxs-lookup"><span data-stu-id="006b3-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriske enheter.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="006b3-125">Hvis fingeravtrykksskanneren ikke vises, og skanneren er integrert i PC-en, går du til nettstedet til PC-produsenten.</span><span class="sxs-lookup"><span data-stu-id="006b3-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="006b3-126">Søk etter en Windows 10-driver for en skanner du kan installere, i delen teknisk støtte for PC-modellen.</span><span class="sxs-lookup"><span data-stu-id="006b3-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="006b3-127">Hvis skanneren er atskilt fra PC-en (koblet til via USB), kan du gå til nettstedet til skannerprodusenten for å finne og installere enhetsdriverprogramvaren for Windows 10 for skannermodellen du har.</span><span class="sxs-lookup"><span data-stu-id="006b3-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
