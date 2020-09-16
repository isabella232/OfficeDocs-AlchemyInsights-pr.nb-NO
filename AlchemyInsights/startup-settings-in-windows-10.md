---
title: Oppstarts innstillinger i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751144"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="63a3a-102">Oppstarts innstillinger i Windows 10</span><span class="sxs-lookup"><span data-stu-id="63a3a-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="63a3a-103">**Endre hvilke apper som kjører automatisk ved oppstart**</span><span class="sxs-lookup"><span data-stu-id="63a3a-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="63a3a-104">Gå til [innstillinger > apper > oppstart](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="63a3a-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="63a3a-105">Kontroller at appen du vil kjøre ved oppstart, er slått **på**.</span><span class="sxs-lookup"><span data-stu-id="63a3a-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="63a3a-106">**Legge til en app som skal kjøres automatisk ved oppstart**</span><span class="sxs-lookup"><span data-stu-id="63a3a-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="63a3a-107">Klikk eller trykk **Start** , og Finn appen du vil kjøre ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="63a3a-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="63a3a-108">Høyre klikk appen, klikk **mer**, og klikk deretter **Åpne fil plassering**.</span><span class="sxs-lookup"><span data-stu-id="63a3a-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="63a3a-109">Dette åpner plasseringen der snarveien til appen er lagret.</span><span class="sxs-lookup"><span data-stu-id="63a3a-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="63a3a-110">Hvis det ikke er noe alternativ for å åpne fil plasseringen, betyr det at appen ikke kan kjøre ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="63a3a-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="63a3a-111">Med fil plasseringen åpen trykker du Windows- **logotasten + R**, skriver inn **Shell: oppstart**, og deretter klikker du **OK**.</span><span class="sxs-lookup"><span data-stu-id="63a3a-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="63a3a-112">Dette åpner oppstarts mappen.</span><span class="sxs-lookup"><span data-stu-id="63a3a-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="63a3a-113">Kopier og lim inn snarveien til appen fra fil plasseringen til oppstarts mappen.</span><span class="sxs-lookup"><span data-stu-id="63a3a-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="63a3a-114">**Avanserte oppstarts alternativer (inkludert sikker modus, UEFI-innstillinger og oppstart fra en annen enhet)**</span><span class="sxs-lookup"><span data-stu-id="63a3a-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="63a3a-115">Lagre arbeidet ditt, og lukk eventuelle åpne dokumenter, siden disse trinnene vil starte data maskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="63a3a-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="63a3a-116">Gå til [innstillinger > oppdater & sikkerhets > gjenoppretting](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="63a3a-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="63a3a-117">Klikk **Start på nytt nå**under **Avansert oppstart**.</span><span class="sxs-lookup"><span data-stu-id="63a3a-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="63a3a-118">Når PC-en starter på nytt i Velg et alternativ-skjerm bilde:</span><span class="sxs-lookup"><span data-stu-id="63a3a-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="63a3a-119">Hvis du vil starte fra en enhet som en USB-stasjon, klikker du **Bruk en enhet**.</span><span class="sxs-lookup"><span data-stu-id="63a3a-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="63a3a-120">Hvis du vil angi UEFI-innstillingene (noen ganger kalt BIOS-konfigurasjon), klikker du **feil søking > avanserte alternativer > innstillinger for UEFI-fastvare**.</span><span class="sxs-lookup"><span data-stu-id="63a3a-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="63a3a-121">Hvis du vil angi sikker modus eller endre avanserte oppstarts innstillinger, klikker du **feilsøk > avanserte alternativer > oppstarts innstillinger**, og deretter klikker du **Start på nytt**.</span><span class="sxs-lookup"><span data-stu-id="63a3a-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="63a3a-122">Du kan bli bedt om å angi [gjenopprettings nøkkelen for BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="63a3a-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="63a3a-123">Når PC-en starter på nytt, klikker du på oppstarts innstillingen du vil bruke.</span><span class="sxs-lookup"><span data-stu-id="63a3a-123">After your PC restarts again, click the startup setting you want to use.</span></span>