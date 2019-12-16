---
title: Kan ikke slette elementer i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049526"
---
# <a name="unable-to-delete-items"></a>Kan ikke slette elementer

Har du problemer med å slette SharePoint-elementer?

- Kontroller alltid at du har de [nødvendige tillatelsene](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) til å slette elementet, eller at en [administrator for områdesamling](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) prøver å fjerne elementet.

- Kontroller at det ikke finnes et oppsett for [oppbevaringspolicy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) for elementet.

- Kontroller at elementet ikke er [sjekket ut](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.

- Administratorer kan bruke SharePoint- [mønstre og-metoder](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som inneholder et bibliotek med PowerShell-kommandoer som gjør det mulig å utføre kompliserte administrasjons handlinger, for eksempel tvinge sletting av sta elementer.
- [Fjern PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjern PNP listeelement](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjern PNP-felt (kolonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)