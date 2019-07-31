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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938288"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7eebd-102">Reparerer Office apps "klarerte plattformmodulen (TPM) på datamaskinen ikke fungerer skikkelig" melding</span><span class="sxs-lookup"><span data-stu-id="7eebd-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7eebd-103">Hvis du vil løse dette problemet, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="7eebd-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7eebd-104">Installere de siste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="7eebd-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7eebd-105">[Fjern Office legitimasjon](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjoner.</span><span class="sxs-lookup"><span data-stu-id="7eebd-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7eebd-106">**Merk:** Registerbaner for Office-2016 har endret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="7eebd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7eebd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7eebd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7eebd-108">Prøv [gjenopprettingsprosessen for brukeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for å rette feil for klarert plattformmodul (TPM).</span><span class="sxs-lookup"><span data-stu-id="7eebd-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7eebd-109">Angi EnableADAL = 0 ved å gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="7eebd-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7eebd-110">Høyreklikk startknappen i Windows, velg **Kjør**, Skriv inn **regedit**, og velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="7eebd-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7eebd-111">Velg **Ja** Hvis du vil tillate Registerredigering til å gjøre endringer til enheten.</span><span class="sxs-lookup"><span data-stu-id="7eebd-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7eebd-112">I Registerredigering, legge til DWORD-verdien **EnableADAL** med innstillingen **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="7eebd-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7eebd-113">Hvis du vil ha mer informasjon, kan du se [tilkobling problemer i pålogging etter oppdatering til Office-2016 build 16.0.7967 på 10 for Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="7eebd-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>