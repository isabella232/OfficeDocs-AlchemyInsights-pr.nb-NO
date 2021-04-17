---
title: Problemer med å logge på Microsoft 365-apper
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833048"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="5d873-102">Tom påloggingsskjerm i Microsoft 365-apper</span><span class="sxs-lookup"><span data-stu-id="5d873-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="5d873-103">Prøv følgende for å løse dette problemet:</span><span class="sxs-lookup"><span data-stu-id="5d873-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="5d873-104">Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="5d873-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="5d873-105">Tilbakestille alternativer for Internet Explorer: Gå til Alternativer for Internett-verktøy Avanserte  >    >    >  **tilbakestillingsinnstillinger** for Internet Explorer (vær oppmerksom på at du mister egendefinerte innstillinger), og prøv deretter å logge på Office på nytt.</span><span class="sxs-lookup"><span data-stu-id="5d873-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="5d873-106">Deaktiver Windows Defender Application Guard (WDAG) eller et lignende brannmur- eller antivirusprogram:</span><span class="sxs-lookup"><span data-stu-id="5d873-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="5d873-107">Gå til Programmer i **Kontrollpanel,** og velg deretter **Aktiver eller deaktiver Windows-funksjoner.**</span><span class="sxs-lookup"><span data-stu-id="5d873-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="5d873-108">Hvis Windows Defender Application Guard er aktivert, kan du prøve å deaktivere den.</span><span class="sxs-lookup"><span data-stu-id="5d873-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="5d873-109">**Obs!** Du må kanskje starte datamaskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="5d873-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="5d873-110">Kontroller at plugin-modulen Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ikke blokkeres av et program eller brannmur/antivirusprogram.</span><span class="sxs-lookup"><span data-stu-id="5d873-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="5d873-111">[Fjern Office-legitimasjon ved hjelp](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) av Windows Legitimasjonsbehandling.</span><span class="sxs-lookup"><span data-stu-id="5d873-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="5d873-112">**Obs!** Registerbanene for Office 2016 er endret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="5d873-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5d873-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="5d873-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="5d873-114">Hvis du vil ha mer informasjon, kan du se Tilkoblingsproblemer ved pålogging etter oppdatering til [Office 2016 bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="5d873-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>