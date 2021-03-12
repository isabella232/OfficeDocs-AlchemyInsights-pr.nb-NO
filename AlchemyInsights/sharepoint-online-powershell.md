---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709079"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="fe93f-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="fe93f-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="fe93f-103">Arbeider du med PowerShell eller skript i Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="fe93f-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="fe93f-104">Gå til koblingene nedenfor hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="fe93f-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="fe93f-105">Komme i gang med SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="fe93f-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="fe93f-106">Koble til SPO PowerShell med godkjenning med flere faktorer (MFA)</span><span class="sxs-lookup"><span data-stu-id="fe93f-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="fe93f-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) inneholder et bibliotek med PowerShell-kommandoer som lar deg utføre komplekse administrasjonshandlinger mot SPO.</span><span class="sxs-lookup"><span data-stu-id="fe93f-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="fe93f-108">Hvis du har problemer med å koble til skallet for administrasjon av SPO, må du kontrollere at du har oppdatert til den nyeste versjonen, og prøve å importere modulen på nytt ved hjelp av *«Import-Module Microsoft.Online.SharePoint.PowerShell».* [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)</span><span class="sxs-lookup"><span data-stu-id="fe93f-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="fe93f-109">Hvis du prøver å kjøre skript for objektmodeller i klientsiden, må du ha SDK for [Sharepoint Online Client Components](https://www.microsoft.com/download/details.aspx?id=42038) installert på den lokale maskinen.</span><span class="sxs-lookup"><span data-stu-id="fe93f-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="fe93f-110">Hvis du har problemer med å kjøre skript fra PowerShell, bør du vurdere å kjøre PowerShell som administrator og endre [kjøringspolicyen.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="fe93f-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>