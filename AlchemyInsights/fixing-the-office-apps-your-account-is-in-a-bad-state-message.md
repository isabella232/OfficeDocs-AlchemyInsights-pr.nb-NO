---
title: Fikse Office-apper kontoen din er i en feilmelding
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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969649"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="e916f-102">Fikse Office-appene "Kontoen din er i en dårlig tilstand" feil</span><span class="sxs-lookup"><span data-stu-id="e916f-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="e916f-103">Hvis du vil løse denne feilen, kan du prøve følgende alternativer på den berørte datamaskinen:</span><span class="sxs-lookup"><span data-stu-id="e916f-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="e916f-104">Åpne en Office-app, velg Logg**av** **filkonto** > \*\*\*\* > for alle kontoer .</span><span class="sxs-lookup"><span data-stu-id="e916f-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="e916f-105">Logg på igjen ved hjelp av en brukerkonto med en gyldig lisens.</span><span class="sxs-lookup"><span data-stu-id="e916f-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="e916f-106">Hvis du vil ha detaljert informasjon, kan du se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="e916f-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e916f-107">[Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="e916f-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="e916f-108">**Merk:** Registerbanene for Office-2016 er endret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="e916f-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e916f-109">For eksempel \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="e916f-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="e916f-110">På den berørte datamaskinen angir du EnableADAL = 0 ved hjelp av følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="e916f-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="e916f-111">Høyreklikk Windows-knappen, og velg **Kjør**.</span><span class="sxs-lookup"><span data-stu-id="e916f-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="e916f-112">Skriv inn **regedit**i **Åpne-boksen,** og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="e916f-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="e916f-113">Velg **Ja** når du blir bedt om å la Registerredigering gjøre endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="e916f-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="e916f-114">I Registerredigering legger du til en DWORD-verdi for EnableADAL med en innstilling på 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="e916f-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="e916f-115">Hvis feilen oppstår under tilkobling til Office 365 ved hjelp av Office-2013, [aktiverer du moderne godkjenning](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for Office-klienten.</span><span class="sxs-lookup"><span data-stu-id="e916f-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="e916f-116">Hvis du vil ha mer informasjon, kan du se Feilsøke apper som [ikke er i nettleseren, som ikke kan logge på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="e916f-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

