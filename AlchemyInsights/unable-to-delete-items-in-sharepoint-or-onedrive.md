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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038526"
---
# <a name="unable-to-delete-items"></a>Kan ikke slette elementer

- Oppbevaringspolicyer kan føre til dette, du må enten deaktivere eller utelate respektive sperring som forårsaker dette problemet. Når en oppbevaringspolicy eller sperring er fjernet, kan det ta opptil 24 timer før endringen trer i kraft. Kontroller at det ikke er et oppsett [for](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) oppbevaringspolicy på elementet.

- Området kan ha overskredet lagringsgrensen, øke [nettstedskvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) og slette elementet.

- Kontroller at elementet ikke er [sjekket ut](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.

- Til slutt kan administratorer [bruke SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) mønstre og fremgangsmåter (PnP) som inneholder et bibliotek med PowerShell-kommandoer som lar deg utføre komplekse administrasjonshandlinger, for eksempel tvinge til å slette stae elementer.
- [Fjern PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjerne PNP-listeelement](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjerne PNP-felt (kolonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)