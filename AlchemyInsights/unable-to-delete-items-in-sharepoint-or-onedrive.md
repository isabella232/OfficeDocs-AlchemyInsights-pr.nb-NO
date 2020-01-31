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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571276"
---
# <a name="unable-to-delete-items"></a>Kan ikke slette elementer

Oppbevaringspolicyer kan forårsake dette, må du enten deaktivere eller ekskludere respektive hold som forårsaker dette problemet. Når en oppbevaringspolicy eller hold er fjernet, kan det ta opptil 24 timer før endringen trer i kraft. Kontroller at det ikke er et oppsett for [oppbevaringspolicy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) på varen.

Området kan ha overskredet lagringsgrensen, øke [områdekvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) og slette elementet.

Kontroller at elementet ikke [er sjekket ut](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.

Til slutt kan administratorer bruke [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som inneholder et bibliotek med PowerShell-kommandoer som lar deg utføre komplekse administrasjonshandlinger, for eksempel kraft sletting av vanskelige elementer.
- [Fjerne PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjern PNP-listeelement](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjern PNP-felt (kolonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)