---
title: Kan ikke slette elementer i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019592"
---
# <a name="unable-to-delete-items"></a>Kan ikke slette elementer

- Oppbevarings policyer kan føre til dette, enten må du deaktivere eller utelukke den respektive sperringen som for år saker Dette problemet. Etter en oppbevarings policy eller sperring er fjernet, kan det ta opptil 24 timer før endringen trer i kraft. Kontroller at det ikke finnes et oppsett for [oppbevarings policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) for elementet.

- Nettstedet kan ha overskredet lagrings grensen, øke [område kvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) og slette elementet.

- Kontroller at elementet ikke er [sjekket ut](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.

- Til slutt kan administratorer bruke [SharePoint-mønstre og-rutiner](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som inneholder et bibliotek med PowerShell-kommandoer som gjør at du kan utføre komplekse administrasjons handlinger, for eksempel tvinge sletting av stubborn-elementer.
- [Fjern PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjern liste element for PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjern PNP-felt (kolonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)