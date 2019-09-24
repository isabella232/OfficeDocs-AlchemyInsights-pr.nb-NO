---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123007"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6fbe4-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="6fbe4-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6fbe4-103">Arbeide med PowerShell eller skript i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="6fbe4-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6fbe4-104">Gå til linkene nedenfor for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="6fbe4-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6fbe4-105">Komme i gang med SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="6fbe4-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6fbe4-106">Koble til SPO PowerShell med multifaktor godkjenning (MFA)</span><span class="sxs-lookup"><span data-stu-id="6fbe4-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6fbe4-107">[SharePoint-mønstre og-fremgangsmåter (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) inneholder et bibliotek med PowerShell-kommandoer som gjør det mulig å utføre kompliserte administrasjons handlinger mot SPO.</span><span class="sxs-lookup"><span data-stu-id="6fbe4-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6fbe4-108">Hvis du har problemer med å koble med SPO Management Shell, må du kontrollere at du har oppdatert til den nyeste versjonen, og prøv å [importere modulen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) ved hjelp av *"import-modul Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="6fbe4-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6fbe4-109">Hvis du prøver å kjøre klientside objektmodell skript, må du ha [SharePoint Online Client komponenter SDK](https://www.microsoft.com/download/details.aspx?id=42038) installert på din lokale maskin.</span><span class="sxs-lookup"><span data-stu-id="6fbe4-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6fbe4-110">Hvis du har problemer som kjører skript fra PowerShell, bør du vurdere å kjøre PowerShell som administrator og endre [policyen for kjøring av policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="6fbe4-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>