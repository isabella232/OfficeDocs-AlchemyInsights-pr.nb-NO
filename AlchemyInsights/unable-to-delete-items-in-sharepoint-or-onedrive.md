---
title: Kan ikke slette elementer i SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057748"
---
# <a name="unable-to-delete-items"></a>Kan ikke slette elementer

Har du problemer med elementer slettes?

- Kontroller alltid at du har [riktige tillatelser](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) til å slette elementet eller har en [administrator for områdesamling](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) forsøk på fjerne elementet.

- Kontroller at det ikke er et oppsett for [oppbevaringspolicy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) på varen.

- Kontroller at elementet ikke er [sjekket ut](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.

- Til slutt, kan administratorer bruke [SharePoint mønstre og praksiser](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som inneholder et bibliotek med PowerShell kommandoer som gjør det mulig å utføre komplekse management handlinger som tvinger sletting av stubborn elementer. 
- [Fjern PNP-fil](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjern PNP listeelement](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-listen](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjern PNP-felt (kolonne)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)