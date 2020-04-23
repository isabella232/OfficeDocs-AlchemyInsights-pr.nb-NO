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
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Arbeide med PowerShell eller skript i Sharepoint Online? Gå til linkene nedenfor for mer informasjon.
- [Komme i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Koble til SPO PowerShell med multifaktorautentisering (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) inneholder et bibliotek med PowerShell-kommandoer som lar deg utføre komplekse administrasjonshandlinger mot SPO.

> [!NOTE]
> - Hvis du har problemer med å koble til SPO management shell, må du kontrollere at du har oppdatert til den nyeste versjonen og prøve å [importere modulen på nytt](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) ved hjelp av *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Hvis du prøver å kjøre objektmodellskript på klientsiden, må du ha [SDK-en for Sharepoint Online-klientkomponenter](https://www.microsoft.com/download/details.aspx?id=42038) installert på den lokale maskinen.
> - Hvis du har problemer med å kjøre skript fra PowerShell, kan det være lurt å vurdere å kjøre PowerShell som administrator og endre [kjøringspolicyen](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).