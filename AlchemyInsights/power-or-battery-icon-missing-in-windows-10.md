---
title: Strøm- eller batteriikon mangler i Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790557"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="4b1ef-102">Strøm- eller batteriikon mangler i Windows 10</span><span class="sxs-lookup"><span data-stu-id="4b1ef-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="4b1ef-103">Hvis Windows 10-enheten har et batteri (f.eks. en bærbar datamaskin eller et nettbrett eller en PC som er koblet via USB til en UPS), vises vanligvis et strøm/batteri-ikon på oppgavelinjen nær klokken, for eksempel:</span><span class="sxs-lookup"><span data-stu-id="4b1ef-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Batteriikon](media/battery-icon.png)

<span data-ttu-id="4b1ef-105">Hvis du ikke ser dette ikonet, kan det være skjult:</span><span class="sxs-lookup"><span data-stu-id="4b1ef-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="4b1ef-106">Gå til **[Innstillinger > Personalisering > Oppgavelinje](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="4b1ef-107">I Systemstatusfeltet klikker du på **Velg hvilke ikoner som skal vises på oppgavelinjen**.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="4b1ef-108">Finn deretter **Power**-elementet i listen, og veksle innstillingen til **På**.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Vis strømikonet i oppgavelinjen](media/power-icon-on.png)

<span data-ttu-id="4b1ef-110">**Feilsøking**</span><span class="sxs-lookup"><span data-stu-id="4b1ef-110">**Troubleshooting**</span></span>

<span data-ttu-id="4b1ef-111">Hvis du har fulgt instruksjonene over og **Power**-veksleknappen er nedtonet eller ikke synlig, skriver du inn **Enhetsbehandling** i søkeboksen på oppgavelinjen, og deretter velger du **Enhetsbehandling** i listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="4b1ef-112">Under **Batterier** høyreklikker du på batteriet for enheten og klikker på **Deaktivere**, og klikker på **Ja**.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="4b1ef-113">Vent noen sekunder og høyreklikk deretter på batteriet og klikk **Aktivere**.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="4b1ef-114">Start deretter enheten på nytt.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-114">Then restart your device.</span></span>

<span data-ttu-id="4b1ef-115">Hvis du har fulgt instruksjonene over, men batteriikonet ikke vises på oppgavelinjen, skriver du inn **oppgavebehandling** i søkeboksen på oppgavelinjen, og klikker deretter **Oppgavebehandling** i listen over resultater.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="4b1ef-116">Gå til **Prosesser** -fanen under **Navn**, høyreklikk på **Explorer**, og klikk deretter på **Start**.</span><span class="sxs-lookup"><span data-stu-id="4b1ef-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
