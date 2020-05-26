---
title: Blokkere nedlasting på delingskoblinger
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358037"
---
# <a name="block-download-on-sharing-links"></a>Blokkere nedlasting på delingskoblinger

**Blokknedlasting** er tilgjengelig for bare visningskoblinger til **Office-dokumenter.** Når du velger dette alternativet, vil ikke personer som får tilgang til filen via koblingen du opprettet, se alternativer for nedlasting, utskrift eller kopier filen.

Administratorer kan kontrollere om innstillingen "blokknedlasting" bare vises for Office-filer eller ikke ved å endre `BlockDownloadLinksFileType` innstillingen i [cmdletene Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) eller [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell .
