---
title: Dataplassering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655291"
---
# <a name="data-location"></a>Dataplassering

Du kan vise plasseringen til leieren i administrasjonssenteret eller ved å koble til Exchange Online via PowerShell.


**Administrasjonssenter:**
1. Logg på [administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home).
2. Velg **Innstillinger** > **Organisasjonsprofil**.
3. Velg **Vis detaljer**under **Dataplassering**.


**Powershell:**
1. Koble til Exchange Online ved hjelp av Windows PowerShell.
2. Utfør cmdleten [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for å vise en liste over leierens egenskaper. 
3. Se på egenskapen OrganizationId.

Når du har dataplasseringen for EXO og SPO, kan du bestemme dataplasseringen for andre tjenester du kan bruke fra [Hvor dataene dine befinner seg.](https://products.office.com/where-is-your-data-located)