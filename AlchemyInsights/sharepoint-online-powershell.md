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
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Arbeider du med PowerShell eller skript i Sharepoint Online? Gå til koblingene nedenfor hvis du vil ha mer informasjon.
- [Komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Koble til SPO PowerShell med godkjenning med flere faktorer (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) inneholder et bibliotek med PowerShell-kommandoer som lar deg utføre komplekse administrasjonshandlinger mot SPO.

> [!NOTE]
> - Hvis du har problemer med å koble til skallet for administrasjon av SPO, må du kontrollere at du har oppdatert til den nyeste versjonen, og prøve å importere modulen på nytt ved hjelp av *«Import-Module Microsoft.Online.SharePoint.PowerShell».* [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)
> - Hvis du prøver å kjøre skript for objektmodeller i klientsiden, må du ha SDK for [Sharepoint Online Client Components](https://www.microsoft.com/download/details.aspx?id=42038) installert på den lokale maskinen.
> - Hvis du har problemer med å kjøre skript fra PowerShell, bør du vurdere å kjøre PowerShell som administrator og endre [kjøringspolicyen.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)