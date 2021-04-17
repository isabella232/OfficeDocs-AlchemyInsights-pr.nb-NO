---
title: Oppstartsinnstillinger i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828161"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="b8677-102">Oppstartsinnstillinger i Windows 10</span><span class="sxs-lookup"><span data-stu-id="b8677-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="b8677-103">**Endre hvilke apper som kjører automatisk ved oppstart**</span><span class="sxs-lookup"><span data-stu-id="b8677-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="b8677-104">Gå til [Innstillinger > Apper > Oppstart](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="b8677-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="b8677-105">Kontroller at alle apper du vil kjøre ved oppstart, er **slått på**.</span><span class="sxs-lookup"><span data-stu-id="b8677-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="b8677-106">**Legge til en app som skal kjøres automatisk ved oppstart**</span><span class="sxs-lookup"><span data-stu-id="b8677-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="b8677-107">Klikk eller trykk **Start,** og finn appen du vil kjøre ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="b8677-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="b8677-108">Høyreklikk appen, klikk **Mer**, og klikk deretter **Åpne filplassering**.</span><span class="sxs-lookup"><span data-stu-id="b8677-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="b8677-109">Dette åpner plasseringen der snarveien til appen er lagret.</span><span class="sxs-lookup"><span data-stu-id="b8677-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="b8677-110">Hvis det ikke er noe alternativ for Åpne filplassering, betyr det at appen ikke kan kjøre ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="b8677-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="b8677-111">Når filplasseringen er åpen, trykker du **Windows-logotasten + R,** skriver **inn skall:oppstart** og klikker **deretter OK**.</span><span class="sxs-lookup"><span data-stu-id="b8677-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="b8677-112">Dette åpner Oppstart-mappen.</span><span class="sxs-lookup"><span data-stu-id="b8677-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="b8677-113">Kopier og lim inn snarveien til appen fra filplasseringen til Oppstart-mappen.</span><span class="sxs-lookup"><span data-stu-id="b8677-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="b8677-114">**Avanserte oppstartsalternativer (inkludert sikkermodus, UEFI-innstillinger og oppstart fra en annen enhet)**</span><span class="sxs-lookup"><span data-stu-id="b8677-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="b8677-115">Lagre arbeidet og lukk alle åpne dokumenter, siden disse trinnene starter PC-en på nytt.</span><span class="sxs-lookup"><span data-stu-id="b8677-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="b8677-116">Gå til [Innstillinger > Oppdatering & Sikkerhets-> gjenoppretting](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="b8677-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="b8677-117">Klikk **Start på nytt** nå under Avansert **oppstart**.</span><span class="sxs-lookup"><span data-stu-id="b8677-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="b8677-118">Når PC-en har startet på nytt, går du til skjermbildet Velg et alternativ:</span><span class="sxs-lookup"><span data-stu-id="b8677-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="b8677-119">Hvis du vil starte opp fra en enhet som en USB-stasjon, klikker **du Bruk en enhet**.</span><span class="sxs-lookup"><span data-stu-id="b8677-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="b8677-120">Hvis du vil angi UEFI-innstillingene (også kalt BIOS-oppsett), klikker du Feilsøk > Avanserte alternativer > **UEFI-fastvareinnstillinger**.</span><span class="sxs-lookup"><span data-stu-id="b8677-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="b8677-121">Hvis du vil angi sikkermodus eller endre avanserte oppstartsinnstillinger, klikker du **Feilsøk**> Avanserte alternativer > Oppstartsinnstillinger og deretter Start **på nytt.**</span><span class="sxs-lookup"><span data-stu-id="b8677-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="b8677-122">Du kan bli bedt om å angi [BitLocker-gjenopprettingsnøkkelen.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="b8677-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="b8677-123">Når PC-en starter på nytt, klikker du oppstartsinnstillingen du vil bruke.</span><span class="sxs-lookup"><span data-stu-id="b8677-123">After your PC restarts again, click the startup setting you want to use.</span></span>