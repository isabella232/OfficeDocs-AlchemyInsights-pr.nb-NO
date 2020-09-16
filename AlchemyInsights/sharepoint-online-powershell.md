---
title: SharePoint Online PowerShell
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770848"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="4a08a-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="4a08a-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="4a08a-103">Arbeider du med PowerShell eller skript i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="4a08a-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="4a08a-104">Gå til koblingene nedenfor for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="4a08a-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="4a08a-105">Komme i gang med administrasjons konsoll for SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4a08a-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="4a08a-106">Koble deg til SPO PowerShell med godkjenning med mer enn fakultet (MFA)</span><span class="sxs-lookup"><span data-stu-id="4a08a-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="4a08a-107">[SharePoint-mønstre og-rutiner (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) inneholder et bibliotek med PowerShell-kommandoer som gjør at du kan utføre komplekse administrasjons handlinger mot SPO.</span><span class="sxs-lookup"><span data-stu-id="4a08a-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="4a08a-108">Hvis du har problemer med å koble deg til SPO Management Shell, må du sørge for at du har oppdatert til den nyeste versjonen og prøver å [importere modulen på nytt](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) ved hjelp av *«Importer-modul Microsoft. online. SharePoint. PowerShell».*</span><span class="sxs-lookup"><span data-stu-id="4a08a-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="4a08a-109">Hvis du prøver å kjøre objekt modell skript for klient side, må du ha [SDK for SharePoint Online-klienten](https://www.microsoft.com/download/details.aspx?id=42038) installert på den lokale maskinen.</span><span class="sxs-lookup"><span data-stu-id="4a08a-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="4a08a-110">Hvis du har problemer med å kjøre skript fra PowerShell, vil du kanskje vurdere å kjøre PowerShell som administrator og endre [Kjørings policyen](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="4a08a-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>