---
title: Problemer med å logge på Office-apper
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763010"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="72893-102">Problemer med å logge på Office-apper</span><span class="sxs-lookup"><span data-stu-id="72893-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="72893-103">Prøv følgende for å løse påloggingsproblemer med Office-apper:</span><span class="sxs-lookup"><span data-stu-id="72893-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="72893-104">Fjern alle arbeidskontoer, unntatt den berørte kontoen, ved hjelp av Windows-innstillinger > **Access-jobb eller skole**.</span><span class="sxs-lookup"><span data-stu-id="72893-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="72893-105">[Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="72893-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="72893-106">**Merk:** Registerbanene for Office-2016 er endret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="72893-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="72893-107">(F.eks. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="72893-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="72893-108">Åpne en Office-app, velg Logg**av** > **filkonto** > . **File** Logg deretter på med en brukerkonto med en gyldig lisens.</span><span class="sxs-lookup"><span data-stu-id="72893-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="72893-109">Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="72893-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="72893-110">Hvis du bruker Mac, kan du ta en titt på [Jeg kan ikke logge på en Office 2016 for Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="72893-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="72893-111">Hvis feilene oppstår under tilkobling til Microsoft 365 ved hjelp av Office-2013, aktiverer du moderne godkjenning for Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="72893-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="72893-112">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="72893-112">For more information, see:</span></span>
- [<span data-ttu-id="72893-113">Du kan ikke logge på Microsoft 365, Azure eller Intune</span><span class="sxs-lookup"><span data-stu-id="72893-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="72893-114">Tilkoblingsproblemer i pålogging etter oppdatering til Office-2016 bygge 16.0.7967 på Windows 10</span><span class="sxs-lookup"><span data-stu-id="72893-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="72893-115">"Beklager, en annen konto fra organisasjonen er allerede logget på denne datamaskinen" i Office</span><span class="sxs-lookup"><span data-stu-id="72893-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="72893-116">Feilsøke påloggingsproblemer med moderne Office-godkjenning når du bruker ADFS</span><span class="sxs-lookup"><span data-stu-id="72893-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)