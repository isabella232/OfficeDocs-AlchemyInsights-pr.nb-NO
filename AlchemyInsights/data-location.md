---
title: Data plassering
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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627855"
---
# <a name="data-location"></a>Data plassering

Du kan vise plasseringen av din Office 365 leier i administrasjonssenteret eller ved å koble til Exchange Online via PowerShell.


**Administrasjonssenter:**
1. Logg på [administrasjonssenteret](https://admin.microsoft.com/Adminportal/Home).
2. Velg **Innstillinger** > **organisasjonsprofil**.
3. Velg **Vis detaljer**under **data plassering**.


**Powershell:**
1. Koble til Exchange Online ved hjelp av Windows PowerShell.
2. Kjør cmdleten [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for å vise en liste over egenskapene for leieren. 
3. Se på OrganizationId-egenskapen.

Når du har data plasseringen for EXO og SPO, kan du bestemme data plasseringen for andre tjenester du kan bruke [der dataene er plassert](https://products.office.com/where-is-your-data-located).