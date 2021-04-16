---
title: Reparere Microsoft 365-appene Kontoen din er i en melding om dårlig tilstand
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812545"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="d3b3f-102">Feilmeldingen «Kontoen din er i dårlig tilstand» for å løse Microsoft 365-appene</span><span class="sxs-lookup"><span data-stu-id="d3b3f-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="d3b3f-103">Hvis du vil løse denne feilen, kan du prøve følgende alternativer på den berørte datamaskinen:</span><span class="sxs-lookup"><span data-stu-id="d3b3f-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="d3b3f-104">Åpne en Office-app, og **velg Logg** av  >    >  **filkonto av alle kontoer.**</span><span class="sxs-lookup"><span data-stu-id="d3b3f-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="d3b3f-105">Logg på igjen med en brukerkonto med en gyldig lisens.</span><span class="sxs-lookup"><span data-stu-id="d3b3f-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="d3b3f-106">Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="d3b3f-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d3b3f-107">[Fjern Office-legitimasjon ved hjelp](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) av Windows Legitimasjonsbehandling.</span><span class="sxs-lookup"><span data-stu-id="d3b3f-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="d3b3f-108">**Obs!** Registerbanene for Office 2016 er endret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="d3b3f-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d3b3f-109">Eksempel: \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="d3b3f-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="d3b3f-110">Hvis feilen oppstår mens du kobler til Office 365 ved hjelp av Office 2013, aktiverer [du moderne godkjenning](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="d3b3f-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="d3b3f-111">Hvis du vil ha mer informasjon, kan du se Feilsøke apper uten nettlesere som ikke kan logge på [Microsoft 365, Azure eller Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="d3b3f-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

