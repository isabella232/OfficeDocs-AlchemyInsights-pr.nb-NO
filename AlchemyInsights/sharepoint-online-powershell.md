---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764270"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="60619-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="60619-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="60619-103">Arbeide med PowerShell eller skript i Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="60619-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="60619-104">Gå til linkene nedenfor for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="60619-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="60619-105">Komme i gang med SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="60619-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="60619-106">Koble til SPO PowerShell med multifaktorautentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="60619-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="60619-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) inneholder et bibliotek med PowerShell-kommandoer som lar deg utføre komplekse administrasjonshandlinger mot SPO.</span><span class="sxs-lookup"><span data-stu-id="60619-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="60619-108">Hvis du har problemer med å koble til SPO management shell, må du kontrollere at du har oppdatert til den nyeste versjonen og prøve å [importere modulen på nytt](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) ved hjelp av *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="60619-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="60619-109">Hvis du prøver å kjøre objektmodellskript på klientsiden, må du ha [SDK-en for Sharepoint Online-klientkomponenter](https://www.microsoft.com/download/details.aspx?id=42038) installert på den lokale maskinen.</span><span class="sxs-lookup"><span data-stu-id="60619-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="60619-110">Hvis du har problemer med å kjøre skript fra PowerShell, kan det være lurt å vurdere å kjøre PowerShell som administrator og endre [kjøringspolicyen](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="60619-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>