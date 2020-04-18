---
title: Fikse Office-appene Kontoen din er i en dårlig tilstandsmelding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: b28865ff1da434a254c9051183074be35cdd0252
ms.sourcegitcommit: 9b2b162ad651e2c3d9d0c746f67a78334592f076
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/17/2020
ms.locfileid: "43547971"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="fe884-102">Fikse Office-appene "Kontoen din er i dårlig tilstand" feil</span><span class="sxs-lookup"><span data-stu-id="fe884-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="fe884-103">Hvis du vil løse denne feilen, kan du prøve følgende alternativer på den berørte datamaskinen:</span><span class="sxs-lookup"><span data-stu-id="fe884-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="fe884-104">Åpne en Office-app, velg Logg av **filkonto** > **Account** > **for alle kontoer**.</span><span class="sxs-lookup"><span data-stu-id="fe884-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="fe884-105">Logg på igjen med en brukerkonto med en gyldig lisens.</span><span class="sxs-lookup"><span data-stu-id="fe884-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="fe884-106">Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="fe884-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="fe884-107">[Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="fe884-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="fe884-108">**Merk:** Registerbanene for Office-2016 er endret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="fe884-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fe884-109">\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="fe884-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="fe884-110">Hvis feilen oppstår under tilkobling til Office 365 ved hjelp av Office-2013, [aktiverer du moderne godkjenning](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="fe884-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="fe884-111">Hvis du vil ha mer informasjon, kan du se [Feilsøke apper som ikke er nettleserapper som ikke kan logge på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="fe884-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

