---
title: Bruke alternativet for å låse opp finger i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795253"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="111b9-102">Bruke alternativet for å låse opp finger i Windows 10</span><span class="sxs-lookup"><span data-stu-id="111b9-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="111b9-103">**Aktiver finger avtrykk for Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="111b9-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="111b9-104">Hvis du vil låse opp Windows 10 ved hjelp av finger avtrykket, må du konfigurere Windows Hello-finger avtrykk ved å legge til (slik at Windows lærer å gjenkjenne) minst én finger.</span><span class="sxs-lookup"><span data-stu-id="111b9-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="111b9-105">Gå til **innstillinger > kontoer > påloggings alternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="111b9-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="111b9-106">Tilgjengelige påloggings alternativer vil være oppført.</span><span class="sxs-lookup"><span data-stu-id="111b9-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="111b9-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="111b9-107">For example:</span></span>

    ![Påloggings alternativer.](media/sign-in-options.png)

2. <span data-ttu-id="111b9-109">Klikk eller trykk **Windows Hello-fingerprint**, og klikk deretter **Konfigurer**.</span><span class="sxs-lookup"><span data-stu-id="111b9-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="111b9-110">I vinduet Windows Hello-oppsett klikker du på **kom i gang**.</span><span class="sxs-lookup"><span data-stu-id="111b9-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="111b9-111">Finger avtrykk sensoren vil aktivere, og du blir bedt om å plassere fingeren på sensoren:</span><span class="sxs-lookup"><span data-stu-id="111b9-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Finger avtrykk sensoren.](media/fingerprint-sensor.png)

3. <span data-ttu-id="111b9-113">Følg instruksjonene, noe som vil be deg om å skanne fingeren din gjentatte ganger.</span><span class="sxs-lookup"><span data-stu-id="111b9-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="111b9-114">Når dette er fullført, har du muligheten til å legge til andre fingre som du kanskje vil bruke til å logge på.</span><span class="sxs-lookup"><span data-stu-id="111b9-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="111b9-115">Neste gang du logger deg på Windows 10, kan du velge å bruke finger avtrykk til å gjøre det.</span><span class="sxs-lookup"><span data-stu-id="111b9-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="111b9-116">**Windows Hello-fingerprint ikke tilgjengelig som et påloggings alternativ**</span><span class="sxs-lookup"><span data-stu-id="111b9-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="111b9-117">Hvis Windows Hello-finger avtrykk ikke vises som et alternativ i **påloggings alternativer**, betyr det at Windows ikke er klar over finger avtrykks leser/skanner som er koblet til data maskinen, eller at en system policy hindrer bruk (Hvis for eksempel data maskinen administreres av arbeids plassen din).</span><span class="sxs-lookup"><span data-stu-id="111b9-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="111b9-118">Slik feil søker du:</span><span class="sxs-lookup"><span data-stu-id="111b9-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="111b9-119">Velg **Start** -knappen på oppgave linjen, og søk etter **enhets behandling**.</span><span class="sxs-lookup"><span data-stu-id="111b9-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="111b9-120">Klikk eller trykk for å åpne **enhets behandling**.</span><span class="sxs-lookup"><span data-stu-id="111b9-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="111b9-121">Utvid Biometriske enheter i enhets behandling ved å klikke vinkel tegnet.</span><span class="sxs-lookup"><span data-stu-id="111b9-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriske enheter.](media/biometric-devices.png)

4. <span data-ttu-id="111b9-123">Finger avtrykks skanneren skal være oppført som en biometrisk enhet, for eksempel Synaptics WBDI-skanneren:</span><span class="sxs-lookup"><span data-stu-id="111b9-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriske enheter.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="111b9-125">Hvis finger avtrykks skanneren ikke vises, og skanneren er integrert i PC-en, kan du gå til PC-produsentens nettsted.</span><span class="sxs-lookup"><span data-stu-id="111b9-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="111b9-126">Søk etter en Windows 10-driver for en skanner du kan installere, i delen teknisk støtte for din PC-modell.</span><span class="sxs-lookup"><span data-stu-id="111b9-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="111b9-127">Hvis skanneren er atskilt fra PC-en (tilknyttet via USB), kan du gå til skanner produsentens nettsted for å finne og installere Windows 10 enhets driver program vare for skanner modellen du har.</span><span class="sxs-lookup"><span data-stu-id="111b9-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
