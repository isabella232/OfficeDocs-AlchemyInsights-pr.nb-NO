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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938286"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="2a2e7-102">Problemer med pålogging til Office-programmer</span><span class="sxs-lookup"><span data-stu-id="2a2e7-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="2a2e7-103">Hvis du vil rette påloggingsproblemer med Office-programmer, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="2a2e7-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="2a2e7-104">Fjern alle arbeid-kontoer, bortsett fra den berørte kontoen, ved hjelp av Windows-innstillinger > **Access arbeid eller skole**.</span><span class="sxs-lookup"><span data-stu-id="2a2e7-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="2a2e7-105">[Fjern Office legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjoner.</span><span class="sxs-lookup"><span data-stu-id="2a2e7-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2a2e7-106">**Merk:** Registerbaner for Office-2016 har endret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="2a2e7-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2a2e7-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2a2e7-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="2a2e7-108">Et Office-program, velger du **fil** > **konto** > **Logg av**. Deretter kan du logge inn med en brukerkonto med en gyldig lisens.</span><span class="sxs-lookup"><span data-stu-id="2a2e7-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="2a2e7-109">Hvis du vil ha mer informasjon, se [kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="2a2e7-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="2a2e7-110">For Mac, kan du se [en Office-2016 for Mac app kan ikke logge på](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="2a2e7-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="2a2e7-111">Hvis det oppstår en feil under tilkobling til Office 365 ved hjelp av Office-2013, aktivere moderne godkjenning for Office-klient.</span><span class="sxs-lookup"><span data-stu-id="2a2e7-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="2a2e7-112">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="2a2e7-112">For more information, see:</span></span>
- [<span data-ttu-id="2a2e7-113">Du kan ikke logge på Office 365, Azure eller Intune</span><span class="sxs-lookup"><span data-stu-id="2a2e7-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="2a2e7-114">Tilkoblingsproblemer i pålogging etter oppdatering til Office-2016 bygge 16.0.7967 på 10 for Windows</span><span class="sxs-lookup"><span data-stu-id="2a2e7-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="2a2e7-115">"Beklager, en annen konto fra organisasjonen er allerede logget på denne datamaskinen" i Office</span><span class="sxs-lookup"><span data-stu-id="2a2e7-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="2a2e7-116">Feilsøke påloggingsproblemer med moderne Office-godkjenning når du bruker ADFS</span><span class="sxs-lookup"><span data-stu-id="2a2e7-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)