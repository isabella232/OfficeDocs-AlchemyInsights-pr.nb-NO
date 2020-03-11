---
title: Bruke alternativet for opplåsing av fingeravtrykk i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588324"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="c3ab9-102">Bruke alternativet for opplåsing av fingeravtrykk i Windows 10</span><span class="sxs-lookup"><span data-stu-id="c3ab9-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="c3ab9-103">**Aktiver Windows Hello-fingeravtrykk**</span><span class="sxs-lookup"><span data-stu-id="c3ab9-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="c3ab9-104">Hvis du vil låse opp Windows 10 ved hjelp av fingeravtrykket ditt, må du konfigurere Windows Hello Fingerprint ved å legge til (la Windows lære å gjenkjenne) minst én finger.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="c3ab9-105">Gå til **Innstillinger > Kontoer > Påloggingsalternativer** (eller klikk [her).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="c3ab9-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="c3ab9-106">Tilgjengelige påloggingsalternativer vises.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="c3ab9-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="c3ab9-107">For example:</span></span>

    ![Påloggingsalternativer.](media/sign-in-options.png)

2. <span data-ttu-id="c3ab9-109">Klikk eller trykk **Windows Hello Fingeravtrykk**, og klikk deretter **Konfigurer**.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="c3ab9-110">Klikk **Kom i gang**i vinduet Installasjonsprogram for Windows Hello .</span><span class="sxs-lookup"><span data-stu-id="c3ab9-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="c3ab9-111">Fingeravtrykkssensoren aktiveres, og du blir bedt om å plassere fingeren på sensoren:</span><span class="sxs-lookup"><span data-stu-id="c3ab9-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Fingeravtrykkssensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="c3ab9-113">Følg instruksjonene, som vil be deg om å skanne fingeren gjentatte ganger.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="c3ab9-114">Når dette er ferdig, har du muligheten til å legge til andre fingre du kanskje vil bruke til pålogging.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="c3ab9-115">Neste gang du logger på Windows 10, har du muligheten til å bruke fingeravtrykket til å gjøre det.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="c3ab9-116">**Windows Hello Fingeravtrykk er ikke tilgjengelig som påloggingsalternativ**</span><span class="sxs-lookup"><span data-stu-id="c3ab9-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="c3ab9-117">Hvis Windows Hello Fingeravtrykk ikke vises som et alternativ i **påloggingsalternativer**, betyr det at Windows ikke er klar over fingeravtrykksleser/skanner som er koblet til PCen, eller at en systempolicy forhindrer bruk (hvis pCen for eksempel administreres av arbeidsplassen din).</span><span class="sxs-lookup"><span data-stu-id="c3ab9-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="c3ab9-118">Slik feilsøker du:</span><span class="sxs-lookup"><span data-stu-id="c3ab9-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="c3ab9-119">Velg **Start-knappen** på oppgavelinjen, og søk etter **Enhetsbehandling**.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="c3ab9-120">Klikk eller trykk for å åpne **Enhetsbehandling**.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="c3ab9-121">Utvid Biometriske enheter i Enhetsbehandling ved å klikke på vinkeltegnet.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriske enheter.](media/biometric-devices.png)

4. <span data-ttu-id="c3ab9-123">Fingeravtrykkskanneren skal være oppført som en biometrisk enhet, for eksempel Synaptics WBDI-skanneren:</span><span class="sxs-lookup"><span data-stu-id="c3ab9-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriske enheter.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="c3ab9-125">Hvis fingeravtrykkskanneren ikke vises, og skanneren er integrert i PCen, går du til PC-produsentens nettsted.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="c3ab9-126">I delen teknisk støtte for PC-modellen søker du etter en Windows 10-driver etter en skanner du kan installere.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="c3ab9-127">Hvis skanneren er atskilt fra PC-en (tilkoblet via USB), går du til skannerprodusentens nettsted for å finne og installere Windows 10-enhetsdriverprogramvare for skannermodellen du har.</span><span class="sxs-lookup"><span data-stu-id="c3ab9-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
