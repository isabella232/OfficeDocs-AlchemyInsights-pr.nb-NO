---
title: Problemer med å logge på Microsoft 365-apper
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695296"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="fc249-102">Blank påloggings skjerm i Microsoft 365-apper</span><span class="sxs-lookup"><span data-stu-id="fc249-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="fc249-103">Prøv følgende for å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="fc249-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="fc249-104">Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="fc249-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="fc249-105">Tilbakestille alternativer for Internet Explorer: gå til **verktøy**  >  **Alternativer for Internet**t  >  **Avansert**  >  **tilbakestille Internet Explorer-innstillinger** (Vær oppmerksom på at du mister egen definerte innstillinger), og prøv deretter å logge på Office på nytt.</span><span class="sxs-lookup"><span data-stu-id="fc249-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="fc249-106">Deaktiver Windows Defender Application Guard (WDAG) eller et lignende brann mur-eller antivirus program:</span><span class="sxs-lookup"><span data-stu-id="fc249-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="fc249-107">Gå til **programmer**i kontroll panel, og velg deretter **slå Windows-funksjoner på eller av**.</span><span class="sxs-lookup"><span data-stu-id="fc249-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="fc249-108">Hvis Windows Defender Application Guard er aktivert, kan du prøve å deaktivere det.</span><span class="sxs-lookup"><span data-stu-id="fc249-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="fc249-109">**Obs!** Det kan hende du må starte data maskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="fc249-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="fc249-110">Kontroller at plugin-modulen Microsoft. AAD. BrokerPlugin [AAD-WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokkeres av program-eller brann mur-/antivirus program.</span><span class="sxs-lookup"><span data-stu-id="fc249-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="fc249-111">[Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjons behandling.</span><span class="sxs-lookup"><span data-stu-id="fc249-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="fc249-112">**Obs!** Register banene for Office 2016 har blitt endret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="fc249-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fc249-113">(Eks: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="fc249-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="fc249-114">Hvis du vil ha mer informasjon, kan du se [tilkoblings problemer i pålogging etter oppdatering til Office 2016 Bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="fc249-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>