---
title: Problemer med pålogging til Office-programmer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938287"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="47111-102">Tom påloggingsbildet i Office-programmer</span><span class="sxs-lookup"><span data-stu-id="47111-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="47111-103">Hvis du vil løse dette problemet, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="47111-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="47111-104">Installere de siste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="47111-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="47111-105">Tilbakestill Internet Explorer-alternativer: Gå til **Verktøy** > **Alternativer for Internett** > **Avansert** > **Tilbakestill Internet Explorer-innstillinger** (Legg merke til at du mister egendefinerte innstillinger), og prøv deretter logger deg på Office på nytt.</span><span class="sxs-lookup"><span data-stu-id="47111-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="47111-106">Deaktiver Windows Defender program Guard (WDAG) eller andre lignende brannmur eller antivirus-programmer:</span><span class="sxs-lookup"><span data-stu-id="47111-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="47111-107">Gå til **programmer**i Kontrollpanel, og velg deretter **Slå Windows-funksjoner på eller av**.</span><span class="sxs-lookup"><span data-stu-id="47111-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="47111-108">Hvis Windows Defender program Guard er aktivert, kan du prøve å deaktivere den.</span><span class="sxs-lookup"><span data-stu-id="47111-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="47111-109">**Merk:** Du må kanskje starte datamaskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="47111-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="47111-110">Kontroller at Microsoft.AAD.BrokerPlugin [AAD WAM-plugin-modulen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke er blokkert av en hvilken som helst program eller brannmur/anti-virus program.</span><span class="sxs-lookup"><span data-stu-id="47111-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="47111-111">[Fjern Office legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjoner.</span><span class="sxs-lookup"><span data-stu-id="47111-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="47111-112">**Merk:** Registerbaner for Office-2016 har endret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="47111-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="47111-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="47111-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="47111-114">Hvis du vil ha mer informasjon, kan du se [tilkobling problemer i pålogging etter oppdatering til Office-2016 build 16.0.7967 på 10 for Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="47111-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>